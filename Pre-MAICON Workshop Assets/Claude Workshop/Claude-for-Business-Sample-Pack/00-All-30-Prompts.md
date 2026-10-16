# The prompts, by scenario

Every prompt is written on CASINO: Context, Audience, Scope, Intent, Narrator, Outcome. Pick the scenario closest to your own work and follow it through all six exercises. Change anything in [square brackets]. If you're using your own material instead of the sample, keep the structure and change the subject.

*Generated from `source/wb_prompts.py`. Edit there, not here.*

---

## 1. Competitive analysis

**Sample file:** `01-Competitive-Visibility-Data.csv`. Trust Insights against Deloitte, McKinsey and BCG on generative engine visibility. The numbers are real and already public.

### Exercise 1: Research

*Switch on Research, attach 01-Competitive-Visibility-Data.csv, and paste this.*

**Context.** I am assessing how Trust Insights compares against Deloitte, McKinsey and BCG on generative engine visibility. The attached file has sixteen sub-metrics across three dimensions (Presence, Appearance and Relevance) for all four organizations.

**Audience.** Our leadership team, who need to decide where next quarter's budget goes.

**Scope.** Only the data in the attached file, plus public sources from the last eighteen months. Exclude the companies' own press releases.

**Intent.** This has to support a decision about where we invest next quarter. I need to know where we genuinely lead, where we genuinely lag, and which gap is worth closing first.

**Narrator.** Act as a competitive analyst who is skeptical of marketing claims and says plainly when the evidence is thin.

**Outcome.** One paragraph per organization. A comparison across the three dimensions. A clearly labeled split between what is evidenced and what is inference. Three things I should do about it, in priority order.

> **How you know it worked:** Spot-check three citations. If two don't support the claim, tighten Scope and run it again.

### Exercise 2: Project

*Create a Project called [GEO competitive]. Add 01-Competitive-Visibility-Data.csv and your Exercise 1 brief. Paste this into the Project instructions.*

**Context.** This Project holds our competitive work on generative engine visibility: Trust Insights against Deloitte, McKinsey and BCG. The data file has sixteen sub-metrics across Presence, Appearance and Relevance. The Exercise 1 brief is our starting read.

**Audience.** Our leadership team. They decide where next quarter's budget goes, and they will ask how every number was produced.

**Scope.** Use the files in this Project and any sources I give you. Name anything else you use. If a figure isn't in the data, say so. Never estimate one.

**Intent.** Every answer in this Project should help decide which visibility gap is worth closing first.

**Narrator.** A competitive analyst who is skeptical of marketing claims, including ours.

**Outcome.** Keep evidence and inference in separate, labeled sections. Use the three dimension names exactly as the file does. Tell me when the data is too thin to support a conclusion.

> **How you know it worked:** Ask one short question, like "Where are we strongest?" If the answer comes back in our terms without you explaining them, the Project is working.

### Exercise 3: Artifact

*In the same Project, paste this.*

**Context.** Use the data file and the brief in this Project.

**Audience.** The leadership team, opening it without me in the room.

**Scope.** The four organizations and three dimensions in the file. Nothing added.

**Intent.** They need to see where we stand and which gap to close first, and trust the numbers enough to act on them.

**Narrator.** A data analyst who shows her working.

**Outcome.** An interactive scorecard: one row per organization, one column per dimension, each scored 0 to 100 by normalizing to the leader. Click a score to see the sub-metrics behind it. Show the calculation, not just the result. Put the one gap worth closing first at the top, in a single sentence.

> **How you know it worked:** Change one number in the data and check the score moves the way you'd expect.

### Exercise 4: Skill

*Still in the Project, paste this.*

**Context.** We just scored four organizations on generative engine visibility: collect the sub-metrics, normalize each to the leader, roll up to Presence, Appearance and Relevance, weight them, and grade.

**Audience.** Anyone on the team who needs a scorecard for a different competitive set, without me explaining the method.

**Scope.** The method, not these four companies. It should work for any set of two to six organizations.

**Intent.** I want the same scorecard, built the same way, every time, without rewriting this prompt.

**Narrator.** A methodologist writing instructions for a capable colleague who wasn't in the room.

**Outcome.** A Skill called geo-competitive-scorecard. A description that says when to use it. Then the steps in plain English, the weighting and grading rules, and the three things that most often go wrong. Then test it on a set of competitors we didn't use today and show me the result.

> **How you know it worked:** If it only works on the original four, you encoded an instance, not a method.

