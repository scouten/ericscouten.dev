+++
title = "Internet Identity Workshop 38"
date = 2024-04-16

[extra]
markers = "markers.js"
bounds = {sw = [37.404, -122.087], ne = [37.424, -122.067]}
cover = "es-4640-061"
toc = true
+++

This week I'm attending the 38th biannual **[Internet Identity Workshop](https://internetidentityworkshop.com),** which is one of the most valuable conferences I've encountered in any professional space. As the name might suggest, the topics are largely around how to express human and organizational identity in digital terms that respect privacy and security. When I attended the previous IIW last fall, [I wrote about it in real time](/2023/iiw) as the conference was in progress. That format worked well for me and received a lot of compliments, so I'm attempting it again this week.

<!-- more -->

# Why Am I Here?

I'm part of a team at [Adobe](https://adobe.com) that is dedicated to helping content creators and content consumers establish genuine connections with each other. We do this through three organizations that we've helped to create:

* **[Content Authenticity Initiative](https://contentauthenticity.org):** CAI is a community of media and tech companies, NGOs, academics, and others working to promote adoption of an open industry standard for content authenticity and provenance. The CAI does outreach, advocacy, and education around these open standards. Content Authenticity Initiative is also the name of the business unit of which I'm a part at Adobe through which we participate in all three of these organizations, develop open source and open standards, and guide implementation within Adobe's product and service suite.

* **[Coalition for Content Provenance and Authenticity](https://c2pa.org):** C2PA is a technical standards organization which addresses the prevalence of misleading information online through the development of technical standards for certifying the source and history (or provenance) of media content.

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

{{ es_image(id = "es-4640-061", caption = "Computer History Museum, Mountain View, California") }}

{{ es_image(id = "es-4640-063", caption = "Computer History Museum, Mountain View, California") }}

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

{{ es_image(id = "es-4640-077", caption = "Computer History Museum, Mountain View, California") }}

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

{{ es_image(id = "jw-244-a379", caption = "Me, making a point. · Computer History Museum, Mountain View, California", creator = "Jin Wen") }}

{{ es_image(id = "es-4640-084", caption = "Computer History Museum, Mountain View, California") }}

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

## Session 10C: Credential Schemas at DIF
_Kim Hamilton Duffy, Otto Mora_

[Slide deck](https://docs.google.com/presentation/d/12hKsOIubyTI7zigMiChmDjTFVK40GBtM8cZM6eeQYHw/edit)

**Goal:** Develop and publish credential schemas to support interoperability.

**Outputs:**

* Guidance examples
* Per type of schema:
  * Purpose, use, alignment, recommendations
  * Abstract data model
  * Mapped schemas for different formats
* Reawakened work item within claims and credentials WG within DIF

**Viewpoint:** Credential schemas provide improved interoperability, discoverability, ease-of-use, and standardization.

Some examples they're working on:

* Basic KYC model
* Proof of humanity
* Proof of age
* Anti-money-laundering

Audience suggestion: DIF should create guidance on how to create new credential types. (Strong agreement from me!)

Some examples of credential schema registries:

* [Credential Finder](https://credentialfinder.org)
* [Polygon Schema Explorer](https://schema-builder.polygonid.me)
* DIF will be building one.

DIF motivation to promote alignment in credential type.

# Thursday Sessions

## Session 11B: Content Authenticity: UX Challenges with Identity
_Pia Blumenthal, Eric Scouten_

[Slide deck](./cawg-ux-for-iiw.pdf)

Notes adapted from audience member Zaïda Rivai. Thank you!

Pia raised several discussion questions:
* Should there be a universal verifier? 
* Who is the owner of that identity?
* Do different types of identity verifications warrant different UI treatment? 
* What level do we need to surface these? 
* The number of identity assertions do we need?
* Do we only ever show things that are verified or can we also share self-asserted information (which is less trustworthy).

**Alex:** UI/UX in Cheqd have the same issue in the team how to display VC easily.

**Pia:** How much verification is needed to provide trust? Single? Proof who you are? Do you have a list of best practices? 

**Alex:** Trust is diagonal. 
* Vertical: within a company 
* Horizontal: “I trust Riley, I’m not working at Trinsic, but I met him.” Creators to accredit other creators and having companies having the vertical trust. 
* Diagonal: is the best

**Judith (ToIP):** How we do everything, but from a specific context, how is that governed> 
How is this covered today in different media outlets? And then getting to the point of trust registries: “This ecosystem recognizes X and this ecosystem trusted Y.” 

**Lorie:** Also a legal problem but onboarding legal frameworks, signatures exist. That is one moving level. KYC is also well known and describe a level of trust is a different thing. But like Alex is the sum of all the parts.

**Drummond:** Don’t get enough UX designers. Gen team is leaning into this. Most of the technical questions are answered, but all are about UX. Literally same as you (Pia) put up here. One context, one specific service. It is a hard problem. 

**Cam:** Is this a problem that needs to be solved? Enough user basis, real problem. Should we prioritize or other problems that have more user aid. 

**Riley:** Interested whether media platforms have different trust requirements. Twitter has their platform and they may be okay with strong verification checkmark but not okay if it would be only oAuth. Is there a mechanism for a platform the users consuming through, tailored the trust decision? Wonder whether the platforms and media whether they want to make the trust decisions for the users. Something that’s considered? 

**Pia:** Progressive disclosure. Implementer chooses what information to highlight. Level 1 and 2.  People don’t necessarily want to see bugs _(overlay icons)_ over top of their content. Up to the implementer to figure what the right information is for that audience. At Adobe, we prioritize AI disclosure. When AI generated or edited with gallery mixed creator work. Might not be the case somewhere else. In C2PA implementations we created a tiered experience. Some only show how it’s created, other show who is involved, the audience has to understand that it’s this model (progressive disclosure).

**Judith:** Think that UI specifically is important for the end user to understand. Getting the interaction patterns, UX is very difficult. UX group, digital wallet survey and coming to what is the next project?

**Alex:** Maybe there should also be a creator reputation WG: completely separate goal to assertions.

{{ es_image(id = "es-4641-002", caption = "Computer History Museum, Mountain View, California") }}

## Session 12A: A Bridge to the Future: Connecting X.509 to DIDs and VIDs
_Drummond Reed, Eric Scouten, Scott Perry, Stephen Curren_

{{ es_image(id = "jf-244-2470", caption = "Computer History Museum, Mountain View, California", creator = "Judith Fleenor") }}

{{ es_image(id = "jf-244-2473", caption = "Computer History Museum, Mountain View, California", creator = "Judith Fleenor") }}

### X.509 Overview

Scott introduced the CA mechanism which is used by browsers to make the trust/don't trust decision in HTTPS interaction. Each browser has its own governance mechanism, but they work together via the CA Browser Forum to share governance requirements known as Web Trust.

EU has its own trust infrastructure via ETSI. EU has a certification structure driven by EIDAS 1.

C2PA is evolving its own distinct trust infrastructure via its Trust List Task Force.

Browsers have worked together to require a control process for certificate issuance tracking known as Certificate Transparency Log, meant to prevent fake CAs from pretending to have issued certs.

### DID/VID Overview

DID = Decentralized Identifier (W3C standard ~2 years ago). Ties public key, private pair, and identifier. Many but not all DID methods allow continuity of identity across private key rotation.

VID = ToIP concept, related to DID, but removing some of the syntactic requirements.

VID is an effort to reopen the tent.

### Comparisons

In X.509, issuer is necessarily always a CA as a means of enforcing the governance rules. DIDs are much more open in issuance. X.509s could be considered VCs, but in a different format and with stricter governance.

DIDs and VCs split the human readable part vs the machine-readable part.

DIDs allow governance to be added post-hoc. A DID can be attached to a VC at a later point depending on the governance or requirements of the DID holder.

{{ es_image(id = "es-4641-003", caption = "Diagram with X.509 and DID/VC comparison. · Computer History Museum, Mountain View, California") }}

### Is This a Bridge Worth Building?

Challenge that ToIP did:x509 TF has encountered: How do you retain a persistent identifier given that X.509 certs have to be periodically rotated? Maybe we don't.

Maybe the answer is to invert that. What if we encode a DID into X.509 subject alternative name (SAN) or similar field?

CA may or may not be able to use SAN depending on type of cert requested.

So can we describe a way for CSR (Certificate Signing Request) to include proof of control over the private key associated with the DID?

Lucy Yang and her company did a conversion of X.509 to DID a few years ago as part of WHO COVID credentials effort. (TO DO: Add link to this effort if possible.)

EBSI is working toward this using exactly this approach. (Follow up with Alex Tweeddale.)

California DMV is referencing X.509 chain via `x5c` parameter in a `did:jwk`.

Look into EBSI verifiable accreditation mechanism. Alex Tweeddale sent a link to a [presentation he did regarding EBSI trust chaining](https://docs.google.com/presentation/d/1SgquY8Gjm4MddkjbEbQ-_KumyOADic1u31OmXsBbiSg).

{{ es_image(id = "es-4641-004", caption = "Alex’s sketch of EBSI verifiable accreditation mechanism. · Computer History Museum, Mountain View, California") }}
