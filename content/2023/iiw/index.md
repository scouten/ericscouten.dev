+++
title = "Internet Identity Workshop 37"
date = 2023-10-10
+++

This week I'm attending the 37th biannual **[Internet Identity Workshop](https://internetidentityworkshop.com)**, in which a few dozen of the world's leading experts on digital identity and credentials gather and a couple hundred more of us do our best to keep up and learn from them.

<!-- more -->

In my work at [Adobe](https://adobe.com) I help define and implement the **[Content Authencity Initiative](https://contentauthenticity.org).** CAI defines itself as:

> ... a community of media and tech companies, NGOs, academics, and others working to promote adoption of an open industry standard for content authenticity and provenance. 

We are particularly interested enabling content creators to identify themselves as the creators of their content and credibly refute false claims of authorship on their behalf, which is why I am attending this conference for the third time. This is my first time attempting to describe it in real time as the conference proceeds.

## The Venue

IIW is held at the lovely **[Computer History Museum](https://computerhistory.org/)**, which recounts the formative years of our tech industry. CHM is located in Mountain View, California, right in the heart of Silicon Valley.

I'll share a few photos of the venue and the conference. My non-technical friends might want to bow out after this section as it will rapidly descend into lots of deep geek speak.

{{ es_image(id = "es-4579-003") }}

{{ es_image(id = "es-4579-005") }}

{{ es_image(id = "es-4579-007") }}

## The Format

IIW is conducted as an **"[unconference](https://en.wikipedia.org/wiki/Unconference),"** which means that there is a pre-defined _structure_ to the conference, but not a predefined _agenda._

There are several variations on how the agenda gets built at an unconference. In IIW's case, there is an opening meeting on each morning in which people stand up and describe sessions they'd like to lead that day. Then there's a mad rush to schedule these sessions (see photo below) and we all choose, in the moment, which sessions to attend.

{{ es_image(id = "es-4579-010", caption = "An as-yet empty schedule board.") }}

{{ es_image(id = "es-4579-011", caption = "Opening discussion before agenda creation.") }}

{{ es_image(id = "es-4580-004", caption = "Introductions.") }}

{{ es_image(id = "es-4580-007", caption = "Calling sessions.") }}

{{ es_image(id = "es-4580-011", caption = "Sessions in the first block.") }}

You might think that not having a predefined agenda would mean that the topics that occur could be flimsy or weak or low in value. In practice, the opposite is true. Both times I've attended this conference so far, I've had to make very difficult choices about which sessions _not_ to attend so I could attend something else which was _also_ very compelling.

Last time (in April), I managed to schedule a weekend to myself [disappearing on the Mendocino coast](https://ericscouten.travel/2023/04-18+california/35-36-on-california-coast/) to decompress afterward. For those of us who are introverts, I highly recommend scheduling some kind of downtime like this afterward. (I talked to almost nobody for four days after IIW and it was _perfect._) This time, I'm headed home for some important family time, so no decompression buffer.

And, with that, here is my description of the sessions I'm attending this time around:

## Session 1L: vLEI updates _(check title)_

_Karla McKenna, Head of Standards and Managing Director of [GLEIF Americas](https://www.gleif.org/en)_

{{ es_image(id = "es-4580-012") }}

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

{{ es_image(id = "es-4580-014") }}

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

Changing the narrative to "organizational identity." Moving from technical capabilities to creating verifiable proof that Person X is a legal representative of Organization Y. _(Add link to Tim's article.)_

Telecomm businesses approaching Provenant and other QVIs to prove authority to communicate on behalf of organization.

Example: If you are running a text messaging campaign, your organization has to be vetted for authority and quality of message. Important in this case to know who are the _people_ that are going to be asking for privileges to execute that campaign. This gets increasingly interesting as tasks such as this get delegated _across companies._ (Consider a major brand hiring a third company to execute the text messaging campaign on their behalf. How does the telco know whether to accept those messages as accurately representing the original brand?)

### Competing Sessions

As mentioned in the intro, IIW almost always presents difficult choices about which sessions to attend. I look forward to reading the notes from these sessions which competed with this one:

* 1D: If DID is so great, why don't I have one yet?
* 1I: Linked Claims: Binding credentials together with cryptographic hashlinks. Giving structure to Verifiable Credential sets

## More Sessions to Follow ...

_(I'll continue to add notes as I attend more session)_

## Resources I've Learned About

* [KERISSE.org](https://kerisse.org): A search engine specifically for KERI topics