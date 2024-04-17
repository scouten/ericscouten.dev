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
_Eric Scouten_

I gave an introductory session titled [Content Authenticity 101](/2024/content-authenticity-101). We had about 30-40 people attend with lots of great questions about identity binding, signature mechanisms, and trust list.

## Session 2L: `did:tdw`
_Stephen Curran_

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
* [Stephen's slide deck](https://docs.google.com/presentation/d/1PHo16asyceRiNKN7UkV8BSmtWtN6Wp3A6_9MV0IQ2jg/edit#slide=id.p)

## Session 3M: Provenance in a ML World
_Matt Miller_

Discussion about image theft and appropriation of identity.

"Overwhelm with the positive (trust signal); ignore the negative."

Discussion about how to have trust in anonymous or pseudonymous content.

Some misconceptions I observed:

* There's a binary distinction between human and generative content. (Where does gen fill fit in?)
* There's a binary distinction between edited and unedited content. (What about photographer's/videographer's choice of what to include in the frame?)
* There's a binary decision to make: trust or not trust. But trust is on a spectrum from closest friend to barbership hearsay.

"I think you just said it sucks to have to make our own (trust) decisions."

[Alethia](https://github.com/danielquinn/aletheia) combines signature with DNS.

[TurnItIn](https://www.turnitin.com) anti-plagiarism tool used in academia.

## Session 4L: Business of SSI and Authentic Data
_Timothy Ruff_

DTV founded in 2019 to launch new SSI businesses.

2022-2024 incubating more startups in health care, trade, securitization, and more.

Business model challenges:

* A use case isn't a business model.
* The tech is the easy part; making money is the hard part.
* Too focused on individuals. Re SSI: "We want this more for people than they want it for themselves."
* Get organizations on board, then the individuals will follow.
* Focused on identity at the expense of authentic _data._
* Well-funded competitors and sensitive data.
* Web3, blockchain, etc. have a not-wonderful reputation in many circles. "It's lost it sizzle."
* The term "self-sovereign" causes allergic reactions esp. among governments.

Suggestions:

* Follow _Running Lean_ by Ash Maurya (a student of Eric Rees)
* Look for problem-**solution** fit (not product-_market_ fit)
* Read _The Mom Test_. (tl;dr: Everyone will lie to you even if they don't think they're lying to you. Work around this by asking about _existing_ behavior, not to predict future behavior.)
* Spend more time understanding the problem, not the product. "Fall in love with your customer's problem. The solution will fall out when you really understand the problem."
* Look for multi-sided markets. In such an environment, find the "queen bee" who controls the overall ecosystem. Understand _their_ problem and you move the market. (Example: European Banking Authority and managing login systems for 6000 banks and their regulatory filings.)
* Find minimum viable "route" for success. Show the solution in the small, then it will grow.
* Be prepared to pivot. Timothy's example:
  * Proprietary -> blockchain -> KERI
  * VCs -> ACDCs
  * DIDs -> AIDs
  * ZKPs -> graduated disclosure
  * SSI -> B2B (the "route" to adoption)
* Be a truth-seeker. "Strong opinions loosely held."

"The technology in this space has a half-life of about five years." 🎤 drop

# Wednesday Sessions

## Session 6C: Content Authenticity 201: Technical Challeges in CAI + VC Binding
_Eric Scouten_

I led a discussion about some of the interesting challenges we're facing as we work to bind varying kinds of credentials to the CAI/C2PA/CAWG ecosystem.

[Slide deck](./iiw38-identity-session.pdf)

![Me, making a point](jw-244-a379.jpg)

![Audience](es-244-8686.jpg)

Some discussion in response to my slides:

* **Broadcast application** _(slide 26):_ Encode as much as possible into the asset VC. This also helps mitigate the "phone home" at time of verification potential harm.
* **Interoperability** _(slide 29):_ Sam suggested to focus on major example DID methods. There's an upcoming registry of DID methods supported by US gov. Pay attention to that. Also, someone recommended using the [DIF Universal Resolver](https://dev.uniresolver.io) to address the DID interop issue. Universal Resolver understands about 60 methods, which is probably a good starting point for what to support.
* **Duplicate identity** _(slide 30):_ Perhaps the DID identifier is more important than the name.
* **Bulk signing** _(slide 31):_ As long as consent is there, authorization of each one is not important.
* **Social media** _(slide 32):_ No standard exists today.

Scott Perry approached me afterwards and encourged me to review the [ToIP Issuer Requirements Guide for Governance Frameworks for Verifiable Credentials](https://trustoverip.org/permalink/Issuer-Requirements-Guide-V0.01-2024-01-30.pdf). This document provides guidances for several of the thorny questions I raised in the session.
## Session 9M: High Assurance DIDs with DNS
_Mathieu Glaude, Tim Bouma, Jesse Carter_

_Check for link and spec after meeting._

Design goal: How can we take a friendly DID method (`did:web`) and add high assurance without adding a lot of complexity.

Problem statement: Idetifiers today are either easy to recognize _or_ easy to verify but rarely if ever both.

Solution: Develop formal guidance for formally binding DID with DNS infrastructure.

Starting from `did:web:issuer.trustregistry.ca`, how can we provide machine-verifiable assertions?

* Leverage DNSSEC to **cryptographically-assured binding** of domain name to X.509 and TLS certs
* Enable a **digitally-signed** DID document

No new infrastructure required.

Tim Bouma: Think of this as 2FA for DID docs.

Using existing DNS record fields and DID document content that are already standardized.

Follow-up: What is Canonical JSON?

Replicate key portions of the DID document (proof?) in DNS records as a safeguard against server compromise.

Look at [DNSViz](https://dnsviz.net), a tool for verifying the status of a DNS zone.

Links:

* [Slide deck](https://docs.google.com/presentation/d/1u6GK7oWw-ewB3lONncI1CfcMpiJ2zUT8LrUGRLuV1w8)
* [Draft specification on GitHub: CIRALabs / high-assurance-dids-with-dns](https://github.com/CIRALabs/high-assurance-dids-with-dns)
* [IETF Draft RFC](https://www.ietf.org/archive/id/draft-carter-high-assurance-dids-with-dns-03.html)

Current implementations:

* [trustregistry.ca](https://trustregistry.ca)
* [trustroot.ca](https://trustroot.ca)
* [Trust Registry HA DIDs](https://trustregistry.nborbit.ca/)
* [Implementation in DID resolver](https://godiddy.com/)
