# **MAICON \- 5 deadly sins of AI Agents**

Thu, 15 Oct 26

#### **The 5 Deadly Sins of AI Agents**

1. **The double agent**: agent works for you but also leaks your data to others  
   * CMO example: customer segments entered into an agent were allegedly used by competitors to target the same customers  
2. **The skeleton key**: giving agents login credentials opens access far beyond the intended task  
   * CMO example: agent with CRM login drafted emails to all 40,000 customers, not just the trade show list  
3. **The guest who never leaves**: agents keep live connections after the task ends  
   * CMO example: campaign agent left connected after Q3 spent \$60,000 in Q4 before anyone noticed  
4. **The empty chair**: C-suite not actively using the technology  
   * Data from Wokme (SAP): companies 5.2x more successful when C-suite actively used and shared results  
5. **No witness**: no verification of who authorized the agent to act  
   * Analogy: a hole-in-one requires a witness signature; agents need the same accountability layer

#### **Building the Agent: Four Steps**

* **Brain**: document every step a human takes to do the job; 10-step process built in Claude with detailed instructions  
* **Context**: define voice, audience, sponsor priorities, banned words, and “insider facts” (e.g., guests who teach vs. guests who pitch)  
  * Corrections fed back as reusable rules so the agent learns over time  
  * Example: agent wrote “boost open rate by 40%”; corrected to reflect the actual 10% to 14% move  
* **Connectors**: link the tools the agent needs (Riverside, Google Sheets, Brevo, Libsyn)  
  * Hardest part of the build; Brevo blocked the agent and required a call with their API team  
  * Riverside MCP connection would have raised the plan from \$60 to \$360/month; switched to Claude’s native connector instead  
* **Autopilot**: triggers (e.g., procurement list over \$50k) or scheduled timing (e.g., every Monday at 8am)  
  * Human-in-the-loop approval gates at key steps  
  * Named outputs and a full activity log for auditability

#### **Results and the Future: Agent-to-Agent**

* Results after \~3 months running the podcast agent:  
  * Prep time: 9 hours down to 3 hours  
  * Guest booking: 4 weeks down to 2 hours  
  * Newsletter open rate: 10% up to 14%  
  * Won 5 marketing podcast awards  
* Future direction: agent-to-agent negotiation with no human involvement  
  * Demo showed one agent requesting calendar access and negotiating topic and time with a guest’s agent  
  * Privacy-focused: only the agreed topic and time are surfaced to humans; negotiation data stays in the “data bubble”  
  * Only \~11% of people currently running agents at this level  
  * Audience skepticism noted: agent-to-agent feels natural for B2B or product sales, but more personal for podcast guest relationships

