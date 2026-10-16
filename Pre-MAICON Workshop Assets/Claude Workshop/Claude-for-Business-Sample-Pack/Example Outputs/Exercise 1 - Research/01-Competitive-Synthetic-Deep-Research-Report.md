# Synthetic Deep Research Report

**Exercise 1 backup · Competitive analysis**

**Use this if your Exercise 1 didn't finish.** It's what the Exercise 1 prompt in your workbook produced from `01-Competitive-Visibility-Data.csv` plus a search of public sources from the last eighteen months, run on 30 September 2026. Every source below was opened and checked. Add it to your Project in Exercise 2 as "your Exercise 1 brief."

---

# Generative engine visibility: Trust Insights against Deloitte, McKinsey and BCG

## The short version

Trust Insights ranks fourth of four. On the file's own method (normalize every sub-metric to the leader, average within each dimension, weight the three dimensions equally) it scores **44.6, a D**, against McKinsey 95.5, Deloitte 78.4 and BCG 65.5. It leads the set outright on Relevance. On Presence and Appearance it is a small fraction of all three. The public research from the last eighteen months says Presence is the dimension most closely tied to showing up in AI answers, and Relevance-type work the least. So the gap worth closing first is Presence.

## The four organizations

**McKinsey** leads on every Presence and Appearance sub-metric in the file: 120,000 mentions in 90 days, 15,000 domains mentioning it, 220,000 referring domains, 3.2 million organic keywords. It ties Trust Insights on AI crawler accessibility and is second on the other four Relevance scores. The public record fits the numbers. Its flagship research gets written up by other people: third-party write-ups of *The State of AI 2025* repeat its "88 percent use AI, 6 percent are high performers" finding, and every write-up is a mention McKinsey didn't write. An April 2026 citation analysis lists McKinsey among the top-tier sources AI engines cite for B2B services, alongside HBR and Gartner, but the analysis doesn't explain how it ranked that vertical. Treat that as a hint, not a measurement.

**Deloitte** is second on every Presence and Appearance sub-metric and sits in the middle on Relevance, with the lowest Content Score in the set (65). Its 85,000 mentions come with a caveat the file can't show: mention counts don't separate good coverage from bad. In October 2025, Deloitte agreed to partially refund the Australian government for an AU$440,000 report that contained fabricated references produced with generative AI. That story was widely covered, and some share of Deloitte's mention volume in the period is coverage like it. Whether that helps or hurts how AI engines describe Deloitte, the file can't say.

**BCG** is third on Presence and Appearance and last or near-last on most Relevance scores: Schema 52, Alignment 65, Metadata 70. It's the weakest of the three large firms here, and still 8 to 17 times Trust Insights' size on every Presence metric, and 30 to 100 times on the Appearance scale metrics. Like McKinsey, its research travels. Its *AI at Work 2025* survey (10,635 employees, 11 countries) was picked up and analyzed by trade press within about a week.

**Trust Insights** leads the set on all four scored Relevance metrics (Metadata 88, Content 82, Schema 78, Alignment 85) and ties McKinsey on crawler accessibility. Everywhere else it is last, and not narrowly: total mentions are 4 percent of McKinsey's, blog and podcast mentions under 3 percent, organic keywords about 1 percent. Its closest non-Relevance number is Domain Rating (72, against 90 to 94), which means the site is well regarded for its size. It just isn't big. Trust Insights publishes a weekly podcast and blog on its own site through 2026, but owned content isn't what the Presence metrics count. They count what *other people* publish. One weak outside signal: a vendor-compiled list of generative engine optimization experts published in July 2026 doesn't include Trust Insights or its founders. That's one vendor's list and method, so don't lean on it.

## Across the three dimensions

| Dimension | Trust Insights | Deloitte | McKinsey | BCG | Where Trust Insights stands |
|---|---|---|---|---|---|
| Presence (6 sub-metrics) | 4.3 | 72.8 | **100.0** | 49.2 | About 3 to 5 percent of the leader on every sub-metric |
| Appearance (5 sub-metrics) | 29.5 | 85.0 | **100.0** | 71.3 | Close on authority (DR 72), far behind on scale (keywords, pages, referring domains) |
| Relevance (5 sub-metrics) | **100.0** | 77.3 | 86.4 | 76.1 | Leads on all four scored metrics, ties on crawler access |
| **Overall (equal thirds)** | **44.6 (D)** | 78.4 (B) | 95.5 (A) | 65.5 (C) | Fourth of four |

The ranking doesn't depend on the weighting. Weight Presence at half and Trust Insights falls to 34.5. Weight Relevance at 60 percent and it rises to 66.7, still fourth. McKinsey is first either way.

## Evidenced

- **The scores above.** Computed from the attached file. Every number in the table can be reproduced from it.
- **Presence-type signals track AI visibility far more closely than site authority does.** Ahrefs studied 75,000 brands across ChatGPT, AI Mode and AI Overviews (December 2025). YouTube mentions correlated at about 0.71 to 0.74 with AI visibility, and branded web mentions at 0.66 to 0.71. Domain Rating was 0.27 to 0.33, backlinks about 0.2, and the number of pages on a site about 0.19. These are correlations, not causes, and the authors say so.
- **Ranking in search matters less than it did.** Ahrefs found that 38 percent of pages cited in Google AI Overviews rank in the organic top 10 (March 2026), down from 76 percent in July 2025.
- **Adding schema markup didn't move AI citations.** Ahrefs tracked 1,885 pages that added schema against 4,000 control pages (May 2026) and found no meaningful uplift on any platform. The caveats: only pages that were already heavily cited, and a 30-day window.
- **llms.txt shows no measurable effect on AI citations.** SE Ranking studied about 300,000 domains (November 2025).
- **Google favors big brands more than ChatGPT and Perplexity do.** Ahrefs (July 2025) found web mentions correlated with visibility at 0.65 in AI Overviews, 0.30 in Perplexity and 0.15 in ChatGPT, although its December 2025 study found big brands ahead on every platform.
- **Consulting firms' own sites aren't among the domains AI engines cite most overall.** Semrush's 100-million-citation study (November 2025) is led by Reddit, Wikipedia, LinkedIn and YouTube. Third-party platforms, not firm websites, dominate.

