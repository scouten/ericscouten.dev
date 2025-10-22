+++
title = "Internet Identity Workshop 41"
date = 2025-10-21

[extra]
toc = true
+++

This week I'm attending the 41st biannual **[Internet Identity Workshop](https://internetidentityworkshop.com),** which is one of the most valuable conferences I've encountered in any professional space. As the name might suggest, the topics are largely around how to express human and organizational identity in digital terms that respect privacy and security.

<!-- more -->

# Why Am I Here?

I'm part of a team at [Adobe](https://adobe.com) that is dedicated to helping content creators and content consumers establish genuine connections with each other. We do this through three organizations that we've helped to create:

* **[Content Authenticity Initiative](https://contentauthenticity.org):** CAI is a community of media and tech companies, NGOs, academics, and others working to promote adoption of an open industry standard for content authenticity and provenance. The CAI does outreach, advocacy, and education around these open standards. Content Authenticity Initiative is also the name of the business unit of which I'm a part at Adobe through which we participate in all three of these organizations, develop open source and open standards, and guide implementation within Adobe's product and service suite.

* **[Coalition for Content Provenance and Authenticity](https://c2pa.org):** C2PA is a technical standards organization which addresses the prevalence of misleading information online through the development of technical standards for certifying the source and history (or provenance) of media content.

* **[Creator Assertions Working Group](https://cawg.io):** CAWG builds upon the work of the C2PA by defining additional assertions that allow content creators to express individual and organizational identity and intent about their content. CAWG is a working group within the [Decentralized Identity Foundation (DIF)](https://identity.foundation).

Last year, I published an article titled **[Content Authenticity 101](/2024/content-authenticity-101.md),** which explains these organizations and our motivations in more detail.

## The Venue

IIW is held at the lovely **[Computer History Museum](https://computerhistory.org/)**, which recounts the formative years of our tech industry. CHM is located in Mountain View, California, right in the heart of Silicon Valley.

I'll share a few photos of the venue and the conference. My non-technical friends might want to bow out after this section as it will rapidly descend into lots of deep geek speak.

## The Format

IIW is conducted as an **"[unconference](https://en.wikipedia.org/wiki/Unconference),"** which means that there is a pre-defined _structure_ to the conference, but not a predefined _agenda._

There are several variations on how the agenda gets built at an unconference. In IIW's case, there is an opening meeting on each morning in which people stand up and describe sessions they'd like to lead that day. Then there's a mad rush to schedule these sessions (see photo below) and we all choose, in the moment, which sessions to attend.

{{ es_cdn_image(id = "es-25a-7560", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7560", caption = "Computer History Museum, Mountain View, California") }}

{{ es_cdn_image(id = "es-25a-7561", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7561", caption = "Computer History Museum, Mountain View, California") }}

{{ es_cdn_image(id = "es-25a-7563", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7563", caption = "Computer History Museum, Mountain View, California") }}

{{ es_cdn_image(id = "es-25a-7565", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7565", caption = "Computer History Museum, Mountain View, California") }}

{{ es_cdn_image(id = "es-25a-7568", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7568", caption = "An as-yet empty schedule board.") }}

You might think that not having a predefined agenda would mean that the topics that occur could be flimsy or weak or low in value. In practice, the opposite is true. Both times I've attended this conference so far, I've had to make very difficult choices about which sessions _not_ to attend so I could attend something else which was _also_ very compelling.

With that, here is my description of the sessions I'm attending this time around:

# Tuesday Sessions

## Session 1M: First Person Project
_Drummond Reed, [First Person Project](https://www.firstperson.network)_

Reviewing version 1.1 of the [First Person Project White Paper](https://static1.squarespace.com/static/6834ee7c55c6376908871a6d/t/68f6402d873ecc0c40810ded/1760968749978/The+First+Person+Project+White+Paper+V1.1.pdf), just published yesterday. It's 86 pages long. This talk is an overview of the major sections. Since it's in the document, I won't transcribe everything, but will instead focus on some highlights.

There's also a [slide deck](https://docs.google.com/presentation/d/1wz_nVjrHzth_QyYAuDWIf4w5Clg_olXvS-jMiv8GR4c/edit?usp=sharing) if you prefer that format.

Fundamental goal: Establish a person-to-person trust layer for the internet.

Ability to impersonate real people and real situations with current generative AI tools has led to an accelerating degeneration of trust.

An essential part of this is to establish and facilitate person-to-person secure channels.

Reference out to [personhood credentials paper](https://arxiv.org/pdf/2408.07892).

{{ es_cdn_image(id = "es-25a-7575", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7575", caption = "Computer History Museum, Mountain View, California") }}

Talk through how people have multiple personas that they might want to disclose selectively, for example:

* political
* religious
* neighborhood
* work
* medical
* online dating

## Session 2M: The Swiss e-ID / The Failure of Decentralized Identity
_Christopher Allen_

This is a recap of the blog post and slide deck posted by Christopher at [Musings of a Trust Architect: Five Anchors to Preserve Autonomy & Sovereignty](https://www.lifewithalacrity.com/article/musings-swiss-eid/).

A few years ago, Swiss Post Office proposed a digital ID. Referendum voted it down.

Government went back and reworked to address system to address feedback. This passed by a very narrow margin in a recent referendum. Result is based on SSI technology, but is completely government-implemented (i.e. centralized). This system is open in the sense that other information _can_ be attached to government-issued digital identifiers; closed in the sense that only government can issue these credential.

Law _says_ that digital identifiers are **not** required, but Chris is skeptical. The implementation will turn out to make physical identifiers into second-class citizens.

Swiss cultural concerns are largely about how the platform vendors (i.e. Android and iOS) will have an outsized ability to use data obtained through those credentials.

**The TLS warning:** Once you ship something, "good enough" becomes "stuck with it." TLS 1.0 was ratified in 1999 with some known problems. Problems weren't fixed until TLS 1.3 in 2019. (Gulp.)

Love this quote:

> If a system cannot hear you say no, it was never built for **us.** It was built for **them.**

Chris describes this as "the least worst implementation" of a government-backed digital ID system.

Swiss ID system doesn't have a well-established right to refuse participation.

### The Sad State of Decentralized ID

* eIDAS captured by Apple & Google (mDL)
  * Very difficult for smaller orgs to participate in standards organizations. W3C makes it hard; ISO is worse because power is in the governments. ISO pricing is difficult.
  * ISO response to "no phone home" was weak. "Phone home" is optional. But eIDAS requires vendors _to test_ phone home capacity. Ugh.
  * Platform vendors have no fiduciary responsibility for the data contained in wallets.
* US states following suit (it's cheap)
* DHS funding for DID/VC has collapsed
* KYC everywhere but insecure
* Web3/Nostr: progress but no key rotation
* Corporate capture of "decentralized"
  * Example: E-mail, which was originally decentralized -- and still is in theory. In practice, it's impossible for anyone but the Major Players to run an e-mail server.
* Builder's dilemma: pure but irrelevant vs adopted but compromised

So what can we do about it?

* Persuade Switzerland to do the right things during this window after the narrow referendum win.
* Persuade more states to follow Utah's lead.

## Session 3C: Content Authenticity 101
_Eric Scouten, Adobe_

Discussion followed [my slide deck (PDF)](./03c-cawg-c2pa-overview.pdf).

## Session 4I: Scaling the Agentic Web
_Andor Kesselman_

Discussion followed [Andor's slide deck](./04i-andor-scaling-the-agentic-web.pdf).

Started with a history of AI evolution.

Andor expects that thinking of agents as _singular_ agents isn't likely to remain common. Pressures are likely to lead to orchestration of agents working with each other, **but** that comes with increased risk of attack surface and error propagation.

Identity for AI agents is far more complex than human identity. For example: Where is the agent running? What version? What host OS? What compute center? What context did it have? What goals was it given?

Some people are now working on **K**now **Y**our **A**gent (KYA).

{{ es_cdn_image(id = "es-25a-7584", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7584") }}

Interesting question: Does DNS scale up sufficiently for agents, especially given their potentially short lifetimes?

As of yet, MCP servers aren't really talking to each other. That will likely change soon and may substantially increase the attack surface vector.

# Wednesday Sessions

## Session 6K: Driving vLEI and KERI Adoption
_Esteban García and Kent Bull, [GLEIF](https://www.gleif.org/en)_

GLEIF goal: Identity system for organizations at global scale.

To drive adoption, you need a "perfect storm" of things going right. GLEIF sees this as a flywheel building on the following components:
* **Policy:** Policy makers in each jurisdiction that registers legal entities need to be on board.
* **Technology:** vLEI ecosystem depends and adoption/viability of KERI protocol.
* **Market drivers:** ROI or policy requirements that drive adoption.

On technology specifically, GLEIF understands that developers need access to easily-onboarded technology. Focusing on developer-oriented training materials.

Hosting a [global vLEI Hackathon](https://www.gleif.org/en/newsroom/events/gleif-vlei-hackathon-2025). Intent is to promote awareness of the ecosystem and to encourage adoption/integration into existing commercial systems. Hackathon projects address these topics: finance, KYB, and supply chain. Over 100 submissions for initial round. Final presentations in next few weeks.

{{ es_cdn_image(id = "es-25a-7592", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7592") }}

Be aware of [vLEI training materials](https://github.com/GLEIF-IT/vlei-trainings) published by GLEIF.

KeriCON coming up: First KERI-only conference. April 2026 in Salt Lake City, just before IIW. Conference web site not yet available.

I asked a question about the ordering of the layer stack. When I reviewed KERI a couple years ago, I had trouble figuring this out. Kent provided the following sequence (top to bottom):

* TSP from ToIP
* ACDC
* KERI
* CESR (serialization format)
* verifiable data structure (key event log) verifiable key and signing history
* cryptographic primitives (seeds, keys, signatures) and data structure primitives (text, labels, field maps)
* libsodium, crypto key generation, signing, and verification (currently written primarily at C)

Karla extends an open invitation to attend the marketing and outreach sessions hosted by KERI Foundation.

## Session 7C: KERI Plus W3C VC Interoperability
_Kent Bull, GLEIF_

Working update on GLEIF-supported work to turn an ACDC into a W3C VC DM 1.1 or 2.0.

Fundamentally trying to solve the problem of making an ACDC credential resolvable by a client using W3C VC technology who doesn't actually understand any of the KERI stack.

Is it possible to go the other way? tl;dr: No. IOW can a W3C VC be turned into a valid ACDC? No, because KERI has tighter security requirements than W3C. One example is the use of JSON LD contexts, which are vulnerable to schema malleability attacks. KERI doesn't rely on any web infrastructure as part of its security posture.

{{ es_cdn_image(id = "es-25a-7597", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7597") }}

Problem: A lot of the security libraries want access to private key material in order to sign.

Utah mentions that there is also work to make ACDCs available as mDLs as well. Proof of concept demonstration at the SEDI summit last week.

ACDC has introduced a new "cargo" field in the ACDC which represents a signed commitment to a particular serialization of (for example) a W3C VC credential, which then gets placed in the ACDC chain.

## Session 9J: First Person + C2PA Registrar
_Luke Nispel, Origin Vault_

Goal: Creat an endorsement network of artists that recognize each other.

Looking into how to use [First Person](https://firstperson.network) credential, which has verified person infrastructure, to build an identity claims aggregator. Their ICA implementation allows Facebook, GitHub, Adobe, many other verified IDs. Then you can anchor things on the blockchain.

{{ es_cdn_image(id = "es-25a-7602", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7602", caption = "Computer History Museum, Mountain View, California") }}

{{ es_cdn_image(id = "es-25a-7603", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7603", caption = "Computer History Museum, Mountain View, California") }}

Have implemented their own C2PA verifier and signing infrastructure. Content uploaded to their service gets registered on blockchain. Registrar for verified persons on the Cheqd. Each Cheqd DID has a linked resources field which allows linkage to small information. Could point to URLs with additional information or C2PA Manifests hosted outside.

Purpose: Peer-to-peer artist network empowered with C2PA and Cheqd.

{{ es_cdn_image(id = "es-25a-7605", cdn_version = "v1", cdn_key = "img/v1/2025/10/es-25a-7605", caption = "Computer History Museum, Mountain View, California") }}

Interesting business model experiment: Artist can choose to charge the verifier to verify identity through this framework.