### Exercise 5: Plugin

*Once the Skill has worked on a second set of competitors, paste this.*

**Context.** The geo-competitive-scorecard Skill works, and I've tested it on a second set of competitors.

**Audience.** Colleagues who have never seen it and won't ask me before they use it.

**Scope.** Bundle the Skill and the connector it needs for current data. Nothing else.

**Intent.** I want other people running this without me being the bottleneck.

**Narrator.** A product manager writing for a stranger.

**Outcome.** A Plugin with a one-line description that says when to reach for it, not what it does. Add a short note on what it does badly, so nobody over-trusts it. For example: it can't see mentions behind paywalls, and a small organization will always look weak on Presence.

> **How you know it worked:** Give it to one colleague with no explanation. If they have to ask you anything, rewrite the description.

### Exercise 6: Scheduled task

*Create a scheduled task, set its model to Sonnet, and paste this as its instructions.*

**Context.** Run the geo-competitive-scorecard Skill on the same four organizations.

**Audience.** Me first. The leadership team only if something moved.

**Scope.** Quarterly, on the first business day of the quarter.

**Intent.** I want to know what changed since last quarter, not reread the same scorecard.

**Narrator.** An analyst writing for someone with five minutes.

**Outcome.** The delta summary first. Flag anything that moved more than 10 points, and tell me if any source went stale or failed to refresh. The full scorecard underneath. Nothing goes to leadership until I've read it.

> **How you know it worked:** Ask yourself honestly how often these numbers change. If the answer is "not quarterly," change the cadence.

---

## 2. Content and editorial

**Sample file:** `02-Content-Brand-Voice-and-Posts.md`. Northwind Supply, an invented industrial fastener distributor with a four-sentence voice note and three published posts.

### Exercise 1: Research

*Attach 02-Content-Brand-Voice-and-Posts.md and paste this. Research doesn't need to be on for this one, because the evidence is in the file.*

**Context.** I am trying to get consistent writing out of Claude for Northwind Supply, an industrial fastener distributor. The attached file has our brand voice note and three published posts.

**Audience.** Maintenance engineers and procurement managers at mid-market manufacturers. They are technical, short on time, and allergic to marketing language.

**Scope.** Use only the attached posts as evidence of how we write. Do not invent house rules that are not in the material.

**Intent.** I need a usable style guide, because the one we have is four sentences long and hasn't been updated since 2021.

**Narrator.** Act as an editor who has read our published work and can describe what we actually do, as opposed to what we say we do.

**Outcome.** A style guide covering voice, sentence length, technical depth, terminology we use and avoid, and three worked before-and-after examples. Flag anything you had to guess at.

> **How you know it worked:** Read the flags. Anything it guessed at is a question for your team, not a rule.

### Exercise 2: Project

*Create a Project called [Northwind voice]. Add 02-Content-Brand-Voice-and-Posts.md and your Exercise 1 style guide. Paste this into the Project instructions.*

**Context.** This Project is how Northwind Supply writes. It holds our brand voice note, three published posts, and the style guide from Exercise 1.

**Audience.** Maintenance engineers and procurement managers at mid-market manufacturers. Technical, busy, and allergic to marketing language.

**Scope.** The published posts are the evidence of how we write. The voice note is what we say about ourselves. Where the two disagree, the posts win. Don't invent rules that aren't in this material.

**Intent.** Anything written in this Project should be publishable with light edits, not rewritten from scratch.

**Narrator.** Our senior editor, who has read everything we've published.

**Outcome.** No exclamation points. "Customers," never "clients." Measurements spelled out. Lead with the practical answer. When you're guessing at a rule, say so.

> **How you know it worked:** Ask for a 150-word post on why Northwind tells customers about substitutions. If it sounds like Post C without you pointing at it, the Project is working.

### Exercise 3: Artifact

*In the same Project, set Output to a document, then paste this.*

**Context.** Use the style guide and the three posts in this Project.

**Audience.** Freelance writers and new hires who have never read a Northwind post.

**Scope.** Only rules the material supports. Mark anything you inferred.

**Intent.** Replace the four-sentence voice note with something a writer can actually use.

**Narrator.** An editor who teaches by example.

**Outcome.** A one-page style guide: voice, sentence length, technical depth, words we use and avoid, and three before-and-after examples built from real sentences in the posts. It has to export to Word, because that's where the writers work.

> **How you know it worked:** Export it and open it. If it only works inside Claude, it isn't finished.

### Exercise 4: Skill

