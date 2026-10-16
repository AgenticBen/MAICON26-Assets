# **MAICON AI Data Analysis**

Thu, 15 Oct 26

#### **Workshop Overview: AI for Data Analysis**

* Session by Trust Insights at MAICON 2026, focused on repeatable AI-driven analytics  
* Core thesis: AI is bad at math but great at writing code; use Python (deterministic) instead of asking AI to calculate directly  
* Three problems addressed:  
  * Generative AI is probabilistic, not deterministic  
  * AI has domain blinders (defaults to Google Analytics when you say “marketing analytics”)  
  * Analytics reports get rebuilt from scratch every time

#### **Model and Prompting Strategy**

* Use large models on low effort for speed in workshops  
  * Opus 5.5 (low), GPT-6 Astro (light), Gemini 4 Argon (low), Qwen 3.8 (low)  
  * Smart model on low effort often beats dumb model on high effort (fewer tokens)  
* Five Keys framework for agentic prompting (Trust Insights):  
  * Purpose, People, Process, Platform, Performance  
  * Always define “done” explicitly; agentic models will infer their own definition otherwise  
  * Tell models what to do, not what not to do (“it’s not X, it’s Y”)

#### **Workshop Exercises**

* Exercise 1: Inventory what’s in the box  
  * Paste the “great big green prompt” into your LLM; it queries Python libraries available in that environment  
  * Output: list of 100-200+ Python libraries and an analytics enablement catalog by NAICS industry code  
  * Reveals hundreds of techniques (clustering, Gini coefficients, regression, etc.) without installing anything  
* Exercise 2: Run analysis on real data  
  * Data source: Google Search Console, Generative AI tab (pages \+ impressions CSV)  
  * Paste prompt 2 \+ CSV into the same chat; model asks clarifying questions, then runs analysis  
  * Example output for Christopher Penn’s site:  
    * AI/tool content: 10% of pages, 28% of impressions  
    * 7 pages \= 50% of impressions (Gini: 0.88, highly concentrated)  
    * Techniques borrowed from economics (Pareto/Lorenz), demography (content vintage cohorts), real estate (hedonic regression)  
    * Insight: AI citations have no correlation with organic search strategy

#### **Homework: Turn It Into a Repeatable Skill**

* Prompt 3 converts the one-time analysis into a reusable Claude skill  
  * Skill uses templates \+ Python code so future runs need far less AI reasoning  
  * Ask two questions, run the skill, get the report  
* Model downgrades once skill is built:  
  * Build with Opus/GPT-6 Astro; run ongoing with Sonnet 5 or GPT-6.1 Sol  
  * Even small models (GPT-6 Luna, Haiku) can run deterministic skills reliably  
* Goal: scheduled task that grabs new data monthly, runs the skill, produces the report automatically

#### **Post-Session: Slash Brag and Agentic App Building**

* Ben (note-taker) connected with two other attendees after the session  
* One attendee (Ben, AI consultant) demoed the /brag skill (GitHub repo):  
  * Points at any repo, database, or file; extracts the most impressive stats  
  * Generates a 20-second branded motion design video using Python audio/video libraries  
  * Chainable with a brand skill (logos, hex codes, positioning) for on-brand output  
  * Used for Iowa State research papers, a manufacturing quoting app, and a pub golf app  
* Agentic app discussion: the attendee builds hosted agentic orchestration apps (Vercel, free hosting)  
  * Includes CRM, billing/invoices, Stripe integration, auto-generated proposals via MCP  
  * Security note: anonymize sensitive client data; add 2FA and DNS-pointed internal hosting for private deployments  
  * SOC 2, HIPAA compliance relevant for enterprise use cases

#### **Next Steps**

* **Complete the homework prompt (Prompt 3\) to build a reusable analytics skill**  
  * Convert today's AI visibility analysis into a scheduled, repeatable Claude skill that runs monthly.  
* **Explore the /brag GitHub skill for content and social graphics use cases**  
  * High potential for reducing time spent on social graphics; pair with a brand skill once brand guidelines are documented.  
* **Follow up with Ben (the AI consultant met at the session)**  
  * Already have his email; explore scoping an agentic proposal-generation app for the Philadelphia conventions sales team.

