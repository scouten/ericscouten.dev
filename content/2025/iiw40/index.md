+++
title = "Internet Identity Workshop 40"
date = 2025-04-08

[extra]
toc = true
+++

This week I'm attending the 40th biannual **[Internet Identity Workshop](https://internetidentityworkshop.com),** which is one of the most valuable conferences I've encountered in any professional space. As the name might suggest, the topics are largely around how to express human and organizational identity in digital terms that respect privacy and security.

<!-- more -->

# Why Am I Here?

I'm part of a team at [Adobe](https://adobe.com) that is dedicated to helping content creators and content consumers establish genuine connections with each other. We do this through three organizations that we've helped to create:

* **[Content Authenticity Initiative](https://contentauthenticity.org):** CAI is a community of media and tech companies, NGOs, academics, and others working to promote adoption of an open industry standard for content authenticity and provenance. The CAI does outreach, advocacy, and education around these open standards. Content Authenticity Initiative is also the name of the business unit of which I'm a part at Adobe through which we participate in all three of these organizations, develop open source and open standards, and guide implementation within Adobe's product and service suite.

* **[Coalition for Content Provenance and Authenticity](https://c2pa.org):** C2PA is a technical standards organization which addresses the prevalence of misleading information online through the development of technical standards for certifying the source and history (or provenance) of media content.

* **[Creator Assertions Working Group](https://cawg.io):** CAWG builds upon the work of the C2PA by defining additional assertions that allow content creators to express individual and organizational identity and intent about their content. **NEW:** As of March 2025, CAWG has become a working group within the [Decentralized Identity Foundation (DIF)](https://identity.foundation).

Last year, I published an article titled **[Content Authenticity 101](/2024/content-authenticity-101.md),** which explains these organizations and our motivations in more detail.

## The Venue

IIW is held at the lovely **[Computer History Museum](https://computerhistory.org/)**, which recounts the formative years of our tech industry. CHM is located in Mountain View, California, right in the heart of Silicon Valley.

I'll share a few photos of the venue and the conference. My non-technical friends might want to bow out after this section as it will rapidly descend into lots of deep geek speak.

## The Format

IIW is conducted as an **"[unconference](https://en.wikipedia.org/wiki/Unconference),"** which means that there is a pre-defined _structure_ to the conference, but not a predefined _agenda._

There are several variations on how the agenda gets built at an unconference. In IIW's case, there is an opening meeting on each morning in which people stand up and describe sessions they'd like to lead that day. Then there's a mad rush to schedule these sessions (see photo below) and we all choose, in the moment, which sessions to attend.

{{ es_cdn_image(id = "es-4579-010", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4579-010", caption = "An as-yet empty schedule board.") }}

You might think that not having a predefined agenda would mean that the topics that occur could be flimsy or weak or low in value. In practice, the opposite is true. Both times I've attended this conference so far, I've had to make very difficult choices about which sessions _not_ to attend so I could attend something else which was _also_ very compelling.

With that, here is my description of the sessions I'm attending this time around:

# Tuesday Sessions

## Session 1H: DID Methods Update
_Markus Sabadello, Danube Tech_

Update on the various working groups working on DID methods.

### W3C

Has ratified the as a [DID Core 1.0](https://www.w3.org/TR/did-1.0/) standard recommendation. New [W3C DID WG](https://www.w3.org/2019/did-wg/) is currently building:

* DID 1.1 standard
  * No breaking changes
  * Adding dependency on the [CID 1.0](https://www.w3.org/TR/cid-1.0/) spec (controlled identifier), which is a generalization of the DID document for non-DID identifiers. Note that the DID document spec is moved from DID Core 1.0 to CID 1.0, but is backward compatible.
  * Introduces a new media type `application/did` which can be used as a simplification compared to `application/did+json` or `application/did+ld+json`

* DID resolution and DID URL dereferencing 1.0 -- adds detail around
  * Algorithms
  * Parameters, metadata, error coes
  * HTTPS bindings

* DID extensions registry
  * Helping to specify behaviors of DID resolver, for example:
    * Translate public key representations
    * Translate relative URIs to absolute URIs
    * Constrain to public keys that are used for specific purposes
    * Look up DID document at a specific version or point in time

### [DIF DID Methods WG](https://identity.foundation/working-groups/did-methods.html)

(Collaboration between DIF, W3C CCG, ToIP, and INATPA.)

This WG is intended to address the question of "which DID methods should be used and implemented." This is an effort to curate the currently-overwhelming list of DID methods.

So far, this group has:

* Selection criteria (How would the WG choose a shortlist of DID methods?)
* Proposing approved/endorsed DID methods (currently about 10 are under consideration)

Related to currently-proposed [W3C DID Methods WG](https://w3c.github.io/did-methods-wg-charter/2025/did-methods-wg.html).

Likely outcome: A curated list of "DIF-endorsed DID methods" which may be formally standardized elsewhere (DIF, EBSI, W3C, ToIP, etc.).

See also (crunched for time at the end):

* DID Traits
* Linked VPs
* Trust Over IP High Assurance VIDs _(linking DIDs to X.509 or web domain)_

## Session 2M: Ayra: Are Ecosystems Really That Hard? – and First Person Credentials
_Darrell O'Donnell and Drummond Reed_

### [Ayra](https://ayra.forum)

Swiss non-profit that aims to build trust ecosystems.

Ayra facilitates ecosystem interoperability.

Each ecosystem (including Ayra itself) governs itself and runs its own trust registry and decides who are legitmate issuers and verifiers within its own ecosystem.

Ayra offers:

* trust registry
* conformance suite

We need to know that connections between any wallet and any data consumer will work.

Business -> Governance -> Tech -- in that order.

Ayra follows a process to ensure that Ayra creates value for each member and partner.

1. **Business:** - do we have a business case and resources to make the impact that is needed?
2. **Governance:** - Do we have sufficient governance to create a simple ecosystem for the business case?
3. **Technical:** Is the technology "sufficiently there?"

Ayra is exploring 2-3 projects in next several months.

### The First Person Project

(Stay tuned for demo in session 4 today.)

Define "first person:" (See Doc Searles' blog post from a decade ago.) Meaning that the identifier is acting in your interest first and foremost. Avoiding the terms "user-centric" and "self-sovereign" because they have become overloaded and contentious.

Bhutan no longer allows username and password for access to government services. 50%+ of country uses national digital ID, which is truly SSI.

DIDs are not enough -- we need SCIDs. A SCID is "the most self-sovereign identifier." It can be generated for free and retained for life.

There are several SCID-based DID methods:

* `did:webs`
* `did:webvh`
* `did:jlinc` (FedID)
* `did:plc` (BlueSky)
* `did:scid` (ToIP) – which rules them all because it can be:
  * peer-to-peer
  * web-based
  * blockchain-based
  * DHT-based

Drummond thinks `did:scid` is the DID method we need for first-person identifiers.

Much more detail in Drummond's [slide deck (PDF)](./02m-drummond-reed-intro-to-first-person-project.pdf) or [Google Slides](https://docs.google.com/presentation/d/1-ca4U5dgld2MkP12TqixOBae5UCf0B1yzPm9Tbbx0Rg/edit?slide=id.g34043a2cb7c_0_0#slide=id.g34043a2cb7c_0_0).

## Session 3G: Switchchord + `did:webs` for vLEIs
_Cole Davis, Switchchord, Lance Byrd, GLEIF, and Jonathon Rayback_

Switchchord moving from `did:web` to `did:webs`. Bringing "full decentralization" to an industry that is "historically not good with tech."

Why? Gives assets and songwriters portability without tying them to specific domains or key holders. Cole: "It gives me a lot of building blocks to marry the worlds of legal and cryptography."

Advantage: `did:webs` can be bound to a vLEI. But ... `did:webs` is undergoing major revision to the current draft to incorporate multi-sig.

Switchchord is working on enabling `did:webs` in production. (Behind a feature flag for now.)

## Session 4L: Demo of First Person Credentials and Verifiable Reliationship Credentials
_Drummond Reed and several others_

Early (alpha) version of mobile app that demonstrates first person credentials and creation of in-person relationships.

It's a "key signing party."

Ooh, cool, all the data exchange is offline.

This is foundational to what Linux Foundation wants to address the open-source supply chain risks.

Group is planning to come back to IIW 41 with a production-ready version of this same app.

## Session 5B: Introduction to DIF and SSI
_Kim Hamilton Duffy, DIF_

_(No notes taken; Kim will publish slides soon.)_

# Wednesday Sessions

## Session 6A: Identity in Digital Media
_Eric Scouten, Adobe_

### Part 1: C2PA and CAWG Overview

Discussion followed [my slide deck (PDF)](./06a-cawg-update-for-iiw40.pdf).

### Part 2: What's Next?

_(Thank you to Luke Nispel of [OriginVault](https://www.originvault.io) for notes.)_

* Overview of who's who
  * CAI - outreach, advocacy, open source
  * C2PA - technical standards
  * CAWG - identity standards
* C2PA data model
  * Overview of the assets and supported assets
  * Assets manifest store overview and its similarity to github
  * Overview of assertions
  * Each manifest has one claim
  * Claim signature is the signed claim
* Question about security of signing plus buggy systems that can be compromised.
  * Scott is leading the trust governance model for the C2PA to talk about how implementation environments can be trusted.
* Created assertions vs gathered assertions
* What does CAWG do?
  * Technical standards include
    * Endorsment
    * Identity
    * Metadata
    * AI Training and Data mining
* Identity Assertion overview
  * Which signatures should we include in the spec
  * What does identity mean to content creators
  * Claims Aggregator overview
* Are we connecting the dots?
* Most people do not have access or understanding to these technologies
* Example of a need is SAAG actors wanting to have auditions tagged with their identity at time of submission
* Levels of assurance vary and need definition by the industry
* Attestation for creation of physical objects was posited as a future use case
* Interest in licensing and IP protection at time of publish
* CR logo needs to be in Unicode to make it interoperable
* What if creators do not want to be tracked but still want to use the framework?
* Is there a trust score mechanism?
* Museums may value physical assentation as a use case for it

## Session 7F: C2PA Digital Trust Infrastructure
_Scott Perry, Digital Governance Institute_

_(Notes and slide deck to follow.)_

## Session 8E: Identity Hooks in C2PA Credentials: Privacy-Preserving Identity Bindings for Digital Content
_Andrew Dworschack, Yakoa_

Lively discussion about potential credentials to be used for CAWG identity assertion. Sadly, no notes taken.

## Session 10J: Content Authenticity: Physics Forums
_Ben Curtis, JLINC_

Interested in how content provenance could apply to text/HTML content.

Anti-pattern: [Physics forum alleged to have generated posts on behalf of long-dormant users](https://hallofdreams.org/posts/physicsforums/).

JLINC has prototyped a system to use DIDs to authenticate text content with potential for capability delegation. (In other words, authorize a system to post on your behalf.)

What's the smallest possible shortcode that could serve as a pointer to more detailed signature/credential information?

Decentralized method for storing signature using shortcode embedded in plain text.
