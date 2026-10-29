---
name: moonsong-writing
description: Moonsong Labs style and voice guide for external-facing writing, including blog posts, engineering articles, case studies, landing pages, social posts, whitepapers, and pitch decks. Use whenever drafting, editing, or reviewing anything published by or on behalf of Moonsong Labs, or writing for an audience of regulated financial institutions. Trigger even when the guide isn't named, for requests like "draft a LinkedIn post," "write up this engineering post for the Moonsong blog," "edit this case study," "clean up this landing page," or "check this draft for AI tells."
---

# Moonsong Labs writing guidelines

This is the style and voice reference for everything Moonsong Labs publishes: marketing pages, case studies, social posts, decks, and articles written by our engineers. It exists so that an engineer's technical post and a founder's LinkedIn post sound like they came from the same firm.

Internal writing (proposals, SOWs, memos, Slack) is not held to every rule here. It should still be plain and direct. Internal strategy documents read like memos, with the main point up front, and skip punchy marketing phrasing.

Before publishing anything, run the [final-pass checklist](#final-pass-checklist) at the bottom.

## Contents

- Core principles
- Voice and tone
- Openings and endings
- Structure and formatting
- Writing technical content
- Channel notes
- Calls to action
- Language and constructions to avoid
- House terminology and mechanics
- Named companies, clients, and quotes
- Numbers and claims
- Review before publishing
- Final-pass checklist

The examples throughout are illustrative. Client names and figures in them are placeholders.

## Core principles

Claims are grounded in what has actually shipped. Moonsong writes from the position of a firm that has built the systems it's describing. When making a claim about how institutions behave, what production infrastructure requires, or what a technology enables, back it with direct experience or a named, verifiable example. If you can't, find the evidence or cut the claim.

Business outcomes over technical mechanics. The audience for most Moonsong writing is a business decision-maker at a regulated financial institution. Explain what a technology means for the institution's risk posture or competitive position. Explain the mechanism when the mechanism is the point. (Engineering articles are the exception; see [Writing technical content](#writing-technical-content).)

Confident without being evangelical. Moonsong does not write like a crypto-native firm. Avoid "this changes everything," "the future is onchain," "trustless," "revolutionary," and similar registers. Write the way a technical peer would speak to another executive: calmly and specifically, with a clear point of view and no ideological charge.

Forward-looking, not defensive. Don't relitigate past hype cycles, address skeptics directly, or pre-empt objections no one has raised. Assume the reader is intelligent and already past the "does blockchain matter" question.

Peer-level, not advisory. Moonsong writes as someone who has been inside the same organizational dynamics the reader is navigating.

## Voice and tone

Moonsong's voice is conversational and discursive. Sentences flow and connect, and each paragraph develops one idea.

Use "we" for Moonsong or the Moonsong team. Prefer "the institutions we're working with" or "clients we're seeing" over "the market" when the observation comes from our own work. In a bylined post, "I" is fine for your own experience and decisions; switch to "we" when describing what the team built.

Hedge appropriately. Moonsong has strong opinions, but overstating certainty on contested topics undermines credibility. "We're seeing" and "tends to" are fine when the observation isn't universal yet. Don't hedge a claim we hold with full conviction.

Don't use "just" as a minimizer ("it's just a matter of," "just a pilot"). It reads as dismissive.

## Openings and endings

Open with the specific thing: the observation or what was built. The first sentence should tell the reader what the piece is about and why it's worth their time.

Avoid these openings:

- A rhetorical question ("What if settlement took seconds instead of days?").
- A statistic followed by an explanation of why the statistic matters.
- A scene-setting line about the industry ("The financial services landscape is changing rapidly.").
- A definition the reader already knows ("Tokenization is the process of...").

End on the last substantive point or a specific closing thought. Don't end with "In conclusion," "In summary," "Overall," or a restatement of what the piece already said. For long-form content a genuine synthesis is fine; a recap dressed up as a conclusion is not.

## Structure and formatting

Prose is the default. Numbered lists and bullets are fine when the content is a list, such as sequential steps or distinct product features. Content that reads better as paragraphs stays in paragraphs.

Bullets, when used, should be at least a sentence long. Navigation lists like a table of contents are the one exception.

No em dashes. Use commas, periods, parentheses, or restructure the sentence. If a sentence seems to need an em dash, it's usually doing too much and should be split.

No single-phrase or single-word paragraphs. Avoid "Distribution." or "The result?" or "That's the point." as standalone lines. They're a recognizable AI and marketing tell.

Sentence case for all headings and titles, including case study and article titles. "How institutions evaluate Canton," not "How Institutions Evaluate Canton." Proper nouns keep their capitals.

Boldface is rare. Use it when introducing a specific term or when a single phrase needs visual weight. Don't bold every important phrase in a paragraph.

One piece, one argument. Especially for social and blog posts. If a draft contains two distinct observations, split it into two pieces.

## Writing technical content

This section is for engineers writing articles, tutorials, implementation guides, and deep dives for the Moonsong blog or partner channels.

Decide who the reader is before you start, and say so early. Most technical pieces have one of two readers: an engineer who will implement something, or a technical decision-maker evaluating an approach. For the first, get to the mechanism quickly. For the second, lead with what the approach means operationally (cost, risk, time to production, what it lets the institution do), then explain how it works.

Explain tradeoffs. What you chose not to do, and why, is often the most credible part of a technical piece. "We considered running a separate privacy chain per counterparty and rejected it because of the operational overhead for the bank's ops team" tells the reader we've built this for real.

Be specific about context. Name versions, networks, environments, and conditions. A benchmark without its setup (hardware, load profile, network, version) shouldn't be published. "Finality in under two seconds on mainnet under normal load" beats "lightning-fast finality."

Use code when the code is the point. Keep snippets short and focused on the idea being explained. Tag the language on every code block. Comment only where the code isn't self-explanatory. Never include secrets, keys, internal hostnames, client identifiers, or anything copied from a client codebase.

Define acronyms on first use for a mixed audience. For a purely engineering audience, don't define basics like RPC or SDK.

Write headings that say what the section says. "Why we batch nonce updates" is more useful than "Implementation details."

Everything else in this guide still applies. Technical writing is where puffery ("blazing fast," "robust," "seamless integration") creeps in most, so watch for it.

Technical posts often touch on client architecture or security-relevant detail. See [Review before publishing](#review-before-publishing).

## Channel notes

LinkedIn posts. One argument per post. Roughly 100 to 250 words. The first line carries the observation, because it's all most readers see before "see more." No engagement bait ("Agree?", "Thoughts?"), no hashtag walls (zero to three hashtags), and no emoji.

X threads. Every post in the thread should stand on its own if quoted. Plain "1/" numbering is fine; no thread emoji. The first post states the point.

Blog posts and engineering articles. Usually 800 to 2,000 words. For anything over about 1,200 words, open with a short paragraph that tells the reader what they'll learn and who it's for.

Case studies. Cover the client, the problem they had, what we built, and what changed. Every claim needs to be verifiable and approved by the client before publication. Describe outcomes in the client's operational terms, such as time to settle or manual steps removed.

Guides and whitepapers. More structure is fine here (numbered sections and tables), but the writing inside each section is still prose-led.

Decks. One idea per slide. Slide headlines are full sentences that state the point ("Settlement moved from T+2 to same day").

Landing pages. Short and concrete. Say what Moonsong does and what it looks like in production. The puffery rules apply with extra force.

## Calls to action

Give the reader one specific next step that matches where they are. A reader learning about a topic gets "read the implementation guide." A reader evaluating vendors gets "talk to our engineering team about your use case."

No urgency or scarcity language ("don't get left behind," "act now"). It reads as consumer marketing and undercuts the peer-level tone.

Engineering articles don't need a sales CTA. A link to the repo or a way to reach the author is enough.

## Language and constructions to avoid

Each of these patterns reads as AI-generated or generic marketing copy. Strip them before publishing.

### Puffery and promotional language

Don't describe Moonsong's work, clients, or the industry in inflated language. Cut words like "robust," "leverage" (as a verb), "seamless," "cutting-edge," "world-class," "best-in-class," "vibrant," "rich," "unlock" (unless something is literally being unlocked), "empower," "transform" (as a metaphor), "revolutionize," "elevate," and "supercharge."

Avoid: "Moonsong leverages robust, cutting-edge infrastructure to empower institutions to unlock the transformative potential of tokenization."

Write: "Moonsong builds settlement infrastructure for [type of institution]. The system we shipped for [client] has been in production since [date]."

### Compound abstractions used as rhetorical trump cards

Phrases like "the operating model," "the architecture bet," "the market direction," "the real story," and "the underlying dynamic" often show up at the end of a paragraph as if delivering an insight, when they're substituting for one. Name the specific thing.

Avoid: "That's the architecture bet institutions are making."

Write: "That's why the institutions we're working with are settling across two chains at once instead of committing to one."

### Meta-signals that insight is coming

"The reality is," "the truth is," "here's what's actually happening," "the real story is," "make no mistake," and "the thing to understand is" announce that an insight is coming. Cut them and let the observation stand.

### Antithesis constructions ("not X, but Y")

The "not X, but Y" construction and its cousins ("less about X, more about Y," "the question isn't X, it's Y," "that's not X, that's Y") are among the most recognizable AI writing tells. They feel sharp but usually wrap a claim that could be made directly.

If the sentence works with only the Y half, cut the X half. If it doesn't, the observation probably isn't strong enough yet.

Occasional use is fine when the contrast is load-bearing, meaning the reader would assume X and Y is the correction. Default to direct assertion.

Avoid: "That's not a technical decision. That's a strategic bet on where the market is going."

Write: "That decision reflects where they think the market is going."

### The "-ing" appendage

LLMs habitually attach a present-participle phrase to the end of a sentence to add significance. It almost always inflates the sentence without adding information.

Avoid: "The bank launched its tokenized fund platform in 2025, marking a pivotal moment in institutional tokenization and highlighting the growing conviction that blockchain will play a central role in regulated finance."

Write: "The bank launched its tokenized fund platform in 2025. Subscriptions and redemptions now settle onchain the same day."

### Undue emphasis on legacy, significance, or broader trends

Cut "stands as a testament to," "marks a pivotal moment in," "underscores its significance," "reflects broader trends in," "represents a shift toward," "sets the stage for," "an enduring symbol of," "shaping the future of," and "a defining moment for."

If a development matters, describe concretely why. Don't tell the reader it's significant.

### Weasel attributions

Avoid unnamed authorities: "industry observers argue," "experts say," "many analysts believe," "sources suggest," "some critics have noted," "it is widely believed that." Cite a specific person or publication, or make the claim directly in Moonsong's voice.

Don't write "several sources" or "many publications" when only one or two are being referenced.

### Formulaic "challenges and future" framings

Don't end pieces with a "Challenges" or "Future outlook" section that follows the pattern "Despite [positive things], [subject] faces challenges including... Despite these challenges, [subject] continues to..."

If there are real challenges, name them specifically without defensive framing. If there aren't, don't invent them for symmetry.

### Rule of three

LLMs disproportionately favor lists of three: three adjectives, three nouns, three parallel phrases. Break the pattern. Two is fine. Four is fine. A single well-chosen word is often best.

Avoid: "The infrastructure is efficient, auditable, and scalable."

Write: "The infrastructure is auditable at the transaction level." (If auditability is the actual point.)

### Elegant variation

Don't synonym-hop to avoid repeating a word. If "institution" is the right word, use it every time instead of cycling through "organization," "firm," "enterprise," and "player." Variation makes the reader wonder whether you mean different things.

### AI vocabulary

These words are disproportionately overused by LLMs. Cut them unless no plainer word does the job.

Nouns and adjectives: crucial, pivotal, intricate, vibrant, robust, enduring, key (as an adjective), significant, meaningful (as filler), valuable, comprehensive, seamless, dynamic, tapestry, landscape (as metaphor), interplay, cornerstone, testament.

Verbs: delve, leverage, navigate (as metaphor), foster, cultivate, empower, unlock, harness, showcase, underscore, highlight (as a verb signaling importance), align with, enhance, streamline, drive (as in "drives growth"), enable (used lazily).

Transitions: additionally (especially as a sentence starter), moreover, furthermore, notably, importantly, it's worth noting, particularly interesting.

Hedges of significance: "may prove," "could reshape," "has the potential to."

None of these is banned outright. If the word is doing real work in the sentence, keep it. If it's inflating a generic sentence, cut it.

### Avoidance of "is" and "has"

LLMs replace simple verbs with inflated ones: "serves as," "stands as," "functions as," "operates as," "represents," "constitutes," "features," "offers," "boasts." Use "is" and "has" when they're the right words. They usually are.

Avoid: "The privacy layer serves as the infrastructure that enables institutional confidentiality."

Write: "The privacy layer is what keeps each bank's transactions hidden from the other banks on the network."

### Showcase, highlight, demonstrate

These verbs get used as generic connectors. Use a verb that says what actually happened. "The bank uses the platform to settle fund redemptions" beats "The deployment showcases the platform's capabilities."

### Emoji, decorative bullets, and title-case headings

No emoji anywhere in external content. No decorative bullets (•, →, ⚡, ✓). Sentence case for all headings.

### Knowledge-cutoff and availability hedges

Don't write "as of the most recent data available," "based on publicly available information," "while specific details are limited," or "though comprehensive data is not widely available." If we don't know something, find out before writing or leave it out.

## House terminology and mechanics

Use these consistently across every channel.

| Use | Not | Notes |
|---|---|---|
| onchain, offchain | on-chain, on chain | One word, no hyphen, in all copy. |
| Moonsong Labs, then Moonsong | MSL, Moonsong labs | Full name on first reference, "Moonsong" after. |
| tokenized, tokenization | tokenised | US spelling throughout. |
| stablecoin | stable coin, stable-coin | |
| digital assets | crypto | "Crypto" is fine when quoting someone or describing crypto-native markets specifically. |
| real-world assets (RWAs) | RWAs unexplained | Spell out on first use. |
| smart contract | Smart Contract | Lowercase unless starting a sentence. |
| Canton Network, then Canton | the Canton | Full name on first reference. |
| institutions, or the specific type (banks, asset managers, custodians) | TradFi, legacy finance, the industry | Name who you mean. |
| | Web3 | Avoid. Name the specific technology or network. |

Write company, product, and network names the way their owners write them. Check their website if unsure.

Mechanics:

- Use US English.
- Use the serial comma ("banks, asset managers, and custodians").
- Spell out numbers one through nine; use numerals for 10 and above and for money and percentages, and in technical contexts ("3 nodes" is fine in a technical context).
- Write percentages as "40%" and money as "$2.5 million" or "$2.5M" in tight spaces like slides.
- Write dates as "October 29, 2026." Avoid numeric dates, which read differently in the US and Europe.
- Use "T+2," "T+0," and similar settlement notation as written.

## Named companies, clients, and quotes

When naming clients or partners, be specific about what was built and for whom. Vague references ("a leading global bank," "a top-tier asset manager") are only appropriate when confidentiality requires them, and even then, describe the shape of the work.

Concrete detail is stronger: "the settlement system we built for [client], now processing their tokenized deposit transfers" beats "our work with leading financial institutions."

Don't name a client, describe their architecture, or attribute a quote to anyone at a client or partner company without approval. Never invent quotes.

When describing joint work with a partner, be precise about who built what. Don't present a partner's product as Moonsong's, or Moonsong's contribution as the whole system.

## Numbers and claims

Use specific numbers whenever possible. Concrete figures with a source ("roughly 40 firms," "15 months," a figure from a named report) are more credible than vague magnitudes ("massive scale," "many institutions").

Avoid false precision. "Roughly 40 firms" is better than "40 firms" if the count fluctuates.

Name the source of external data in the prose or a citation. Don't write "reports indicate" when a specific report exists.

## Review before publishing

Send a draft to Moonsong marketing before it goes out if it does any of the following:

- Names a client or partner, or describes work done for one.
- Includes architecture details, security-relevant information, or code from a client engagement.
- Makes a claim about Moonsong's scale, track record, or results.
- Will run on a partner's channel or as co-marketing.

Engineering posts that cover open-source work or general techniques, with none of the above, need only the normal team review.

## Final-pass checklist

Before publishing any external Moonsong writing, check:

1. Are there em dashes? Remove them.
2. Are there single-phrase paragraphs? Fold them into surrounding prose.
3. Are there "not X, but Y" constructions? Convert to direct assertion unless the contrast is doing real work.
4. Are there "-ing" appendages inflating sentences? Cut them.
5. Are there AI vocabulary words (robust, leverage, pivotal, delve, showcase)? Replace with specific language or cut.
6. Are there compound abstractions ("the operating model," "the architecture bet") acting as rhetorical trump cards? Name the specific thing.
7. Are there weasel attributions ("experts say," "industry observers")? Name the source or make the claim directly.
8. Are there rule-of-three lists? Break the pattern where it isn't load-bearing.
9. Are there title-case headings or titles? Convert to sentence case.
10. Are there emoji or decorative bullets? Remove them.
11. Does the opening start with the specific thing, or with a question, a statistic, or industry scene-setting? Rewrite if needed.
12. Does the piece end with "In conclusion" or a recap? Rewrite the ending.
13. Is terminology consistent with the house list (onchain, tokenized, Moonsong Labs on first reference)?
14. Are all named clients, numbers, and claims verifiable and approved?
15. For technical pieces, do benchmarks include their conditions, and is the code free of secrets and client details?
16. Is there one clear call to action, with no urgency language?
17. Does the piece make one argument? If it has stitched two together, split it.
