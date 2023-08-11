+++
title = "I Built My Own Linkroll"
date = 2023-07-04
+++

Ever have that feeling that you might run across something on the web and hope you can find it again someday?

Yeah, me too.

So I built my own linkroll.

<!-- more -->

**tl;dr:** If you're just interested in the linkroll, you can find it at ~~This Might Be Useful~~, which I often abbreviate as TMBU.

**August 2023 Update:** I've since renamed TMBU to [ericscouten.link](https://ericscouten.link). I've updated the links accordingly, but the name lives on in some related code as you'll see below.

Things you'll find there:

* lots of developer-related things (especially related to the Rust language)
* some photography things
* a few travel links
* and some random stuff beyond that.

Yes, I know there are linkroll solutions out there. I've even used a couple of them over time (notably Digg, once upon a time).

Call me an old curmudgeon, but I'm increasingly of the opinion that I want to own my own content and not have my online presence be subject to anyone else's business whims, which is why my links are self-hosted and not on anyone else's platform.


## Design Goals

Since we all have our own notions of what such a site should entail, let me share my goals (✅) and non-goals (❌) for this site:

* ✅ self-hosted site (see earlier commentary)
* ✅ easy for me to add new links
* ✅ publicly visible
* ✅ publicly searchable
* ❌ letting other people contribute links
* ❌ letting other people comment on links
* ❌ building a generalized linkroll tool

## Alternative Considered: Mastodon Itself

A lot of my content these days comes from a [well-curated list of follows on Mastodon](https://ericscouten.social/@scouten/following). Theoretically, I could search posts and boosts on Mastodon to accomplish most of my linkroll goal, except for three things:

1. Not *everything* I'm interested in comes from Mastodon.
2. The overlap between what I boost on Mastodon and what I might want to find later is incomplete in both directions.
3. The Mastodon culture is [notoriously hostile to search efforts](https://searchtodon.social/Adventures-in-Mastoland.html).

So I built my own linkroll.

## Alternative Considered: Private Bookmarks

Someone close to me asked me why I wouldn't just use browser bookmarks. Which also _almost_ works, but ...

1. I want my bookmarks and my commentary on them to be public.
2. I don't really want to be tied to any particular browser or its bookmark sync technology.

So I built my own linkroll.

## How I Built It

A significant part of the art of being a programmer is to identify relevant technology that already exists and figure out how to combine it in the most minimal new way. I'd say I found some pretty good off-the-shelf components to use.

And, of course, I did build a few new pieces.

### The Core: Zola

Almost all of my web presences these days (including this one) are built using [Zola](https://www.getzola.org), a super-fast [static-site generator](https://jamstack.org/generators/) built in the [Rust](https://www.rust-lang.org) programming language. The only current exception is my primary site, [ericscouten.com](https://ericscouten.com), and I have plans for a Zola-based makeover soon.

Zola neatly satisfies most of the design goals I listed above and I built the core of the site using Zola several months ago using templates that I had built for my other sites, including this one. I use [Netlify](https://www.netlify.com) to automatically deploy and build my site, but could pretty quickly move elsewhere if the platform stops working for whatever reason.

### Ruh Roh: I Stalled Out!

The source code for the site is available on [GitHub @ scouten/ericscouten.link](https://github.com/scouten/ericscouten.link/). If you look at the commit history, you'll see a big burst of energy from when I started the site in mid-February until early March.

And … then … nothing.

🦗 _crickets_ 🦗

### What Happened?

Well, the typically workflow was that I'd see something on Mastodon, typically on my iPhone, using the delightful [Ivory](https://tapbots.com/ivory/) client from Tapbots.

I'd e-mail myself a copy of the link when I found it and then circle back later, read that e-mail, and manually convert that into a Zola post and push it to GitHub.

What happened was that _manually_ part began to feel tedious. _Really_ tedious.

By the time I circled back to the posts a couple of days ago, I had more than 100 such messages and there was **no way** I was going to do this manually.

### The Solution: Automate It!

So, having a bit of time to myself this week thanks to a summer vacation (read: Adobe's [excellent sabbatical program](https://benefits.adobe.com/us/time-off/sabbatical)), I built a tool that would read my (purpose-specific) inbox, parse out some relevant bits from the message, and write most of the desired Zola post.

I'm making this tool available via open-source ([GitHub: scouten/tmbu-worker](https://github.com/scouten/tmbu-worker)).

A couple of quick notes about this tool:

* I'm a huge fan of the [Rust](https://rust-lang.org) programming language, so the tool is written in Rust.
* Though licensed under a permissive open-source (MIT) license, this is really "inspire-ware." I do not plan to invest the effort to make this into a larger general-purpose tool. [More details here](https://github.com/scouten/tmbu-worker#status-of-this-project).

This tool wouldn't have been possible without the following open-source crates:

* [imap](https://crates.io/crates/imap)
* [regex](https://crates.io/crates/regex)
* [reqwest](https://crates.io/crates/reqwest)
* [serde](https://crates.io/crates/serde)
* [titlecase](https://crates.io/crates/titlecase)

Thank you to the authors of these crates!

## Bottom Line

Using this automation enabled me to change the time it took me to prepare a new bookmark from 10-20 minutes per post to roughly 3 minutes per post. That makes it really close to sustainable. I cleared the 100+ message backlog in just a couple of days, and expect to keep up with new "might be useful" content going forward.