## Inference (my read, not established)

- **Trust Insights' Relevance lead is real, but it probably isn't buying much.** The evidence above says the technical and on-page work that Relevance measures has a weak or unproven link to being cited. That's a reason to maintain it, not to invest more in it.
- **The Big Three aren't the right benchmark for a budget decision.** Trust Insights can't close a 20-to-1 mention gap with firms of that size in a quarter, or in several. The useful question is share of voice on a narrow set of topics where it has standing: AI measurement, analytics, the frameworks it teaches. This file doesn't measure that.
- **YouTube is the most specific lever.** It had the strongest correlation in the largest study, and it's where Trust Insights is 30 videos against BCG's 250. The file doesn't say whether "YouTube Content Volume" counts Trust Insights' own videos or videos about it, and that changes the recommendation. Check before you spend.
- **Mention volume overstates the large firms' advantage somewhat.** Some of it is unfavorable coverage, as with Deloitte in Australia. The file can't separate sentiment, so neither can this brief.
- **The file itself is a proxy.** It measures inputs that correlate with AI visibility. It doesn't show what ChatGPT, Gemini or AI Overviews actually say about any of these four when asked. The sub-metrics also carry no collection dates or sources, and the Relevance scores have no stated method.

## What to do about it, in priority order

1. **Put next quarter's new money into Presence, on other people's channels, on two or three topics.** Guest podcasts, co-authored pieces, conference talks that get written up, and YouTube, in that order of evidence. Don't aim at McKinsey's volume. Aim to be the name that comes up on the topics you choose.
2. **Measure what AI engines actually say before you spend, and again after.** Pick 20 to 30 questions your buyers ask, record which organizations each engine names, and repeat monthly. It's cheap, and it's the only way to know whether step 1 worked. The file can't tell you that.
3. **Hold Relevance and Appearance at maintenance.** Keep the metadata, content and crawler access you already lead on. Don't fund more schema or llms.txt work on the current evidence, and don't try to close the backlink or keyword gap by force. It's the wrong fight at this scale.

## Where the evidence is thin

- Almost all the public research on what drives AI citations comes from SEO tool vendors (Ahrefs, Semrush, SE Ranking). It's the best available, it's correlational, and the platforms change monthly.
- No independent source in the window measures AI visibility for these four organizations specifically.
- None of the four companies' own press releases were used.

## Sources

From the attached file: `01-Competitive-Visibility-Data.csv` (16 sub-metrics, four organizations; no collection dates given).

- Ahrefs, *Top Brand Visibility Factors in ChatGPT, AI Mode, and AI Overviews (75k Brands Studied)*, 12 December 2025. https://ahrefs.com/blog/ai-brand-visibility-correlations/
- Ahrefs, *Update: 38% of AI Overview Citations Pull From The Top 10*, 2 March 2026. https://ahrefs.com/blog/ai-overview-citations-top-10/
- Ahrefs, *We Tracked 1,885 Pages Adding Schema. AI Citations Barely Moved.*, 11 May 2026. https://ahrefs.com/blog/schema-ai-citations/
- Ahrefs, *Google Seems More Biased Towards Big Brands Than ChatGPT and Perplexity*, 7 July 2025. https://ahrefs.com/blog/branded-web-mentions-visibility-ai-search/
- Search Engine Journal, *LLMs.txt Shows No Clear Effect On AI Citations, Based On 300k Domains* (SE Ranking study), 20 November 2025. https://www.searchenginejournal.com/llms-txt-shows-no-clear-effect-on-ai-citations-based-on-300k-domains/561542/
- Semrush, *The Most-Cited Domains in AI: A 3-Month Study*, 10 November 2025. https://www.semrush.com/blog/most-cited-domains-ai/
- Digital Applied, *AI Search Citation Analysis Q2 2026: Domains Ranked*, 16 April 2026. https://www.digitalapplied.com/blog/ai-search-citation-analysis-q2-2026-domains-ranked
- The Register, *Deloitte refunds Australian government over AI in report*, 6 October 2025. https://www.theregister.com/2025/10/06/deloitte_ai_report_australia/
- UNLEASH, *BCG's AI at Work 2025 report: Four takeaways for HR leaders*, 3 July 2025. https://www.unleash.ai/artificial-intelligence/analysis/bcgs-ai-at-work-2025-report-four-takeaways-for-hr-leaders
- Winsome Marketing, *McKinsey's State of AI Report: 88% Adoption, But Only 6% Are Actually Winning* (covers the June to July 2025 survey). https://winsomemarketing.com/ai-in-marketing/mckinseys-state-of-ai-report-88-adoption-but-only-6-are-actually-winning
- Profound, *The 2026 A-list of generative engine optimization (GEO) experts*, 26 July 2026. https://www.tryprofound.com/articles/top-experts-in-generative-engine-optimization
- Trust Insights, *In-Ear Insights: AI Skills Governance*, August 2026, one of the weekly episodes on its own site. https://www.trustinsights.ai/blog/2026/08/in-ear-insights-ai-skills-governance/
