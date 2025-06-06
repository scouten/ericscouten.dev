+++
title = "Internet Identity Workshop 37"
date = 2023-10-10

[extra]
cover = "es-4579-005"
cover_cdn_key = "img/v1/2023/10/es-4579-005"
toc = true
+++

This week I'm attending the 37th biannual **[Internet Identity Workshop](https://internetidentityworkshop.com)**, in which a few dozen of the world's leading experts on digital identity and credentials gather and a couple hundred more of us do our best to keep up and learn from them.

<!-- more -->

# Why I'm Here

In my work at [Adobe](https://adobe.com) I help define and implement the **[Content Authencity Initiative](https://contentauthenticity.org).** CAI defines itself as:

> ... a community of media and tech companies, NGOs, academics, and others working to promote adoption of an open industry standard for content authenticity and provenance. 

We are particularly interested in enabling content creators to identify themselves as the creators of their content and credibly refute false claims of authorship on their behalf, which is why I am attending this conference for the third time. This is my first time attempting to describe it in real time as the conference proceeds.

# The Venue

IIW is held at the lovely **[Computer History Museum](https://computerhistory.org/)**, which recounts the formative years of our tech industry. CHM is located in Mountain View, California, right in the heart of Silicon Valley.

I'll share a few photos of the venue and the conference. My non-technical friends might want to bow out after this section as it will rapidly descend into lots of deep geek speak.

{{ es_cdn_image(id = "es-4579-003", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4579-003") }}

{{ es_cdn_image(id = "es-4579-005", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4579-005") }}

{{ es_cdn_image(id = "es-4579-007", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4579-007") }}

# The Format

IIW is conducted as an **"[unconference](https://en.wikipedia.org/wiki/Unconference),"** which means that there is a pre-defined _structure_ to the conference, but not a predefined _agenda._

There are several variations on how the agenda gets built at an unconference. In IIW's case, there is an opening meeting on each morning in which people stand up and describe sessions they'd like to lead that day. Then there's a mad rush to schedule these sessions (see photo below) and we all choose, in the moment, which sessions to attend.

{{ es_cdn_image(id = "es-4579-010", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4579-010", caption = "An as-yet empty schedule board.") }}

{{ es_cdn_image(id = "es-4579-011", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4579-011", caption = "Opening discussion before agenda creation.") }}

{{ es_cdn_image(id = "es-4580-004", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4580-004", caption = "Introductions.") }}

{{ es_cdn_image(id = "es-4580-007", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4580-007", caption = "Calling sessions.") }}

{{ es_cdn_image(id = "es-4580-011", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4580-011", caption = "Sessions in the first block.") }}

You might think that not having a predefined agenda would mean that the topics that occur could be flimsy or weak or low in value. In practice, the opposite is true. Both times I've attended this conference so far, I've had to make very difficult choices about which sessions _not_ to attend so I could attend something else which was _also_ very compelling.

Last time (in April), I managed to schedule a weekend to myself [disappearing on the Mendocino coast](https://ericscouten.travel/2023/04-18+california/35-36-on-california-coast/) to decompress afterward. For those of us who are introverts, I highly recommend scheduling some kind of downtime like this afterward. (I talked to almost nobody for four days after IIW and it was _perfect._) This time, I'm headed home for some important family time, so no decompression buffer.

And, with that, here is my description of the sessions I'm attending this time around:

# Tuesday Sessions

## Session 1L: vLEI Developments and Updates

_Karla McKenna, Head of Standards and Managing Director of [GLEIF Americas](https://www.gleif.org/en)_

{{ es_cdn_image(id = "es-4580-012", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4580-012") }}

Vendors moving through vLEI qualification program: roughly 8 vendors in progress now.

### SDK Update

SDK in progress. Release candidate will be shown during demo hour. SDK includes:

* Identifier management
* Custodial wallet hosting for vLEI issuers
* vLEI credential management
* vLEI credential issuance
* _(upcoming)_ Python client back end
* _(upcoming)_ Mobile wallet
* _(upcoming)_ Structured official organizational roles in vLEIs

OORs (Official Organizational Roles) added in June 2023, lists 2000+ distinct kinds of official roles that are known to the varying forms of legal entities across 89 jurisdictions. (See photo below.)

{{ es_cdn_image(id = "es-4580-014", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4580-014") }}

vLEI adding support for `did:webs` method.

### Standards Update

KERI, ACDC, CESR officially moved to ToIP Foundation. GLEIF is driving standardization for this tech through W3C Verifiable Credentials working group.

### Adoption

QVIs have to disclose rate of issuance. It's early days overall in vLEIs, but some sectors (notably telecommunication) "reaching critical mass." Still working on issuing at scale.

Selling point is international verifiability.

### Regulatory Adoption?

GLEIF under regulatory oversight since formation. Roughly 70 global regulators, largely in financial sector because that was the reason for creation.

GLEIF looking at vLEI as a method for enhancing adoption of LEI. Private sector reporting to public sector is a huge use case.

[European Banking regulator (EBA)](https://www.eba.europa.eu/), which regulates several thousand banks in the EU, did proof-of-concept with vLEI for signature and EBA verified those signatures. Initial indications about this are very promising.

### Messaging Shift: Embracing Organizational Identity

Changing the narrative to "organizational identity." Moving from technical capabilities to creating verifiable proof that Person X is a legal representative of Organization Y. Timothy Ruff wrote about this earlier this year: **[The Dawn of Organizational Identity, Part 1: Identifiers](https://rufftimo.medium.com/the-dawn-of-decentralized-organizational-identity-part-1-identifiers-ffb9091fd47a)** and **[The Dawn of Organizational Identity, Part 2: Credentials](https://rufftimo.medium.com/the-dawn-of-decentralized-organizational-identity-part-2-organizational-credentials-d8baf5fd9114)**.

Telecomm businesses approaching Provenant and other QVIs to prove authority to communicate on behalf of organization.

Example: If you are running a text messaging campaign, your organization has to be vetted for authority and quality of message. Important in this case to know who are the _people_ that are going to be asking for privileges to execute that campaign. This gets increasingly interesting as tasks such as this get delegated _across companies._ (Consider a major brand hiring a third company to execute the text messaging campaign on their behalf. How does the telco know whether to accept those messages as accurately representing the original brand?)

### Slides

* **[Karla McKenna: verifiable LEI (vLEI) Update](https://github.com/WebOfTrust/IIW37/blob/main/2023-10-10_vLEI-Update-IIW37-October_v1.0_final.pdf)** (PDF)

### Competing Sessions

As mentioned in the intro, IIW almost always presents difficult choices about which sessions to attend. I look forward to reading the notes from these sessions which competed with this one:

* 1D: If DID is so great, why don't I have one yet?
* 1I: Linked Claims: Binding credentials together with cryptographic hashlinks. Giving structure to Verifiable Credential sets

## Session 2M: Answers to "The Four Horsemen of SSI"

_Timothy Ruff, GP, Digital Trust Ventures_

{{ es_cdn_image(id = "es-4581-003", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4581-003") }}

Timothy starts by replaying [_The Four Horsemen of SSI_ from Identiverse 2023](https://pages.scmagazine.com/rs/188-UNZ-660/images/Identiverse%202023%20-%20The%20Four%20Horsemen%20of%20the%20SSI%20Apocalypse%20-%205.31.pdf) by Jeremy Grant.

The key points of Grant's presentation:

1. Key management sucks
2. What are the validated attributes?
3. Privacy is oversold
4. Why do I need a coin?
5. (bonus) Choice!

Let's not build identity for the 1%.

### Timothy's Refutation of Point 1: Key management sucks

Question: How many of you use a password manager? (Most hands went up.)

Password management _onboarding_ is awful. Once you're there, there's no going back!

Hmmm ... managing passwords is much like managing keys. Once you turn it over to trusted software, password vs key is not that different. You can manage thousands of keys this way.

### Timothy's Refutation of Point 2: Where are the validated attributes?

Ummm ... there **are** authoritative sources participating in SSI space. _(Looks around room ...)_

### Timothy's Refutation of Point 3: Privacy is oversold

Timothy sort of agrees with this but shifts the thinking here.

Once you've shared information, it's shared. There's no unsharing.

There are lots of unintentional and non-consensual data leaks (face-recognizing cameras, using credit cards for purchases, etc.).

Huh. Interesting take: Stop trying to _conceal_ data. Stop worrying about PII. Corraling data back is a lost cause. It's too easy to re-identify data sets that have supposedly been anonymized by correlated with other data.

Legal mechanism for preventing info sharing of this sort is a non-disclosure agreement. Those are very heavyweight.

What if ... NDAs were streamlined, digital, and digitally signed _before_ data was disclosed?

Now we're enforcing limited data sharing by legal terms, not technical. Something like this is built into KERI stack via ACDCs.

Timothy: "Privacy is dead. Long live confidentiality."

### Timothy's Refutation of Point 4: Why do I need a coin?

You don't.

### Timothy's Refutation of Point 5: (bonus) Choice!

This is actually valid. Defaults win.

### Slides

* **[Timothy Ruff: Answers to ... "The Four Horsemen of the SSI Apocalypse"](./02m-truff-answers-to-four-horsemen.pdf)** (PDF)

### Competing Sessions

* 2L: DIDComm 101 & Q/A

## Lunch

The meals at IIW are surprisingly good for conference food.

{{ es_cdn_image(id = "es-4582-001", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4582-001", caption = "Buffet line.") }}

## Session 3A: OpenWallet Foundation 

* Tracy Kuhrt, TAC chair, OWF
* Daniel Bachenheimer, Unique Identity Services Global Lead, Accenture
* Kaliya Young, consultant to OWF
* Lucy Yang, consultant to OWF

{{ es_cdn_image(id = "es-4582-003", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4582-003") }}

Wallets are critically important.

Speaker was in China recently and couldn't pay for food without Chinese wallet app.

OWF is _not_ about creating standards. Building upon standards built by Open ID Foundation, FIDO, etc.

OWF advocates for open-source software to build wallets for cost, time, and security, and interoperability reasons.

In April, OWF had 26 corporate members and no code. Today, 52 members including Google and Microsoft. Now have a lot of code.

OWF seeking members to join technical community. Slides will be made public.

Google proposing to contribute Android Identity Library to OWF.

Agenda shifted to what can you contribute to OWF, which isn't particularly relevant for me. I departed at this point.

## Session 4E: How Are You Solving for the UX Challenges of SSI?

Open discussion about UX challenges in SSI.

{{ es_cdn_image(id = "es-4583-004", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4583-004") }}

Issues raised:

* Onboarding and education
* Balance between security and ease of use

Moderator Q: Who has solved a serious UX challenge already? 

One answer: "If you get the UX right for a new technology, it will not be adopted." Hmmm.

Sukhi Chuhan (Senior UX Designer at Ontario government): Expectation is that VCs for end users needs to be about ease of use. Make it more and more like what you can do with physical IDs.

If you're creating a new digital wallet product, you are competing with free and built-in from Apple and Google.

Terminology has a big impact. Example: "biometric authentication" scares users, but "Touch ID" and "Face ID" don't.

Remember accessibility. For example, people with impaired vision can't really use QR codes. Also, some people with disabilities and also children may have caregivers or guardians who need to be able to act on their behalf.

Most users will pick utility over sovereignty any day.

Some resistance to using platform-provided wallets due to perception of security concerns and hackability.

Audience Q: How do you present VCs in a way that's digestible?

BC wallet specifically avoids showing information on screen. They want to force the info to be transmitted digitally and displayed on the _verifier's_ device, not the holder's device. On-screen display is easily faked by the credential holder.

### Competing Sessions

* 4C: Credential vs wallet selection
* 4F: SOLID

## Session 5A: Trust Spanning Protocol for Muggles

* Drummond Reed, Steering Committee member of the ToIP Foundation
* Wenjing Chu, Steering Committee member of the ToIP Foundation
* Sam Smith, Creator of KERI

As is so often the case, this was one of the best-attended sessions at IIW.

{{ es_cdn_image(id = "es-4584-004", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4584-004") }}

{{ es_cdn_image(id = "es-4585-001", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4585-001") }}

Recap of this blog post from ToIP: **[Mid-year Progress Report on the ToIP Trust Spanning Protocol](https://trustoverip.org/blog/2023/08/31/mid-year-progress-report-on-the-toip-trust-spanning-protocol/)**.

Seven pillars of trust spanning protocol:

### 1. Verifiable Identifiers

Believe the trust layer for the Internet will require a new spanning layer, akin to IP for traffic itself. Requires a new form of address, which they call Verifiable Identifier. These are commonly DIDs, but not necessarily.

VIDs can also incorporate centralized identifiers. For example, HTTPS address or X.509.

A ToIP identifier _must_ be cryptographically bound to private keys and discoverable.

### 2. End-to-end authenticity and confidentiality

Talking about **[ESSR (Encrypt Sender’s key then Sign Receiver’s key) pattern](https://eprint.iacr.org/2001/079)**. That is a 50-page white paper; it's well summarized in this blog post by Neil Madden: **[Public key authenticated encryption and why you want it (Part II)](https://neilmadden.blog/2018/11/26/public-key-authenticated-encryption-and-why-you-want-it-part-ii/)**.

ESSR allows you to build from zero trust to verifiably authentic with an option to add encryption.

### 3. Direct connections (inner and outer channels)

Remember that privacy has two aspects:

If I trust you (by sending you data that you can decrypt), there's little I can do _technically_ to prevent you from misusing that data. Legal and contractual obligations are more relevant here.

But ... we _can_ prevent third parties who don't have the right keys from spying on the data or even breaching "correlation privacy" which establishes a pattern of communication between two parties.

Every ToIP connection provides at least _partial_ correlation privacy.

### 4. Routing via intermediaries

Using intermediaries allows full correlation privacy. From a protocol design standpoint, it requires one more level of nesting. But no further "onion" style routing is required.

### 5. Relationship context channels

Nested channels also allows you to create an unlimited number of communication _contexts_ between patterns.

### 6. Serialization

ToIP wound up choosing **[CESR](https://github.com/SmithSamuelM/Papers/blob/master/presentations/CESR_Overview.web.pdf)**.

Basic idea was not to fight the protocol war between text and binary representations. CESR allows you to switch back and forth in composable and predictable fashion _without invalidating the signature._

### 7. Trust task protocol framework

All three of the VID-to-VID protocols (DIDComm, KERI, and DWN) include frameworks to support higher-level protocols designed to accomplish specific trust tasks.

Examples of trust tasks are: 

* discovery
* error handling
* trust ping
* logging/auditing

Those trust tasks (layer 3 of the ToIP stack) enable an infinite set of applications on top of that (layer 4 of the ToIP stack).

{{ es_cdn_image(id = "es-4586-002", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4586-002") }}

# Wednesday Sessions

## Session 6C: People Don't Want a Digital Identity; They Want ...

{{ es_cdn_image(id = "es-4587-006", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4587-006") }}

Open discussion led by Adrian Gropper (the volunteer CTO of the non-profit Patient Privacy Rights Foundation). What do people want instead of digital identity?

* address (email, phone, etc. -- how can we improve on that?)
* reputation
* credential (vaccination card, drivers license, proof of age)
* anonymity (activists, citizen journalists)
* freedom of association and assembly
* to be left alone
* user experience / digital convenience

Representative from [Guardian Project](https://guardianproject.info): How do you have continuity and yet anonymity?

Usability and perceived security risk again is a topic.

California's digital ID is dual-format (mDL and VC). Proof of age via VC. Look at TruAge, about to be integrated with point-of-sale systems, supported by age-restricted goods industries.

### Competing Sessions

* 6F: GLEIF's Experience with the vLEI. Ecosystem Governance Framework: Lessons Learned _(seems similar to [yesterday's GLEIF session](https://ericscouten.dev/2023/iiw/#session-1l-vlei-developments-and-updates))_
* 6K: Dying with Dignity: A consent-driven dead man's switch for online services

## Demos

* Provenant: automated process for vLEI issuance

## Session 9H: Secure Organizational Identity

* Lance Byrd, software developer, GLEIF
* Alex Andrei, GLEIF
* Rodolfo Miranda, GLEIF

Organizational identity is nuanced and complex. Contractors, employees, vendors ... all of these relationships require verification, trust, audit trails.

Many organizational identity considerations:

{{ es_cdn_image(id = "es-4589-001", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4589-001") }}

Organizations have a high stake in their identity. Can not trade-off security with anything else.

Lifetime of identifiers is critical.

**NEW:** Securing keys at the edge (KATE). HSMs and/or local biometrics control access to keys. Using multi-sig gives you ability to recover access to personal AID.

New "signify" codebase helps with signing at the edge. Key event generation and signing, among other tasks.

{{ es_cdn_image(id = "es-4590-001", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4590-001") }}

{{ es_cdn_image(id = "es-4590-004", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4590-004") }}

Audience Q: How much do witnesses cost? How do you find them?

A: Early days. Right now it's the early adopters. Expect this to be commoditized. "We anticipate that there will be witness services." Those are likely to be free for low/normal volume situations. If signing millions per month, then cost may need to be passed along.

ACDC means that vLEI credentials are chainable, end verifiable, attestable organizational credentials. Chainable means orgs can issue credentails for anyone from C-suite to individual employees.

IPEX (VC issuance and presentation exchanges). Exchanging of chained credentails facilitates legally-binding agreements and contractually-protected disclosures.

### Competing Sessions

* 9G: Should governments be involved in VC system?
* 9M: IEEE 7012, Personal terms and conditions

## Session 10C: Fitting credentials that are verifiable into NIST's digital identity guidelines

* Justin Richer, independent identity consultant

I came in late. Justin was giving some background explanation of [NIST SP 800-63-4 "Digital Identity Guidelines,"](https://csrc.nist.gov/pubs/sp/800/63/4/ipd) which is currently in "initial public draft" stage.

{{ es_cdn_image(id = "es-4591-006", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4591-006") }}

He was explaining subject -> CSP (Credential Service Provider) -> IDP (ID Provider) -> relying party interaction in NIST terms.

"IDP is played by the wallet. This is where things start to go funny."

NIST uses different terminology from SSI/VC community. Approximate translations of a few common terms:

* (NIST) Subject -> (SSI) Holder
* (NIST) CSP -> (SSI) Issuer
* (NIST) IDP -> (SSI) Wallet
* (NIST) RP -> (SSI) Verifier
* (NIST) Assertion -> (SSI) Presentation

I'm a bit out of my element here because my work doesn't particularly overlap with NIST (or at least hasn't so far), so it's mostly interesting to see how things map from one world to another.

# Thursday Sessions

{{ es_cdn_image(id = "es-4592-007", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4592-007", caption = "Taking photos of the schedule board before the first session of the morning.") }}

## Session 11B: Selective Disclosure is Useless: We Have Receipts

* Timothy Ruff
* Sam Smith

{{ es_cdn_image(id = "es-4592-008", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4592-008") }}

Define **ephemeral privacy:** Privacy "exists" but is easily undone because "de-anonymized" data is easily re-correlated.

It's effectively trivial to re-identity individuals from de-anonymized data sets.

Define **privacy washing:** De-anonymize data to the point where it can legally be re-shared. But ... there are holes. You may have intentionally or unintentionally left hooks for yourself or others to re-correlate and re-identity individuals in that data set.

Timothy argues that ZKPs and AnonCreds (which his team helped develop) are no longer useful. So easily defeated as to be not worth the effort.

"We aren't saying privacy is dead. We believe the future is confidentiality ..." using legal tools rather than technical tools.

Privacy through obscurity is no longer worth it.

New focus: Make legally-binding personal terms and conditions easily exchanged.

Joyce Searls points toward [IEEE standard P7012](https://standards.ieee.org/ieee/7012/7192/) which is a way that individuals can exchange terms. Timothy: "It is exactly that." ACDCs enable that technically.

Sam Smith: "People are falsely believing that they have a false sense of security with selective disclosure." This is no longer true.

Description of how little info it takes to re-identify data.

Privacy washing exists because the legal frameworks are years behind the technology.

FTC issued a report last year that says k-anonymity is no longer sufficient for privacy. Example given of how cell-phone location data can be used for re-identification. Another example: social graphs could be reconstructed via the so-called anonymous identifiers in Covid contact tracing apps we had a year or two ago.

Anyone sophisticated enough to verify a ZKP is almost certainly sophisticated enough to perform a re-identification attack.

### Proposed Solution

ACDCs have the ability to support contractually-protected disclosure. This is the technical part that enables a quick and frictionless agreement of terms. The mechanics are there to do this. Now need policy that follows that.

Daniel Hardman isn't present, but it sounds like his work in the earlier-mentioned IEEE standard builds upon this.

Timothy Ruff: "Timing is everything. I think there is a hunger for privacy like the world has never seen. So our timing is good to introduce these things to the world." And tech is converging around this.

Audience Q: Is this a US problem or a worldwide problem? Audience answer: Same issue (resale and re-correlation of private data) exists worldwide, only varying by degree country to country and even state to state within the US (e.g. CCPA in California).

### Competing Sessions

* 11A: Stitching together a wallet: What's there, what's missing
* 11G: Bubbles? Federation in disadvantaged and disconnected environments

## Session 13C: What does Presentation Exchange do and what parts of it do we actually need?

* Mike Jones, independent consultant in digital identity, security, and interoperability

Presentation Exchange can do a lot of different things.

* OpenID for VPs
* High Assurance 

Starts by summarizing content posted at [What does Presentation Exchange do and what parts of it do we actually need?](https://self-issued.info/?p=2395) on Mike's blog, [Mike Jones: self-issued](https://self-issued.info/).

Much active discussion about combining credentials issued from different sources (e.g. university degree + drivers license + professional license).

## Session 15A: ToIP SSI Glossary

* Drummond Reed, Steering Committee member of the ToIP Foundation
* Brian Richter, member of Concept and Terminology Working Group, ToIP

{{ es_cdn_image(id = "es-4593-009", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4593-009") }}

I came in late. Drummond was walking through some existing SSI glossaries that already existed and why ToIP is building its own.

On [eSSIF-Lab Glossary](https://essif-lab.github.io/framework/docs/essifLab-glossary) (EU funded), they also have a mental models section.

Glossary is currently available as an early draft on [Google Docs](https://docs.google.com/document/d/1fZByfuSOwszDRkE7ARQLeElSYmVznoOyJK4sxRvJpyM). Sounds like they will migrate it to MediaWiki or similar later this year.

Brian Richter did a [bunch of tooling](https://github.com/aviarytech/tev2-ingress) to make this feasible and to assist in the translation from GitHub wikis to Google Docs. Looks like a tremendous amount of work done to make editing and viewing accessible to people who do and do not prefer working with GitHub.

{{ es_cdn_image(id = "es-4594-002", cdn_version = "v1", cdn_key = "img/v1/2023/10/es-4594-002") }}

# Important Learning: Verifiable Identifiers

Just a week or so ago, I first heard the term "**verifiable identifier**" when Drummond Reed appeared on [episode #60 - Trust Spanning Protocol: Seven Key Pillars](https://overcast.fm/+pswpLY518) of Matthieu Glaude's excellent [_SSI Orbit_ podcast](https://northernblock.io/podcasts/).

This is described in the **[ToIP Technology Architecture Specification](https://github.com/trustoverip/TechArch/blob/main/spec.md#trust-over-ip-toip-technology-architecture-specification)** in section 6.4 titled **[ToIP Identifiers](https://github.com/trustoverip/TechArch/blob/main/spec.md#trust-over-ip-toip-technology-architecture-specification)**. I'm happy to hear that ToIP is recognizing that there's value in identifiers that can be independently verifiable, regardless of how they are issued (i.e. in a decentralized or centralized fashion).

It looks like this is currently a _conceptual unification_ between DIDs and centralized identifiers (X.509 and similar) and not yet a _technical spec_ that describes a protocol format that allows you to express "DID or X.509 or ..." but that this is an area of active interest from ToIP.

# Conference Proceedings

Full proceedings from the conference are typically available a few weeks afterward. I'll add a link when that becomes available.

# Resources I've Learned About

* [KERISSE.org](https://kerisse.org): A search engine specifically for KERI topics
