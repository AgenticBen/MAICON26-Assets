---
name: geo-competitive-scorecard
description: Score a competitive set (2-6 brands) across Presence, Appearance, and Relevance using Trust Insights' GEO 201 normalize-to-leader methodology. Use when the user asks to "score this competitive set," "build a scorecard," "run the GEO scorecard," or provides raw sub-metric values for a brand comparison and wants dimension scores, a weighted overall score, a letter grade, a rank, and gap analysis.
---

# GEO Competitive Scorecard

## Overview

This skill turns raw competitive research (mentions, domain metrics, content-quality scores, or similar) into a scored, ranked, auditable scorecard using Trust Insights' GEO 201 methodology. It's the middle step of a three-step workflow: a research brief gives the directional picture, this skill turns it into numbers, and Code can optionally rerun the same math on a full dataset.

## When to Use This Skill

Use this skill when the user:
- Asks to "score this competitive set," "build a scorecard," or "run the GEO scorecard"
- Pastes raw research (mentions, backlinks, content-quality notes, etc.) about their brand vs. competitors and wants it turned into a structured comparison
- Provides a table of sub-metric values across brands and wants dimension scores, a weighted overall, a letter grade, or a rank
- Asks "who's winning" or "where are our gaps" about a competitive set already described in the conversation

## Workflow

### Step 1: Identify the competitive set and dimensions
Confirm the brands being compared (2-6) and the dimensions in play. Default to three: **Presence** (how much content exists about a brand), **Appearance** (how findable it is in search), **Relevance** (how usable its content is once found). If the user's use case doesn't fit GEO, ask what 2-4 dimensions they want instead — the scoring math is dimension-agnostic.

### Step 2: Collect sub-metrics
For each dimension, gather 4-6 measurable sub-metrics per brand (e.g., Presence: total mentions, unique domains, news mentions, blog/podcast mentions, YouTube volume, author diversity). Extract these from pasted research if a structured table isn't provided, and confirm your extraction with the user before scoring — don't silently guess at numbers.

### Step 3: Normalize each sub-metric to the category leader
For every sub-metric, the brand with the highest raw value becomes the leader and scores 100. Every other brand scores:

```
normalized_score = (their_value ÷ leader_value) × 100
```

### Step 4: Roll up to dimension scores
Average the normalized sub-metric scores within each dimension to get that dimension's score (0-100) for each brand.

### Step 5: Compute the weighted overall score
```
weighted_overall = (Presence × weight) + (Appearance × weight) + (Relevance × weight)
```
Default weights are equal thirds (33.33 / 33.33 / 33.34). Ask the user if they want custom weights (e.g., to emphasize one dimension).

### Step 6: Assign a letter grade
- A: 85–100
- B: 70–84
- C: 55–69
- D: 40–54
- F: below 40

### Step 7: Rank and flag gaps
Rank all brands by weighted overall score. Flag:
- **White space:** any dimension where the category-max score is below 60 (nobody in the set owns it)
- **Priority fix:** any dimension where the user's own brand ranks last

### Step 8: Output
Produce:
1. A scorecard table — Brand | [Dimension] score columns | Weighted Overall | Grade | Rank
2. A 2-3 sentence narrative summary naming the biggest gap and the biggest strength
3. A gap/opportunity callout listing anything flagged in Step 7

## Notes

- Always show your work (raw value → normalized score → dimension average → weighted overall) so the result is auditable, not a black box.
- This is designed to be rerun on the same competitive set every quarter to track score deltas over time — a scheduled task in Claude is a natural fit for that cadence.
- Originally built for Trust Insights' GEO 201 course (competitive Generative Engine Optimization). The math generalizes to any multi-dimension competitive comparison, not just GEO.
