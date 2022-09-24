+++
title = "How I Built 146 Parks"
date = 2021-06-05

[extra]
cover = "146-parks-on-zola"
comments = true
+++

Since last fall, I have been working on a project to visit, photograph, and document each of the [146 state parks](https://146parks.blog) in my home state of Washington in the U.S. Normally _this_ site will be devoted to my life as a developer, but today I will incorporate the outdoor-explorer and photographer parts of my life. This is an article about how I built the blog for the 146 Parks project.

<!-- more -->

Here is a screen shot from the current home page:

![Gingko Petrified Forest on Zola](./146-parks-on-zola.jpg)

## Initial Launch: Squarespace

I first launched the site using [Squarespace](https://www.squarespace.com) last fall. 

Here is an equivalent screen shot from the old version of the site:

![Gingko Petrified Forest on Squarespace](./146-parks-on-squarespace.jpg)

The good news about launching on Squarespace: I was able to test the concept, build a prototype design, and share some of the initial posts very quickly.

But there were some definite downsides as well:

* **I wound up spending a lot of time expressing the same concepts over and over.** For example, the maps that I include needed to be rebuilt for each page and I needed to remember to apply the same settings each time.
* **I rather quickly hit the limits of what I could build with their template system.** Again, regarding the maps on each page, I could only put a single marker on each individual page.
* **Perhaps most seriously, I repeatedly experienced data loss while composing my content.** Squarespace's interface often involves going several layers deep in modal dialogs. When I found myself in the wrong dialog, my instinct was to hit the Escape key a time or three to get out of that modal world. The problem is that the Escape key _also_ exits the editing experience. So if I miscalculated on how many times to hit Escape, I lost my work-in-progress content. This happened several times.

## The Goals

**I wanted to be able to build the site while off-line.** Back in the Before Times, I would often work on my sites from places with very limited internet access. A B&B in Ireland a few years ago sticks out as a particularly painful authoring experience on Squarespace. Ironically, as I write the first draft of this article I am on a plane with mediocre Internet access.

**I wanted deep control over the site design.** And yet, I didn't want to have to build the whole thing from scratch.

**Being a good software developer, I like doing things efficiently.** And I like writing text using a code editor.

## Previous Experience

It turns out I've been down this road before. Long-time readers of mine might remember that I [rebuilt my primary site](https://www.ericscouten.com/articles/new-site/) in 2018 using a static site generator, which let me build that site using a combination of HTML templates and [Markdown](https://en.wikipedia.org/wiki/Markdown).

That part felt right to me, but the SSG that I use there, [Jekyll](https://jekyllrb.com), felt heavyweight to me (lots of work to get the right version of Ruby installed, etc.), so I decided to look for something easier to use and maintain.

## I Got Zola

I've been doing most of my professional work in the [Rust](https://www.rust-lang.org) language lately, so I was _very_ happy to learn that there are a few good Rust-based static site generators.

**I settled on [Zola](https://www.getzola.org).** Zola's own site does a good job of describing its benefits, but I feel the need to call out one more: the templating system **rocks.** What I especially like is that it offers a mechanism for reuse and customization. This played out in a way that was a pleasant surprise for me.

Although the Zola project no longer directly links to it, I also found the [Bulma](https://bulma.io) CSS framework very valuable.

So I first rebuilt 146 Parks using Zola and Bulma. The new version of the site launched a few weeks ago and I couldn't be happier with how it turned out.

I then had the idea to start rebuilding the rest of my web presence. That project is ongoing, but you're reading one part of that project now.

I refactored my 146 Parks theme into a shared theme with some common elements that I am now using for other sites.

The sites may not look much alike, but this site, my new [travel blog](https://ericscouten.travel), and [146 Parks](https://146parks.blog) are all built on the same shared theme with relatively little custom template code for each.

## Have a Look Around

I'm open-sourcing the repos behind each site and the shared theme here:

* **[146 Parks](https://146parks.blog)**: [GitHub](https://github.com/scouten/146parks.blog)
* **[ericscouten.dev](https://ericscouten.dev)**: [GitHub](https://github.com/scouten/ericscouten.dev) _(this site)_
* **[ericscouten.travel](https://ericscouten.travel)**: [GitHub](https://github.com/scouten/ericscouten.travel) _(an up-and-coming blog about my non-state-park travels)_
* **[zola-es-theme](https://github.com/scouten/zola-es-theme)**: _(the shared theme behind all of these sites)_

These are all provided as-is and as what I will call "inspire-ware." I don't wish to enable outright clones of my look and feel, and for that reason I'm not applying a traditional open-source license to them. If you find a snippet that helps you, feel free to adapt it for your purpose. But, please, make your site yours.

Hope this tour of Zola was helpful!
