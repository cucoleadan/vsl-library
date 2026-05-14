---
name: prepublish-fact-checker
description: >
  Extract factual claims from article drafts, verify them against primary or authoritative sources,
  flag outdated or unsupported statements, and rewrite weak claims with honest attribution.
  Use when preparing a newsletter, guest post, blog post, comparison, tutorial, or essay for publication
  and you need a pre-publish fact-checking pass, source links, or a clear distinction between firsthand
  experience and researched claims.
---

# Prepublish Fact Checker

Run this skill after a full draft exists and before publication. Use it to separate real verification work from style editing.

## Scope the Pass

Read the full draft first. Separate claims that need verification from opinion, framing, storytelling, and personal reflection.

Verify claims about:
- dates
- numbers
- pricing
- launch timelines
- feature availability
- company, model, or product naming
- comparisons stated as facts
- quotes
- "I tested" or "I found" statements that imply firsthand use

Do not waste time trying to "verify" subjective takes, analogies, or obvious transitions.

## Workflow

### 1. Extract the Claim Ledger

Turn the draft into a numbered claim ledger.

For each entry, record:
- a short paraphrase of the claim
- claim type: date, pricing, feature, benchmark, quote, comparison, firsthand, or other
- verification priority: high, medium, or low
- whether the claim needs an external source or user confirmation

Prefer atomic claims. If one sentence contains multiple facts, split it into multiple entries.

### 2. Verify Each Claim With Sources

Use web research for unstable or external claims. Prioritize sources in this order:
1. official docs, pricing pages, product pages, company announcements, filings, or regulatory sources
2. original research, benchmark writeups, or direct transcripts
3. reputable secondary coverage only when primary sources are unavailable

For technical or product claims, prefer official documentation.
For benchmarks, cite the original benchmark or test source, not a summary post.
For pricing, record the exact date checked.
For news-sensitive claims, record both the event date and the date verified.

Give each claim one verdict:
- verified
- verified but needs nuance
- outdated
- unsupported
- user confirmation required

Include direct source links with every verified or corrected claim.

### 3. Run the Honesty Pass

Check whether the draft overstates firsthand knowledge.

Ask:
- Did the writer personally test this?
- Did the writer observe this directly?
- Is this based only on research, docs, reviews, or another person's benchmark?

If the draft contains multiple firsthand claims and testing status is unclear, pause and ask the user which tools, products, or workflows they personally tested.

When firsthand status is unclear or false, rewrite the sentence to credit the source without flattening the voice.

Useful rewrite patterns:
- "In one test I studied..."
- "Based on the docs and current pricing pages..."
- "Reviewers consistently report..."
- "According to [source]..."
- "The company says..."

### 4. Produce the Pre-Publish Report

Return four sections:
1. `Verified claims`
2. `Claims fixed or softened`
3. `Open flags`
4. `Suggested rewrite snippets`

Keep rewrites short and ready to drop into the draft.

## Working Rules

- Use absolute dates, not relative timing like "currently," "recently," or "today," unless anchored to a real date.
- When sources disagree, say so plainly and show the conflict.
- When a claim cannot be verified quickly, flag it instead of bluffing.
- Prefer one strong source over several weak echoes.
- Do not turn this pass into a full structural rewrite unless the user explicitly asks for that.
- Raise the risk level for legal, health, safety, financial, or earnings claims and be stricter about sourcing.

## Output Shape

For each claim that matters, use this format:

- `Claim:` short paraphrase
- `Status:` one verdict from the list above
- `Evidence:` one or two sentences
- `Source:` direct link or links
- `Suggested fix:` revised sentence only when needed

## Finish Line

A good run leaves the writer with:
- a clean claim ledger
- source links for every material fact
- corrected dates, numbers, and pricing
- honest language where firsthand testing is missing
- a short unresolved list that needs the writer's input
