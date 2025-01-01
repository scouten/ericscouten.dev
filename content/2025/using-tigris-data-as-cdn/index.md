+++
title = "Using Tigris Data as a CDN"
date = 2025-01-01
+++

Hello and welcome to 2025! I'm sharing some fun news about my blog's custom tech stack. I have a new way of hosting the static image content for my blog and I'm really happy about it.

<!-- more -->

A few years ago, [I wrote about how I built the 146 Parks blog](https://ericscouten.dev/2021/how-i-built-146-parks/). What I wrote then has become the backbone of all of my web sites. Almost four years later, and it's all holding up remarkably well. I have no intent of moving from [Zola](https://www.getzola.org) and [Netlify](https://www.netlify.com) as the core technologies that serve my sites.

But ... I have encountered a couple of tech challenges in the last year or so, specifically around how I host large binary content (mostly still images).

To wit:

* **Git's [Large File Storage mechanism](https://git-lfs.com) isn't all that performant.** Put a few thousand large JPEGs in a git repo -- even with Git LFS -- and `git status` and its friends become noticably slower. Not so bad as to be a blocker (several seconds at worst), but ... enough that it made me stop and ask how this might scale when a few thousand becomes many thousand.

* **Netlify [deprecated their Large Media Service](https://answers.netlify.com/t/large-media-feature-deprecated-but-not-removed/100804) in September 2023.** All of my sites use this service because it provided a convenient and optimized link between git repo content and Netlify's content distribution network (CDN). To their credit, Netlify has -- more than a year later -- not yet announced a schedule for shutting down Large Media Service, so those of us who had built a dependency on it have already been given a very comfortable transition window. But ... the writing is on the wall, and I've been on the lookout for a suitable replacement technology.

So, the immortal question comes up ... "Now what?"

## Enter Changelog podcast

So, I was listening to one of my favorite developer podcasts, [The Changelog](https://changelog.com/podcast/).

On [episode 621, "Building the developer cloud,"](https://changelog.com/podcast/621#t=1490) about a month ago, they interviewed Kevin Mackey of [fly.io](https://fly.io) and they dropped some knowledge that was exactly what I needed to hear. Quoting [Adam Stachoviak](https://changelog.com/podcast/621#transcript-91):

> You were talking about [Tigris](https://www.tigrisdata.com), and correcting yourself ... Tigris is basically like the promise of object storage, but it allows you to actually build a CDN. Like, you can basically run a – you can write some JavaScript, use Tigris, and you have a CDN baked into your application. You couldn’t build anything like that before. You could try and do this with S3, but it’s so complicated to like manage multiple regions of data that it’s impossible ...

Ooh, ooh ... 💡!

## An idea is born ...

A few weeks later, I was [travelling in California](https://ericscouten.travel/2024/12-20+california/), and I thought:

> Why not see if it's really as simple as they say?

**It was.**

In the course of a few hours, I was able to provision a storage bucket in Tigris, revise my existing (personal) photo-tooling infrastructure to use it (including the reusing existing off-the-shelf [Rust S3 SDK](https://crates.io/crates/aws-sdk-s3)), and adapt my existing [Zola](https://www.getzola.org) shortcodes to work together.

I'm very happy with how it has all turned out.

I'm now in the process of retrofitting all of my existing web content to move my photos from Netlify Large Media to Tigris Data.

## What is the tech stack now?

I'm not sure if I've shared all of this before, but here is a summary of the technology I use for my web presences as of the beginning of 2025:

* **[Zola](https://www.getzola.org)** -- an excellent Rust-based static site generator
  * **[My custom Zola theme](https://github.com/scouten/zola-es-theme)** -- my customizations for Zola that make this and other sites look they way I want them to
* **[GitHub](https://github.com)** -- core storage for the content
* **[Netlify](https://www.netlify.com)** -- hosting of the rendered site content
* **[Hyvor Talk](https://hyvor.com)** -- commenting and reactions
* _new_ **[Tigris Data](https://www.tigrisdata.com)** -- large binary hosting (mostly images and fonts)
* **[Vimeo](https://vimeo.com)** -- video content hosting

Hope you enjoyed this view into how I build my web sites and I'd love to hear any further thoughts on how things might evolve over time.
