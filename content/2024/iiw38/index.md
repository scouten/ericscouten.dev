+++
title = "Internet Identity Workshop 38"
date = 2024-04-16

[extra]
toc = true
+++

This week I'm attending the 38th biannual **[Internet Identity Workshop](https://internetidentityworkshop.com),** which is one of the most valuable conferences I've encountered in any professional space. As the name might suggest, the topics are largely around how to express human and organizational identity in digital terms that respect privacy and security. When I attended the previous IIW last fall, [I wrote about it in real time](/2023/iiw) as the conference was in progress. That format worked well for me and received a lot of compliments, so I'm attempting it again this week.

<!-- more -->

# Why Am I Here?

I'm part of a team at [Adobe](https://adobe.com) that is dedicated to helping content creators and content consumers establish genuine connections with each other. We do this through three organizations that we've helped to create:

* **[Content Authenticity Initiative](https://contentauthenticity.org):** CAI is a community of media and tech companies, NGOs, academics, and others working to promote adoption of an open industry standard for content authenticity and provenance. The CAI does outreach, advocacy, and education around these open standards. Content Authenticity Initiative is also the name of the business unit of which I'm a part at Adobe through which we participate in all three of these organizations, develop open source and open standards, and guide implementation within Adobe's product and service suite.

* **[Coalition for Content Provenance and Authenticity](https://c2pa.org):** C2PA is a technical standards organization which ddresses the prevalence of misleading information online through the development of technical standards for certifying the source and history (or provenance) of media content.

* **[Creator Assertions Working Group](https://creator-assertions.github.io):** CAWG builds upon the work of the C2PA by defining additional assertions that allow content creators to express individual and organizational identity and intent about their content.

I recently published an article titled **[Content Authenticity 101](/2024/content-authenticity-101.md),** which explains these organizations and our motivations in more detail.

## The Venue

IIW is held at the lovely **[Computer History Museum](https://computerhistory.org/)**, which recounts the formative years of our tech industry. CHM is located in Mountain View, California, right in the heart of Silicon Valley.

I'll share a few photos of the venue and the conference. My non-technical friends might want to bow out after this section as it will rapidly descend into lots of deep geek speak.

## The Format

IIW is conducted as an **"[unconference](https://en.wikipedia.org/wiki/Unconference),"** which means that there is a pre-defined _structure_ to the conference, but not a predefined _agenda._

There are several variations on how the agenda gets built at an unconference. In IIW's case, there is an opening meeting on each morning in which people stand up and describe sessions they'd like to lead that day. Then there's a mad rush to schedule these sessions (see photo below) and we all choose, in the moment, which sessions to attend.

![An as-yet empty schedule board.](/2023/iiw/es-4579-010.jpg)

You might think that not having a predefined agenda would mean that the topics that occur could be flimsy or weak or low in value. In practice, the opposite is true. Both times I've attended this conference so far, I've had to make very difficult choices about which sessions _not_ to attend so I could attend something else which was _also_ very compelling.

With that, here is my description of the sessions I'm attending this time around:

# Tuesday Sessions

## Session 1C: Content Authenticity 101

I gave an introductory session titled [Content Authenticity 101](/2024/content-authenticity-101). We had about 30-40 people attend with lots of great questions about identity binding, signature mechanisms, and trust list.

## Session 2L: `did:tdw`

Simplified version of DID with key rotation sponsored by BC Government.

<1000 lines of code to implement.

Intended to incorporate key concepts from KERI, but not take on the complexity of KERI.

Compatible with `did:web`!

Still to do: DID challenges.

Ohhh, wait ... they have DID issuer trust chaining built in via `/did/whois`.

Heading to standardization (IETF likely) soon.

Links:

* [Specification](https://github.com/bcgov/trustdidweb)
* [TypeScript implementation](https://github.com/bcgov/trustdidweb-ts/)
* Stephen's slide deck](https://docs.google.com/presentation/d/1PHo16asyceRiNKN7UkV8BSmtWtN6Wp3A6_9MV0IQ2jg/edit#slide=id.p)

## Session 3M: Provenance in a ML World

Discussion about image theft and appropriation of identity.

"Overwhelm with the positive (trust signal); ignore the negative."

Discussion about how to have trust in anonymous or pseudonymous content.

Some misconceptions I observed:

* There's a binary distinction between human and generative content. (Where does gen fill fit in?)
* There's a binary distinction between edited and unedited content. (What about photographer's/videographer's choice of what to include in the frame?)
* There's a binary decision to make: trust or not trust. But trust is on a spectrum from closest friend to barbership hearsay.

"I think you just said it sucks to have to make our own (trust) decisions."

Elithia combines signature with DNS.

Tonaten (sp?) anti-plagiarism tool used in academia.