*Still in the Project, paste this.*

**Context.** Northwind has a style guide now. It's in this Project.

**Audience.** Anyone writing or editing for Northwind, including writers who have never seen the guide.

**Scope.** Editing, not writing from scratch. Change what breaks the guide and leave the rest alone.

**Intent.** Every draft should come back in our voice without anyone pasting the guide into a prompt.

**Narrator.** A careful copy editor who explains every change.

**Outcome.** A Skill called northwind-voice-edit. Given a draft, it returns the edited version, then a short list of each change and the rule behind it, then anything the guide doesn't cover. Test it on a paragraph that's badly off-voice (write one with three exclamation points and the word "revolutionary") and show me what it does.

> **How you know it worked:** Also test it on one of the published posts. It should change almost nothing.

### Exercise 5: Plugin

*Once the Skill passes both tests, paste this.*

**Context.** northwind-voice-edit works on drafts I didn't write, and leaves good copy alone.

**Audience.** The marketing team, our two freelancers, and the product managers who write the spec sheets.

**Scope.** The Skill, plus the style guide it depends on.

**Intent.** One voice across everyone who writes for us, without me reviewing every draft.

**Narrator.** A product manager writing for a stranger.

**Outcome.** A Plugin with a one-line description that says when to reach for it. Package the style guide in, so the Skill never runs without it. Add a short note on what it does badly: it can't check facts, and it will smooth out a technically correct sentence if nobody's watching.

> **How you know it worked:** Give it to someone who writes spec sheets. If they can't tell when to use it from the description alone, rewrite the description.

### Exercise 6: Scheduled task

*Create a scheduled task, set its model to Sonnet, and paste this as its instructions.*

**Context.** Our published posts, in [the folder or site section where they live], and the style guide in this Project.

**Audience.** Me, and our lead editor.

**Scope.** Posts published in the past week only. Every Monday morning.

**Intent.** I want to catch drift from our voice before it becomes the new normal.

**Narrator.** The same copy editor, reporting instead of editing.

**Outcome.** A short note: which posts drifted, the specific sentences, and the rule each one breaks. If nothing drifted, one line saying so. Don't edit anything that's already published.

> **How you know it worked:** If it flags the same thing three weeks running, the problem is the guide, not the writers.

---

## 3. Reporting and performance

**Sample file:** `03-Reporting-Channel-Performance-Data.csv (and 03-Reporting-Answer-Key.md, to check your work afterward)`. Five months of Northwind Supply channel performance, April to August 2026. Thirty rows.

### Exercise 1: Research

*Attach 03-Reporting-Channel-Performance-Data.csv and paste this. Leave 03-Reporting-Answer-Key.md closed until you've seen the answer.*

**Context.** The attached file has five months of channel performance for Northwind Supply, April through August 2026: sessions, engaged sessions, conversions, revenue and spend, by month and channel.

**Audience.** Our CEO, who has ten minutes and will ask one question: what do we do about it?

**Scope.** Only the attached data. Do not speculate about causes you cannot see in it.

**Intent.** I need to know which single trend in here matters most, and what I am recommending we do before the Q4 budget is set.

**Narrator.** Act as an analyst who leads with the conclusion and shows the arithmetic underneath it.

**Outcome.** The finding first, in one paragraph. Then the numbers that support it. Then what you would do about it and what it would cost. Show the paid search efficiency calculation (revenue divided by spend) for every month.

> **How you know it worked:** Now open 03-Reporting-Answer-Key.md. Did it lead with the same thing?

### Exercise 2: Project

*Create a Project called [Northwind channel reporting]. Add 03-Reporting-Channel-Performance-Data.csv and your Exercise 1 readout. Paste this into the Project instructions.*

**Context.** This Project is Northwind Supply's monthly channel reporting. It holds five months of performance by channel, April to August 2026, and the readout from Exercise 1.

**Audience.** Our CEO, who has ten minutes, and finance, who will check every number.

**Scope.** Only the data in this Project. Don't speculate about causes you can't see in it.

**Intent.** Every answer should end in what we do about it before the Q4 budget is set.

**Narrator.** An analyst who leads with the conclusion and shows the arithmetic underneath.

**Outcome.** Use these definitions every time. Paid search efficiency: Paid Search revenue divided by Paid Search spend. Engagement rate: engaged sessions divided by sessions. Conversion rate: conversions divided by sessions. Round money to the nearest thousand. Say when a trend rests on fewer than three months.

