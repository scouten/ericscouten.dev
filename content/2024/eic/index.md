+++
title = "European Identity Conference 2024"
date = 2024-06-04
aliases = ["/2024/eic2024"]

[extra]
bounds = {sw = [52.511, 13.407], ne = [52.531, 13.427]}
markers = "markers.js"
toc = true
+++

This week I'm in Berlin, attending the **[European Identity Conference](https://www.kuppingercole.com/events/eic2024).** When I attended the IIW earlier this spring, [I wrote about it in real time](/2024/iiw38) as the conference was in progress. That format worked well for me and received a lot of compliments, so I'm attempting it again this week.

<!-- more -->

_NOTE: Rather than trying to take comprehensive notes for each presentation, I'll share my own photos and comments that aren't immediately obvious from the slides. The slides for each presentation are generally available if you click the link on the section header._

# Why Am I Here?

I'm part of a team at [Adobe](https://adobe.com) that is dedicated to helping content creators and content consumers establish genuine connections with each other. We do this through three organizations that we've helped to create:

* **[Content Authenticity Initiative](https://contentauthenticity.org):** CAI is a community of media and tech companies, NGOs, academics, and others working to promote adoption of an open industry standard for content authenticity and provenance. The CAI does outreach, advocacy, and education around these open standards. Content Authenticity Initiative is also the name of the business unit of which I'm a part at Adobe through which we participate in all three of these organizations, develop open source and open standards, and guide implementation within Adobe's product and service suite.

* **[Coalition for Content Provenance and Authenticity](https://c2pa.org):** C2PA is a technical standards organization which addresses the prevalence of misleading information online through the development of technical standards for certifying the source and history (or provenance) of media content.

* **[Creator Assertions Working Group](https://creator-assertions.github.io):** CAWG builds upon the work of the C2PA by defining additional assertions that allow content creators to express individual and organizational identity and intent about their content.

I recently published an article titled **[Content Authenticity 101](/2024/content-authenticity-101.md),** which explains these organizations and our motivations in more detail.

# Tuesday Sessions

## [DID - Catching the Wave in Government and Financial Services](https://www.kuppingercole.com/sessions/5481)

Interesting things not directly on slides:

* Bangladesh GDP increased 7% after national digital ID program launched.
* eIDAS 2 _requires_ relying parties above a certain size to accept EU digital credentials.
* Introduced to the concept of "rogue verifiers."
* Interesting that X.509 is the backing architecture for issuer trust registries in the EU trust infrastructure.

## [Defense against Mis/Disinformation Roundtable: Collaboration through Standards](https://www.kuppingercole.com/sessions/5705/1)

_VERY_ full room.

{{ es_image(id = "es-4661-096", caption = "Berlin Congress Center, Berlin, Germany") }}

This session spoke to security and user control of credentials, but did not cover misinformation/disinformation as we think of it in the CAI/C2PA sense. (We think primarily about misrepresenting context, technique, or identity as a way to mislead.)

Content not directly on slides:

* Sam Curren gave a demo of OpenIDIDComm.
  * Value proposition: You can add distributed identity to an existing identity infrastructure.
* [DID method rubric](https://www.w3.org/TR/did-rubric/) -- check link ... is this what Kim was referring to?

## Outside Interlude

A quick view of the Berlin Congress Center as I was walking toward it:

{{ es_image(id = "es-4661-110", caption = "Berlin Congress Center, Berlin, Germany") }}

## [Vision 2030: Rethinking Digital Identity in the Era of AI and Decentralization](https://www.kuppingercole.com/sessions/5486)
_Martin Kuppinger_

(Title tl;dr: Finally solving the IAM puzzle.)

"Will decentrialized ID really be the thing that helps us solve the puzzle?" (Which puzzle.)

Interesting axes: Security/protection vs enablement, technology vs business

I like the term "identity silos." (They won't go away quietly.)

"The risk of siloed wallets."

{{ es_image(id = "es-4662-004", caption = "Berlin Congress Center, Berlin, Germany") }}

A friend who had observed last year's conference was stunned by the sea change in this conference. Last year, decentralized identity and even eIDAS seemed like an afterthought; this year, in the keynote, we were told that it is the next big thing.

Related links:

* [DIF blog: Decentralized ID Technical Mastery Sprint @ EIC](https://blog.identity.foundation/decentralized-id-technical-mastery-sprint-eic/)

## [Protocols, Payloads, Policies, Oh My!: How can Enterprise Customers Make Better Decisions?](https://www.kuppingercole.com/sessions/5487)
_Anil John, US Department of Homeland Security_

"Just like the Trojans, you are going to be getting a lot of gifts."

"The right to paper" as a way of saying digital is not a requirement.

Everybody who is arguing for their standards: "A swirling whirlpool of doom." (Obligatory reference to the XKCD "competing standards" comic.)

Mistake: Don't assume that issuers and verifiers will move in tandem.

## [IAM at the Front of the Cyber War: Are We Able to Beat the Bad Guys?](https://www.kuppingercole.com/sessions/5488)
_Ivo van Bennekom, EMEA Impact Center Leader Digital Identity_

Sweden saw rise in cyberattacks by 239% in the months prior to joining NATO.

## [Misinformation, Disinformation, Malinformation: How to Build Public Trust in a Crisis-Shaken World](https://www.kuppingercole.com/sessions/5495)
_Joni Brennan, Digital ID and Authentication Council of Canada_

Canada building a digital identity platform starting late 2021. Wow ... conspiracy theories killed this off.

I love her use of "super-spreaders" to describe misinformation ... super-spreader.

"Authenticity is the new identity."

## [Building Trust in a World of Misinformation and Crisis: Navigating the Storm](https://www.kuppingercole.com/sessions/5496)
_(panel)_

One panelist looking for a new term to fit somewhere on the spectrum between (human) unintentional misinformation, AI hallucination, and (human) _intentional_ misinformation.

Pablo: "We're still trying to find out how to label bad information (*); we should be thinking about how to label good information." (Hello!)

## [Standards are About Making Choices](https://www.kuppingercole.com/sessions/5499)

"Standards are about making choices that don't matter." (Examples: 200 is the HTTP status code for a successful response.) ... Except that they do. Everyone has to make the _same_ choices for the same concepts for a standard to lead to meaningful interoperability.

Key point: Choices matter. Making them improves interoperability.

Gives W3C VCs a C rating.

Gives DIDs a D rating. "But it does get worse."

Then gives Multiverse (an IETF proposal) an F rating. "It institutionalizes the failure to make a choice." See [Multiformats Considered Harmful](https://self-issued.info/?p=2408). 😱

## [Les Miserables of the Cyber Frontier: The Dueling Narratives of Decentralized Identities](https://www.kuppingercole.com/sessions/5572)
_Markus Sabadello and Nat Sakimura_

Like Kuppinger earlier today, Markus notes the shift in how much decentralized identity has become welcome here at EIC.

Interesting assertion: Data format can convey liberty. (Counterargument: The data format that supports liberty also adds complexity.)

# Wednesday Sessions

## [Panel: Latest on eIDAS Legislation and What it Means for People, Business and Government](https://www.kuppingercole.com/sessions/5510/1)

Estonia saves 2-3% of GDP by using digital signatures.

Awareness of friction inherent in multiple wallet implementations (i.e. each country has its own national wallet app -- is this really necessary?).

In Netherlands, there is a substantial cost (thousands of euros) to have a vetted business identity.

Talk of having wallets for businesses.

There is an eIDAS Expert Group which is advising member states on implementation details.

Audience question: Why isn't there just one wallet for the entire EU? _(Much laughter in the room.)_ Serious answer: Allow member states to continue using existing systems.

## [eIDAS 2, the Protocol Challenge and the Art of Timing](https://www.kuppingercole.com/sessions/5510/2)
_Andreas Freitag, Co-CEO, Procivis AG_

Analogy of one standard for all to Esperanto. It didn't work.

So be prepared to manage and embrace diversity. "You reach interoperability through flexibility." Very much the opposite of Mike Jones' keynote last night.

Write many, display as one, present what is required.

Ooh, Procivis has done _many_ implementations in Rust. (!) Note that Procivis has a trust list implementation.

## [eIDAS Architecture Reference Framework Status and Progress](https://www.kuppingercole.com/sessions/5546/1)
_Paolo De Rosa, Policy Officer, European Commission_

Key recent updates:

* Architecture Reference Framework on GitHub
* First release of libraries and software conponents for ARF
* Large-scale pilots underway

Ahhhh... relying parties need to be registered.

EC looking for active feedback _now._

## [Content Authenticity Overview and eIDAS Investigation: How Can eIDAS Support Content Creators?](https://www.kuppingercole.com/sessions/5553/1)
_Eric Scouten_

I gave a 15-minute talk about the Content Authenticity Initiative, identity, and the status of our investigation about how eIDAS-based identity might enable that technology.

But first ... a tech check. I was a theatre geek back in high school. Had to make sure my slides (which the AV staff at BCC were driving) were ready to go!

{{ es_image(id = "es-4663-016", caption = "Berlin Congress Center, Berlin, Germany") }}

Backstage, about ready to go on:

{{ es_image(id = "es-4663-020", caption = "Berlin Congress Center, Berlin, Germany") }}

And a few photos during my presentation, captured by my friend Judith Fleenor, executive director of the [Trust Over IP Foundation](https://trustoverip.org):

{{ es_image(id = "jf-246-2683", caption = "Berlin Congress Center, Berlin, Germany", creator = "Judith Fleenor") }}

{{ es_image(id = "jf-246-2686", caption = "Berlin Congress Center, Berlin, Germany", creator = "Judith Fleenor") }}

[Slide deck](./eic-cai-intro.pdf) (9MB PDF)

## [Panel: Real-World Examples of How Smart Wallets will Transform how we Navigate our Digital World](https://www.kuppingercole.com/sessions/5553/2)

Next I was part of a 45-minute panel discussion on how digital wallets will enable new relationships between consumers and businesses and governments.

{{ es_image(id = "jf-246-2693", caption = "Berlin Congress Center, Berlin, Germany", creator = "Judith Fleenor") }}

# Thursday Sessions

## [Panel: The Wallets we Want](https://www.kuppingercole.com/sessions/5590/1)

Fear of "decentralized silos." Too many context-specific wallets.

Martin Kuppinger suggests that we shift our thinking from "levels of assurance" of credentials and start thinking about *provenance* of credentials.

## [Securing the Foundations of Verifiable Credential Ecosystems](https://www.kuppingercole.com/sessions/5693/3)
_Dr. Daniel Fett, Security and Standardization Expert, Authlete_

No notes.

## [Introduction to the German EUDI Wallet Project](https://www.kuppingercole.com/sessions/5603/1)

Why eIDAS? Need to ensure that identity data is handled properly and with sufficient protection to users.

"Germany isn't a leader in digital identity." (Audience murmur.)

# Friday Sessions

As is so often the case for multi-day conferences, the last day of the conference is notably deflated compared to the other days as people start to make their journeys home. Such was the case on this Friday.

## [Panel: Decentralized Identity in Production](https://www.kuppingercole.com/sessions/5629/1)

I made one more panel appearance to talk about how we anticipate decentralized identity fitting into the Content Authenticity ecosystem.

{{ es_image(id = "jf-246-2746", creator = "Judith Fleenor") }}

# Wrap Up

After the morning panel, I needed to leave to make my own travel logistics work out.

All in all, this was a very impressive conference. Very well produced. Hats off to Jörg Resch who shared that this was the last conference he would be organizing before his upcoming retirement. Whoever manages the agenda for EIC 2025 will have very big shoes to fill.
