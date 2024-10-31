+++
title = "Internet Identity Workshop 39"
date = 2024-10-29

[extra]
toc = true
+++

This week I'm attending the 39th biannual **[Internet Identity Workshop](https://internetidentityworkshop.com),** which is one of the most valuable conferences I've encountered in any professional space. As the name might suggest, the topics are largely around how to express human and organizational identity in digital terms that respect privacy and security.

<!-- more -->

# Why Am I Here?

I'm part of a team at [Adobe](https://adobe.com) that is dedicated to helping content creators and content consumers establish genuine connections with each other. We do this through three organizations that we've helped to create:

* **[Content Authenticity Initiative](https://contentauthenticity.org):** CAI is a community of media and tech companies, NGOs, academics, and others working to promote adoption of an open industry standard for content authenticity and provenance. The CAI does outreach, advocacy, and education around these open standards. Content Authenticity Initiative is also the name of the business unit of which I'm a part at Adobe through which we participate in all three of these organizations, develop open source and open standards, and guide implementation within Adobe's product and service suite.

* **[Coalition for Content Provenance and Authenticity](https://c2pa.org):** C2PA is a technical standards organization which addresses the prevalence of misleading information online through the development of technical standards for certifying the source and history (or provenance) of media content.

* **[Creator Assertions Working Group](https://creator-assertions.github.io):** CAWG builds upon the work of the C2PA by defining additional assertions that allow content creators to express individual and organizational identity and intent about their content.

This spring, I published an article titled **[Content Authenticity 101](/2024/content-authenticity-101.md),** which explains these organizations and our motivations in more detail.

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

## Session 1L: Personhood, the Killer Credential -- Killer Credential Network Effects

* Drummond Reed, GEN, ToIP, GAN governance workstream
* Andor Kesselman, DIF, ToIP, GAN tech workstream
* Dave Poltorak, GAN tech workstream
* Andre Kudra, Esatus

Three "killer" credentials in the digital world:

* passport
* drivers' license
* credit card

They work because there are _ecosystems_ of issuers. Trust is in the _ecosystem,_ not just the issuer.

This work because there's an agreement amongst issuers on what the issuing conditions are.

Drummond: "If we want to have breakthrough in this industry that we've been creating these past 20 years, premise number 1: They need to be multi-issuer credentials. Premise number 2: We're going to need governance."

That is the fundamental premise behind the [Global Acceptance Network](https://gan.foundation).

This is a business session; technical parts will be in Session 5 today.

Point to blog post by Eve Maler, _[Personhood: The Killer Credential?](https://www.vennfactory.com/blog-post/personhood-the-killer-credential)._

GAN brings the core infrastructure to make that work.

GAN position: personhood credential is good, but there are at least two others. Also looking at known customer and known employee. Unified employee badge.

Feel that this is useful from the start.

GAN wants to be in the sweet spot of business, not government credentials. Looking at B2B and B2C credentials. That leaves them flexible to work with lower (LOA) levels of assurance.

Will be talking later at IIW about the "ecosystem of ecosystems model." One of the key principles is that each ecosystem is self-sovereign. The purpose of the GAN is to address the problem of cross-ecosystem trust interoperability.

Business model: Can you monetize your credentials? But that, of course, means that I have to have a model to trust another ecosystems.

Andre: We don't want to have fifty different "killer credentials." Just a very few.

Observation from Bhutan, where they are leading with a national digital ID system based on SSI. Most valuable credential currently on offer is verified phone number.

Risk raised by audience member: Could known-customer credential be over-used / abused?

GAN principle: The more sensitive the data, the more important it is that you verify the verifier.

Goal of the GAN is not to create new standards, but rather to create the venue for collaborating to establish trust across ecosystems.

## Session 2F: Privacy Concerns Around the mDL
_Timothy Ruff and Phil Windley_

Follow up to [Timothy's LinkedIn post](https://www.linkedin.com/posts/rufftim_aclu-digital-id-state-legislative-recommendations-activity-7250510391376551937-SWPf/) based on [ACLU's digital ID state legislative recommendations](https://www.aclu.org/documents/aclu-digital-id-state-legislative-recommendations).

Timothy starts from ACLU state legislative reocmmendations, issued October 2024.

Timothy's concerns center around (1) handing unlocked phone to police officer, and (2) issuer ability to track users via "phone home" mechanisms.

mDL works via device engagement. This is what's happening either via QR code or NFC.

Digital identity is thus far siloed by B2C interaction. Government getting into the game represents a likely consolidation of identity issuance. If government gets into digital identity, life will get likely get worse.

"My dream of self-sovereign identity can turn into a nightmare of government surveillance" ... if we don't exercise care _now_ about how digital credentials are issued and used.

Audience Q: What is the counter-incentive that we can present to discourage surveillance? Timothy will present something tomorrow as a potential model.

Fear: Governments exempt themselves from data privacy regulations. Rare, if ever, that the capability to collect data rolls back.

# Wednesday Sessions

## Session 6L: First Person Credentials

Growing concern about overuse of mDLs as credential and privacy concerns related to such. (See Timothy's session yesterday.) Can we find -- and agree to -- a privacy-preserving credential with strong proof of personhood?

Doc Searls wrote an article in 2014 titled [Why we need first person credentials on the Net](https://projectvrm.org/2014/03/19/why-we-need-first-person-technologies-on-the-net/); used as a foundation for this talk.

Kim Duffy gave a quick introduction to the state of ID verification techniques. At the low-end and high-end of ID verification techniques, it's increasingly easy for generative AI to defeat verification techniques. Becoming increasingly urgent to do something new to verify personhood in a more secure method. Pressure will increase to convincingly prove personhood. If we are to avoid overuse (and privacy violations inherent in) of mDLs, the time is now.

See also the [paper from OpenAI and others](https://arxiv.org/html/2408.07892v1) regarding the need for personhood credentials.

Now that you understand the need for personhood credentials and the core of the GAN framework (see yesterday's talk), we'll talk about specific credential types.

How about using people as mutual trust roots?

People commonly exchange credentials using informal means already. Examples: In China, everybody uses WeChat. "Hi, how are you? Here's my QR code." In Bhutan, WhatsApp or LinkedIn. So we already have the ceremony that we need, except that it isn't wallet to wallet.

Whiteboard diagram (I'll add <!-- IMG_2032 --> later) about how to create "verifiable relationship credential" between two people which either can then use to prove to anyone else that the other is a known person.

These identifiers are truly privacy preserving and have _no relation_ to e-mail or phone or other too-well-known identifiers.

Initial discussion was about person-to-person credential, but guess what? It also applies for B2C relationships as well. <!-- IMG_2033 -->

Reputation is built by presenting P2P credentials to a third party (what they call an "oracle server") to aggregate P2P credentials and issue 

See [Greencheck](http://greencheck.world) as an example of "three-friend authentication." (Who knows better than I'm a real person than my friends?)

Interesting: They have validation of claims of social media. Hmmm ...

## Session 7J: Bhutan NDI

_Michael Becker, Drummond Reed_

<!-- Add link to Michael's slide deck. -->

Population 790K, geographically isolate.

First country to launch national SSI infrastructure.

Almost completely digitized currency.

First carbon-negative country in the world.

First country to join GAN.

Bhutan's definition of mindfulness steps beyond "presence" to "compassionate presence" – having compassion for all living beings, born and unborn.

They think of this when talking about modernizing their technological footprint.

Used to take 10 days to create a bank account; now it's 10 seconds via SSI.

140K IDs created in 8 months. 56% of smartphone owners. Working on web wallets and paper QR code wallets for those without smartphone access.

Can integrate new private partners in less than a month. Very strict data minimization rules. Criminal penalties (jail time) for using data beyond authorized scope.

Now working on launching same tech in other countries, especially less-developed countries. (Papua New Guinea launching now; working on Uganda.) Recouping Bhutan's cost by exporting/selling the tech to other countries.

What Bhutan is doing is uprooting the whole model of ID verification. Once this proliferates as a public good, foundational ID becomes essentially free.

EU is 18-24 months behind Bhutan on this process.

## Session 8C: Dude (Person), Where's Your DID?
_Eric Scouten, Adobe_

I gave a brief overview of the C2PA data model and then explained the CAWG ([Creator Assertions Working Group](https://creator-assertions.github.io/)) framework for allowing content creators to add their own identity attestations to content they create.

The framework roughly translates as: "The actor* described by ${credential} using a credential issued by ${issuer} produced the content described by ${signer_payload}. Signed by: ${credential_holder}." _(*Actor can be human, non-human, or organization of humans.)_

These placeholders can be filled in with different data types depending on the kinds of credentials available to the content creator. We spent most of the discussion talking about the recently-introduced model of **[identity claims aggregation](https://creator-assertions.github.io/identity/1.1-draft/#_identity_claims_aggregation)** which allows a trusted third-party to gather identity claims (proof of control over social media accounts and web sites as common examples) and link them to the content created by the same actor.

Slides here:

![Slides for IIW 39: Dude (Person), Where's Your DID?](./2024-10-30-iiw-dude-wheres-your-did.pdf)

## Session 9E: Originator Profile

_Shigeya Suzuki_

[Originator Profile](https://originator-profile.org/en-US/)

Aimed at providing information about publisher of information, including . Typical emphasis is news media.

OP provides content attestation, common technology, baseline governance model.

Common technology and baseline governance model.

Data model: Using the name "web content authenticity."

Major difference from C2PA data model: Can authenticate web page as a whole, as part of a site, and individual media files.

Originator profile can include contact information.

Currently certificates can only be issued to Originator Profile members. Will be extending to Japanese news media and local Japanese government units.

Status:

* Phase 1 (Early 2025): Limited numer of media outlets
  * Missing features: lacking identity flexibility (key rotation)
* Phase 2 (Spring 2025): Outlet via aggregators and digital advertising
  * Feature complete for static web sites
* Phase 3 (EOY 2025): Local (Japanese) government outlets

Signing per fragment of DOM.

Provides traceability for content, but only for pre-approved publishing sites.

## Session 10H: Sneaking SSI into the Music Industry
_Cole Davis, Switchchord_

Music industry has complex legal relationship between identified parties.

<!-- IMG_2039 -->

Example use case: Using a song in an advertisement. As of 2016, needed to search multiple databases to find all the parties who are owed compensation for that use.

Recording: "That's a recent phenomenon based on technology invented in the early 1900s." But it has a completely separate licensing model from composition.

<!-- IMG_2041 -->

Ownership of rights is often sorted out well _after_ a song is published and/or streamed.

Legal concepts and identity are entangled.

<!-- IMG_2042 -->

<!-- IMG_2044 -->

Switchchord lets people:

* Prove legal relationships
* Let relationships define state of copyright
* Enable data to update downstream databases