> **How you know it worked:** Ask "What's the one number the CEO needs this month?" If it answers with a number and the arithmetic behind it, the Project is working.

### Exercise 3: Artifact

*In the same Project, paste this.*

**Context.** The data and definitions in this Project.

**Audience.** The CEO, opening it on her own before the budget meeting.

**Scope.** April to August 2026, all six channels.

**Intent.** She needs to see, in under a minute, that we're paying for revenue we used to get for free.

**Narrator.** An analyst who builds for executives.

**Outcome.** An interactive dashboard. The finding in one sentence at the top. Sessions and revenue by channel over time. Paid search efficiency as its own chart, with the calculation visible, so finance can check it. A filter by channel.

> **How you know it worked:** Filter to Paid Search and check August's efficiency against your own arithmetic. It should be about 2.1.

### Exercise 4: Skill

*Still in the Project, paste this.*

**Context.** We just built the monthly readout by hand: the finding first, then the numbers, then the recommendation, using the definitions in this Project.

**Audience.** Whoever produces the monthly readout, including whoever covers for me.

**Scope.** Any month's channel data, in the same columns.

**Intent.** The same readout, with the same definitions, every month, without rebuilding the prompt.

**Narrator.** A reporting lead writing the runbook.

**Outcome.** A Skill called monthly-channel-readout. It takes the latest month's rows and returns: the one finding that matters most, the numbers behind it with the arithmetic shown, what changed from last month, and one recommendation with what it would cost. Put the metric definitions in the Skill itself. Then test it on April to July only, and show me the July readout.

> **How you know it worked:** A good July readout should already see paid search efficiency sliding. If it needs August to notice, the Skill is too timid.

### Exercise 5: Plugin

*Once the Skill has handled a month it hadn't seen, paste this.*

**Context.** monthly-channel-readout works on a month it hadn't seen.

**Audience.** Marketing and finance. Finance has to recognize the numbers as theirs.

**Scope.** The Skill and its metric definitions.

**Intent.** Marketing and finance reading the same numbers, calculated the same way.

**Narrator.** A product manager writing for a stranger.

**Outcome.** A Plugin with a one-line description that says when to reach for it. Add a short note on what it does badly: it only knows the channels in the file, it can't explain causes the data doesn't show, and it will treat a tracking change as a real trend unless someone tells it.

> **How you know it worked:** Show finance the definitions before anyone else installs it. If they'd calculate it differently, fix it now.

### Exercise 6: Scheduled task

*Create a scheduled task, set its model to Sonnet, and paste this as its instructions.*

**Context.** Run the monthly-channel-readout Skill on the newest export in [the folder or Drive location where it lands].

**Audience.** Me first. The CEO once I've read it.

**Scope.** Monthly, on the third business day, after the month has closed.

**Intent.** I want to walk into the month knowing what moved, without building the report.

**Narrator.** The same analyst, writing for someone with five minutes.

**Outcome.** The finding first. Flag it if paid search efficiency drops below 2.0, or any channel moves more than 15 percent month over month. If the export is missing or the columns have changed, tell me instead of running on partial data. Nothing goes to the CEO until I've read it.

> **How you know it worked:** The failure check is the line that matters. A report that runs quietly on half the data is worse than no report.

---

## 4. Process and documentation

**Sample file:** `04-Process-Onboarding-Notes.md (and 04-Process-Distributor-Accounts.csv, for Exercise 6)`. How Northwind Supply onboards a new distributor account, written down once by somebody who has since left.

### Exercise 1: Research

*Attach 04-Process-Onboarding-Notes.md and paste this.*

**Context.** The attached file is the only documentation we have for how Northwind Supply onboards a new distributor account. It was written by somebody who has left.

**Audience.** The person who inherits this process next month, and the manager deciding who should own it.

**Scope.** Work only from the attached notes. Where the notes are ambiguous, say so rather than resolving it for me.

**Intent.** I need a documented process good enough to hand to a new owner, and an honest list of what's broken in it.

**Narrator.** Act as an operations lead who has cleaned up processes like this before and knows which gaps cause the expensive failures.

**Outcome.** The process as a numbered sequence with an owner named for each step. Then a separate list of the failure points you found, ranked by what they would cost us. Then the three questions I need to answer before this can be finalized.

> **How you know it worked:** Count the steps with no owner. That number is the real finding.

### Exercise 2: Project

*Create a Project called [Distributor onboarding]. Add 04-Process-Onboarding-Notes.md and your Exercise 1 process. Paste this into the Project instructions.*

