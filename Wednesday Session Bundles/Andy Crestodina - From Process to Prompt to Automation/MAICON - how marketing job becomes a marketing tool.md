# **MAICON \- how marketing job becomes a marketing tool**

Wed, 14 Oct 26

#### **The Evolution: Prompts to Assistants to Tools**

* Andy Crestodina’s MAICON presentation on AI-powered marketing tools  
* Three-stage evolution for marketers:  
  1. Prompts: tested, reusable, saved, shared into a prompt library  
  2. Assistants: Claude projects, custom GPTs, Copilot agents combining multiple prompts into sequences  
  3. Tools: purpose-built applications that carry the thinking farther and run autonomously

#### **Building Tools Without Technical Skills**

* Core insight: “The hottest new programming language is English” (Andrej Karpathy)  
* If you can describe a thing, AI will build it  
* Framework for defining a tool upfront (from Christopher Penn):  
  * Goals: what is this for, why are we building it  
  * Inputs: what data goes in  
  * Outputs: what forms, alerts, reports come out  
  * Specs: training data, examples, UX, data sources  
* Key mindset shift: have a conversation about what to build, don’t just give detailed instructions  
  * Ask “what should we do next?” rather than dictating every step  
  * The Bitter Lesson (Sutton, 2019): AI performs best when given open-ended problems, not rigid rules

#### **Three Tools Built and Demonstrated**

* CRO Bot: conversion rate optimization tool  
  * Input: a URL  
  * Steps: builds persona, audits page, constructs wireframe, extracts design standards, outputs a mockup  
  * Two modes: human-in-the-loop (step-by-step review) or one-shot (full build)  
  * Supports mobile/desktop/tablet toggle, inline editing via prompting, and “explain this” feature per page block  
  * Honest limitations: no CMS connection, no SEO, no analytics, no accessibility check; useful as a conversion hypothesis  
* Buyer Signals Monitor: voice-of-customer intelligence from sales calls  
  * Ingests call transcripts automatically (Mondays and Thursdays)  
  * Surfaces weighted themes from actual buyer language, not sales rep recollection  
  * Tracks technology signals: which tools buyers mention and their relative popularity over time  
* Lead Enrichment \+ Sales Coach: bridges marketing and sales  
  * Clay enriches inbound leads with company size, revenue, industry, business model  
  * Enriched lead pushed to Slack as a full mini-playbook for the sales rep  
  * Sales Coach tool trained on past calls and best practices  
    * Rep can practice on a real enriched lead with multiple buyer personas  
    * Scores calls, flags weaknesses (e.g. too much talking, poor listening)  
    * Suggests responses to prospect emails based on 400+ calls and persona data  
    * Includes a fitness-tracker-style progress view

#### **How Long It Actually Takes**

* Sales Coach build: 7 hours, 62 prompts  
* Build report breakdown:  
  * \~33% strategy and direction  
  * \~51% waiting (walk the dog, call your mom, build another tool)  
  * Remainder on UX, which matters for adoption  
* Estimated pre-AI equivalent: 5-7 people, 4-6 months, \~\$500K  
* “One-shotting” is not a flex: great tools take iteration, not a single prompt  
* 24-hour rule: sleep on what you built before showing anyone

#### **Architecture, Skills, and Mindset**

* Data architecture matters: build tools that pull from shared data lakes, not isolated buckets  
  * Sources: sales call transcripts, CRM, analytics  
  * Multiple tools should draw from the same central rivers  
* Skills that matter most going forward:  
  * Domain expertise  
  * Framing and prioritization  
  * First-party data judgment  
* Good words for 2027: architecture, orchestration, process, repo  
* Bad words for 2027: tool scroll, shelfware, Frankenstack, data swamp  
* Closing thesis: process \+ tools \= system; the marketer’s job is now to build systems that drive measurable outcomes

