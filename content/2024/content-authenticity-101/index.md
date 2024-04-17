+++
title = "Content Authenticity 101"
date = 2024-04-13
aliases = ["/cai-101", "/cai101", "/ca101", "/ca-101"]
+++

As part of preparing for [Internet Identity Workshop](https://internetidentityworkshop.com) (IIW) next week, I've been refining the presentation I often give about the work of the Content Authenticity Initiative and related projects.

<!-- more -->

I'm posting it here a few days in advance of IIW as an opportunity for conference-goers to have a pre-read ([slide deck](./2024-04-16-iiw-cai-101.pdf)) and as hopefully helpful material for those who can't attend.

## Why Content Provenance?

In my appearance on [**The Future of Identity** podcast](https://www.buzzsprout.com/2132091/14725496-eric-scouten-adobe-s-leading-role-in-the-content-authenticity-boom), Riley Hughes asked me the question with which he closes every episode:

**"What does the future of identity looks like to you?"**

Here's how I answered (at 32′19″ of the recording):

> When I talk about the work that I'm doing with friends and family and people that I meet in the general public, there's a lot of interest in what we're doing. And a lot of that comes down to this fatigue that people feel, this onslaught of information designed to misinform and mislead. So they're really interested in hearing about potential answers to that.
>
> The same is true when I have conversations with people in news media, government, business, entertainment, and sports. They're frustrated that they're losing contact with their audiences because their identities, their likenesses, and their messages are being stolen and corrupted and abused to tell stories that aren't really theirs.
>
> I see us in the technology and identity community stepping forward to say, "Hey, we think we can bring you back into genuine contact with each other."
>
> And so, when I think about the future of identity, I think that you and I and so many other talented people that we work with on the regular have a point in the not-so-distant future where we've had a really big positive impact on the marketplace of ideas.
>
> That's a future I'm super thrilled to be part of.

## Our Approach

Fundamentally our goals are to:

* Allow **content creators** to make tamper-evident, digitally-signed statements about what they've created.
* Allow **content consumers** to evaluate those statements and use them to make trust decisions.

We are _not_ attempting to build a fact-checking or fake image detection system. Those aren't sustainable efforts.

Some examples of things we enable content creators to say:

* location and time of original capture
* actions taken while editing
* thumbnail description of content
* ingredients (other content) incorporated when making new content
* who was involved in creating the content

## Who's Building This Vision?

I'm part of a team at [Adobe](https://adobe.com) that is dedicated to building out the future I described above. We do this through three organizations that we've helped to create:

* **[Content Authenticity Initiative](https://contentauthenticity.org):** CAI is a community of media and tech companies, NGOs, academics, and others working to promote adoption of an open industry standard for content authenticity and provenance. The CAI does outreach, advocacy, and education around these open standards. Content Authenticity Initiative is also the name of the business unit of which I'm a part at Adobe through which we participate in all three of these organizations, develop open source and open standards, and guide implementation within Adobe's product and service suite.

* **[Coalition for Content Provenance and Authenticity](https://c2pa.org):** C2PA is a technical standards organization which ddresses the prevalence of misleading information online through the development of technical standards for certifying the source and history (or provenance) of media content.

* **[Creator Assertions Working Group](https://creator-assertions.github.io):** CAWG builds upon the work of the C2PA by defining additional assertions that allow content creators to express individual and organizational identity and intent about their content.

## Technical Data Model

As part of the IIW presentation, I'll walk through how we translate the above vision into technical reality. This will largely be a recap of the following:

### C2PA Data Model

* Slides 15 through 27 of [IIW slide deck](./2024-04-16-iiw-cai-101.pdf)
* [C2PA Content Credentials Technical Specification, version 2.0](https://c2pa.org/specifications/specifications/2.0/specs/C2PA_Specification.html)

### CAWG Identity Assertion

* Slides 29 through 34 of [IIW slide deck](./2024-04-16-iiw-cai-101.pdf)
* [CAWG Identity Assertion (current working draft)](https://creator-assertions.github.io/identity/1.x-add-vc-v3/)

## More Sessions at IIW

The Content Authenticity 101 talk (Tuesday) or similar knowledge is a recommended prerequisite for two other sessions that I'll be leading on Wednesday or Thursday:

* CAWG identity assertion technical working session
  * More detailed walkthrough of identity assertion
  * "Interesting challenges" using VCs in a broadcast media context

* CAWG identity assertion user experience working session
  * Co-led with Pia Blumenthal, UX lead for CAI at Adobe

## Recent Presentations and Podcast Appearances

I've been invited to give several presentations on our work in the last few months:

* [**Trust Over IP Foundation:** Content Authenticity Initiative and Trust Over IP Foundation Collaboration](https://www.youtube.com/watch?v=pq_fFHMs7sQ) _(21 February 2024):_ My colleague Santiago Lyon, Head of Advocacy and Education for [CAI](https://contentauthenticity.org), and I were the invited guests at the [Trust Over IP Foundation](https://trustoverip.org)'s monthly all-members meeting. We gave an introduction to how CAI works, a technical overview of the [C2PA data model](https://c2pa.org/specifications/specifications/2.0/specs/C2PA_Specification.html), and an early discussion of the [CAWG identity work](https://creator-assertions.github.io/identity/1.x-add-vc-v3/). ([PDF slides](./2024-02-20-toip.pdf))

* [**W3C Credentials Community Group**](https://w3c-ccg.github.io/meetings/2024-03-05/) _(5 March 2024):_ My colleague [Leonard Rosenthol](https://www.linkedin.com/in/lrosenthol/), chief architect for [C2PA](https://www.linkedin.com/in/lrosenthol/), and I presented to [W3C](https://www.w3.org) about C2PA and the [CAWG identity work](https://creator-assertions.github.io/identity/1.x-add-vc-v3/).

* [**ICANN 79:** Digital Trust Panel](https://icann.zoom.us/rec/play/WT_3H1hiqsNjhETwphfZ0XotRoJ1NwMBdGCdsxVcgo_-UvucGFZ3HrqujbrC33k3DhUa-_1OKzunifs1._3gUlV0p-0ENqQOH?canPlayFromShare=true&from=share_recording_detail&startTime=1709745304000&componentName=rec-play&originRequestUrl=https%3A%2F%2Ficann.zoom.us%2Frec%2Fshare%2FtgQRWJcqsyp0QoTP_oZ3rq5mgqwPCiaWP2BVtGA5k4tOrZPcVZDOHeYx5NMnTQgh.qXXceOvRIMqBxhd0%3FstartTime%3D1709745304000) _(6 March 2024):_ I was an invited guest speaker with:
  * [Jacques Latour](https://www.linkedin.com/in/jacqueslatour/) of [CIRA](https://www.cira.ca) as session moderator
  * (1′36″) [Darrell O'Donnell](https://www.linkedin.com/in/darrellodonnell/) of [Continuum Loop](https://www.continuumloop.com) on the challenges of establishing trust on the internet
  * (10′42″) I spoke about [CAI](https://contentauthenticity.org), [C2PA](https://c2pa.org), and [Identity](https://creator-assertions.github.io/identity/1.x-add-vc-v3/) ([PDF slides](./2024-03-06-icann.pdf))
  * (28′51″) Darrell added more context about the non-technical challenges in establishing trust, introduced the concept of Digital Public Infrastructure, and [Trust Over IP](https://trustoverip.org)
  * (36′03″) [Mathieu Glaude](https://www.linkedin.com/in/mathieuglaude/) introduced the concept of trust registries
  * (56′16″) Darrell closed with some additional comments about the establishment of trust registries and an emerging trust layer
  * (1h04′06″) Q&A

* [**The Future of Identity** podcast: Adobe's Leading Role in the Content Authenticity Boom](https://www.buzzsprout.com/2132091/14725496-eric-scouten-adobe-s-leading-role-in-the-content-authenticity-boom) _(20 March 2024):_ [Riley Hughes](https://www.linkedin.com/in/rileyparkerhughes/) of [Trinsic](https://trinsic.id) interviewed me about adoption of the [C2PA standard](https://c2pa.org/specifications/specifications/2.0/specs/C2PA_Specification.html), how the [Content Authenticity Initiative](https://contentauthenticity.org) recruited so many of the most influential tech and media platforms, and how [Adobe](https://www.adobe.com/) built the conviction to ship the first versions into production despite a cold start problem.

* [**SSI Orbit** podcast: Content Authenticity: Combating Deepfakes, Misinformation and Fraud](https://www.youtube.com/watch?v=VnovH1Cxz8g) _(22 March 2024):_ [Mathieu Glaude](https://www.linkedin.com/in/mathieuglaude/) of [Northern Block](https://northernblock.io) interviewed me about the challenges of comating misinformation and disinformation online, how [CAI](https://contentauthenticity.org) aims to differentiate legitimate content, the role of [C2PA's technical standards](ttps://c2pa.org/specifications/specifications/2.0/specs/C2PA_Specification.html) in establishing content provenance, and upcoming strategies for documenting individual and organizational content authorship.

* **[Internet Identity Workshop](https://internetidentityworkshop.com):** Content Authenticity 101 _(16 April 2024):_ This presentation (not recorded) will largely mirror the content in this article.