**Context.** This Project is the documentation for how Northwind Supply onboards a new distributor account. It holds the original notes, written by someone who has left, and the documented process from Exercise 1.

**Audience.** Tom Beckett, who owns this process as of October, and whoever runs it day to day.

**Scope.** The notes and the documented process. Where they disagree or are unclear, flag it. Don't resolve it for me.

**Intent.** Anything built here should make this process safe to hand to someone new.

**Narrator.** An operations lead who has cleaned up processes like this before.

**Outcome.** Always name an owner for every step, or say there isn't one. Keep the national and regional paths visible rather than blending them. Keep a running list of open questions.

> **How you know it worked:** Ask "Who owns the welcome email?" The right answer is "nobody yet." If the Project invents an owner, tighten Scope.

### Exercise 3: Artifact

*In the same Project, paste this.*

**Context.** The documented process in this Project.

**Audience.** Whoever sets up the next account, working through it step by step.

**Scope.** The process as documented. Mark any step where the owner is still undecided.

**Intent.** No account gets stuck at the tax certificate again, and no first order goes unnoticed.

**Narrator.** An operations lead building a tool, not a document.

**Outcome.** An interactive onboarding checklist. One row per step, with owner, typical time and a checkbox. The ERP setup step can't be ticked until the tax exemption certificate is. A day counter from ERP setup that turns red at 14 days with no first order. A toggle between the national and regional paths.

> **How you know it worked:** Try to tick ERP setup before the tax certificate. If it lets you, it isn't finished.

### Exercise 4: Skill

*Still in the Project, paste this.*

**Context.** We just turned messy onboarding notes into an owned, numbered process with its failure points.

**Audience.** Anyone in operations with a process that lives in someone's head or a stale document.

**Scope.** Any process described in rough notes. Work only from what's written.

**Intent.** I want every undocumented process we find turned into something ready to hand off, the same way every time.

**Narrator.** The operations lead, writing the method down.

**Outcome.** A Skill called process-from-notes. It returns the process as a numbered sequence with an owner for each step, the failure points ranked by what they'd cost, the questions someone has to answer before it's final, and a TRIPS read on which step is worth automating first. Test it on a different process you know, even one written in five lines.

> **How you know it worked:** Thin notes should produce a long list of open questions, not a confident-looking process.

### Exercise 5: Plugin

*Once the Skill has handled a second process, paste this.*

**Context.** process-from-notes works on a process it didn't see today.

**Audience.** The operations team, and any manager who inherits a process.

**Scope.** The Skill only.

**Intent.** Documentation stops depending on one person noticing it's missing.

**Narrator.** A product manager writing for a stranger.

**Outcome.** A Plugin with a one-line description that says when to reach for it. Add a short note on what it does badly: it can only document what's written down, and it will make thin notes look finished. The open-questions list is not optional.

> **How you know it worked:** If someone skips the open questions and ships the process, the Plugin did its job and the governance didn't.

### Exercise 6: Scheduled task

*Put 04-Process-Distributor-Accounts.csv in [the folder or Drive location the task can read]. Create a scheduled task, set its model to Sonnet, and paste this as its instructions.*

**Context.** 04-Process-Distributor-Accounts.csv lists every distributor account with its type, who set it up, setup date, whether the tax certificate is on file, and first order date. The onboarding process is in this Project.

**Audience.** Tom Beckett, who owns onboarding.

**Scope.** Every account with no first order yet, however old. Every Monday morning.

**Intent.** No account goes more than 14 days without a first order without someone knowing.

**Narrator.** An operations coordinator who keeps things moving without drama.

**Outcome.** A short list: every account past 14 days with no first order, days since setup, who set it up, and the next step from the process. Separately, any account missing a tax certificate. If nothing needs attention, one line saying so.

> **How you know it worked:** Run it once by hand today. Harbor Point Industrial should be at the top, and it's been waiting since May.

---

## 5. Meetings to actions

**Sample file:** `05-Meetings-Pipeline-Review-Transcript.md`. Northwind Supply's Q3 pipeline review on 14 September 2026. Four people, twenty minutes, five commitments.

### Exercise 1: Research

*Attach 05-Meetings-Pipeline-Review-Transcript.md and paste this.*

**Context.** The attached file is a transcript of our Q3 pipeline review, 14 September 2026, with four people present.

**Audience.** The four attendees, who will each get their own items and need no context beyond what was said.

**Scope.** Only commitments actually made in the transcript. Do not infer tasks that were discussed but not agreed.

