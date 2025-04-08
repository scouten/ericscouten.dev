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