**Intent.** I need every commitment captured with an owner and a date, so that nothing depends on somebody remembering.

**Narrator.** Act as a chief of staff who is careful about the difference between a decision and a discussion.

**Outcome.** A table of owner, commitment and due date. Then a short list of things that were raised but deliberately not assigned, so we can see what we chose to leave. Flag any commitment where the date was implied rather than stated.

> **How you know it worked:** Dana's summary at the end lists four items. If your table has more than five, it's turning discussion into tasks.

### Exercise 2: Project

*Create a Project called [Pipeline reviews]. Add 05-Meetings-Pipeline-Review-Transcript.md and your Exercise 1 table. Paste this into the Project instructions.*

**Context.** This Project holds Northwind Supply's pipeline review meetings, starting with the 14 September 2026 transcript, and the commitments table from Exercise 1.

**Audience.** The four regular attendees: Dana Whitfield (Sales), Marcus Reyes (Finance), Priya Raman (Marketing) and Tom Beckett (Operations).

**Scope.** Only what was said in the transcripts. A decision is something agreed. A discussion isn't.

**Intent.** Nothing agreed in these meetings should depend on someone remembering it.

**Narrator.** A chief of staff who is careful about the difference between a decision and a discussion.

**Outcome.** Show commitments as owner, commitment and due date. Flag dates that were implied rather than stated. Keep a running list of things raised but deliberately not assigned.

> **How you know it worked:** Ask "What did Marcus agree to?" It's a subtle one. Marcus agreed to work on Priya's traffic analysis. Reviewing Tom's buffer stock and getting Priya's data first are conditions he set for other people, not tasks he took on.

### Exercise 3: Artifact

*In the same Project, paste this.*

**Context.** The commitments table in this Project.

**Audience.** The four attendees, each checking their own items.

**Scope.** Commitments from the 14 September meeting.

**Intent.** Everyone can see what they owe and when, without a follow-up email thread.

**Narrator.** A chief of staff building a tracker.

**Outcome.** An interactive tracker: owner, commitment, due date, status, and whether the date was stated or implied. Filter by owner. Sort by due date. Overdue items in red. A second section for things raised but not assigned.

> **How you know it worked:** Filter to Tom. He should have two items, and the shipping model is due first.

### Exercise 4: Skill

*Still in the Project, paste this.*

**Context.** We just turned a meeting transcript into an owned list of commitments.

**Audience.** Anyone who runs or attends a recurring meeting.

**Scope.** Any meeting transcript. Only commitments actually made.

**Intent.** Every meeting ends with owners and dates, without anyone writing them up.

**Narrator.** A chief of staff, writing the method down.

**Outcome.** A Skill called meeting-to-actions. It returns a table of owner, commitment and due date; a list of things raised but not assigned; a flag on every implied date; a flag on any commitment with no owner; and a two-line summary of what was decided. Test it on a transcript from a meeting you were in, or a short made-up one.

> **How you know it worked:** The test that matters: does it leave a discussion as a discussion?

### Exercise 5: Plugin

*Once the Skill has handled a second transcript, paste this.*

**Context.** meeting-to-actions works on a transcript it hadn't seen.

**Audience.** Managers who run recurring meetings.

**Scope.** The Skill. If your transcripts live in a notetaker with a connector, include that connector.

**Intent.** Follow-up stops depending on whoever took notes.

**Narrator.** A product manager writing for a stranger.

**Outcome.** A Plugin with a one-line description that says when to reach for it. Add a short note on what it does badly: it can't tell a joke from a commitment, it only knows who said what if the transcript labels speakers, and it will miss anything agreed in the chat or after the call.

> **How you know it worked:** Hand it to a manager who wasn't at today's workshop. If the description doesn't tell them when to use it, rewrite it.

### Exercise 6: Scheduled task

*Create a scheduled task, set its model to Sonnet, and paste this as its instructions.*

**Context.** The commitments tracker in this Project.

**Audience.** The four attendees, through me.

**Scope.** Every Friday at noon. Commitments due in the next seven days, plus anything overdue.

**Intent.** Nothing slips because people forgot, and nobody has to chase.

**Narrator.** A chief of staff who is firm and never passive-aggressive.

**Outcome.** A short digest grouped by owner: what's due next week, what's overdue and by how long. Draft a one-line reminder for each owner for me to send. Don't send anything yourself.

> **How you know it worked:** "Don't send anything yourself" is the governance line. Keep it until you trust the output.
