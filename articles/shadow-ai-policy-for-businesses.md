---
title: "Shadow AI Policy for Businesses: What to Put in It and How to Enforce It"
description: "A shadow AI policy sets which AI tools staff may use, what data is off-limits, and who approves exceptions. Here is what to include and how to enforce it."
date: 2026-09-09
keyword: "shadow ai policy for businesses"
---

# Shadow AI Policy for Businesses: What to Put in It and How to Enforce It

> A shadow AI policy is the document that tells your staff which AI tools they may use at work, what company and customer data may never be pasted into them, and who signs off when someone needs an exception. For a New Zealand or Australian business it has to do three things: name an approved list of tools, draw a hard line around personal and confidential data under the Privacy Act, and route anything outside the list through a named approver rather than a blanket ban that staff quietly ignore. A ban on its own does not work, because the tools are free and already on everyone's phone. The policies that hold up are the ones paired with an approval path, so the safe option is also the easy one. Across Sentry AI's own agent operations, 127 of 82,910 logged tool calls were held for explicit human approval before anything ran, which is the same control a workforce policy needs: a gate, not a wall.

The short answer: a shadow AI policy should list the AI tools staff are approved to use, state plainly that customer records, employee data, financial information and anything else personal or confidential must not be entered into any unapproved tool, and give people a fast, named route to get a new tool approved. Pair it with light technical controls (a sanctioned tool that is genuinely good, plus network or browser visibility into what is being used) so that following the policy is easier than going around it. A policy that only says "do not use ChatGPT" produces more shadow AI, not less, because the need does not go away and the usage simply goes underground.

The rest of this guide sets out the clauses a workable policy contains, the New Zealand and Australian legal backdrop that shapes them, how to enforce it without pretending you can block everything, and where a shadow AI policy sits inside a wider governance programme.

## What shadow AI actually is, and why a ban makes it worse

Shadow AI is any use of artificial intelligence tools inside your business that IT and leadership have not sanctioned: a consultant pasting a client brief into a free chatbot to summarise it, a salesperson running customer emails through a writing assistant, a developer piping code into whichever model answers fastest. It is the direct descendant of shadow IT, and it spreads faster because the tools are free, need no installation, and produce obviously useful results in seconds.

The instinct is to ban it. That instinct is the problem. A flat ban does not remove the pressure that created the behaviour (people are busy and the tool saves them real time), so the usage continues on personal devices and personal accounts where you have zero visibility and zero control. You have not reduced the risk, you have blinded yourself to it. The goal of a shadow AI policy is not to stamp out AI use. It is to pull that use into the light, where the data going into these tools can be governed.

## What a shadow AI policy must contain

A policy staff will actually follow is short, specific, and names people rather than committees. At minimum it covers:

1. **An approved tools list.** The named AI services staff may use for work, and for what. "Our licensed Microsoft Copilot for document drafting; our internal assistant for customer data; this specific vendor for code." A short allow-list beats a long block-list, because block-lists are always out of date.
2. **A data classification line.** The single most important clause. State explicitly which categories of data may never enter an unapproved tool: personal information about customers or staff, health information, financial records, anything under NDA, and source code or trade secrets. Tie it to your existing data classification if you have one.
3. **An exceptions and approval route.** Who a staff member asks when they want to use a tool that is not on the list, and how fast they will get an answer. If the answer takes two weeks, people will not wait. Name the approver and set a service level (for example, a response within two working days).
4. **Accountability and consequences.** Who owns the policy, how breaches are handled, and the fact that the employee remains responsible for the output (AI does not transfer liability).
5. **A review cadence.** AI tools change monthly. A policy reviewed once a year is obsolete by March. Commit to a quarterly review of the approved list.

## The New Zealand and Australian legal backdrop

A shadow AI policy is not an abstract tidiness exercise. In both countries, existing privacy law already governs what happens when staff feed data into these tools, whether or not you have written anything down.

In New Zealand, the Privacy Act 2020 applies to personal information the moment a staff member enters it into an AI tool, exactly as it applies to any other handling of that information. Information Privacy Principle 5 requires you to keep personal information secure, and Principle 11 limits disclosure: pasting a customer's details into a third-party tool whose terms allow it to train on that input is a disclosure you probably did not authorise. Principle 12 adds obligations around sending personal information offshore, which most consumer AI tools do by default.

In Australia, the Privacy Act 1988 and the Australian Privacy Principles impose parallel duties, with APP 6 (use and disclosure), APP 8 (cross-border disclosure) and APP 11 (security) all directly engaged when staff use unsanctioned tools. The Act's reforms have sharpened enforcement and penalties, which raises the cost of finding out about shadow AI through an incident rather than a policy.

Neither regime has a specific "AI law" that changes this: it is your existing privacy obligations, applied to a new channel. If your business also touches the European market, the rules tighten further, as our guide to [EU AI Act compliance for New Zealand businesses](eu-ai-act-compliance-for-new-zealand-businesses.md) explains. The practical upshot is the same on both sides of the Tasman: the data line in your policy is not optional, it is how you meet obligations you already have.

## Enforcement: a gate, not a wall

The hard part is not writing the policy, it is making it real. Three layers do most of the work, and none of them is a firewall rule alone.

**Give people a genuinely good sanctioned option.** The reason staff reach for a free chatbot is that it works. If the approved tool is slower, clunkier or locked down to uselessness, the policy loses to convenience every time. The first enforcement measure is a sanctioned tool worth using.

**Make the safe path the easy path.** An approval route that is fast and visible means people use it. An approval route that is slow and buried means they route around it. This is the same design principle that governs automated systems: the strongest control is not blocking an action, it is requiring a quick human sign-off before a sensitive one proceeds, so the default is safe without being frozen.

**Get visibility, then coach.** Browser and network tooling can show you which AI services are in use across the business, and our guide on [how to detect shadow AI in your organisation](how-to-detect-shadow-ai-in-your-organisation.md) sets out the five signals to read before you write the approved list. The point of that visibility is not to punish, it is to find out what people actually need and fold the genuinely useful tools into the approved list. Most shadow AI is not malicious, it is unmet demand.

### What our own operations data shows about approval gates

The case for a gate over a wall is one we can put numbers to from our own systems rather than a vendor survey. Across Sentry AI's own automated agent operations, the telemetry for this period looks like this:

| Metric | Count |
| --- | --- |
| Logged agent tool calls | 82,910 |
| Automated runs | 875 |
| Actions held for explicit human approval before running | 127 |

In other words, roughly one action in every 650 was routed to a person for sign-off before it executed, while the rest proceeded automatically. That is the exact shape a workforce shadow AI policy should take: the overwhelming majority of AI use flows freely through sanctioned tools, and a small, well-defined set of sensitive actions stops at a human gate. A policy that tried to gate everything would be ignored; one that gates nothing is not a policy at all. The ratio is the design.

## Where a shadow AI policy sits in the bigger picture

A shadow AI policy is the staff-facing, day-one layer of AI governance: it is the thing you can publish this month. Underneath it sits the question of how your organisation governs AI as a system, which is where formal frameworks come in. If you are weighing which framework to build toward, our comparison of the [NIST AI Risk Management Framework and ISO 42001](nist-ai-rmf-vs-iso-42001.md) sets out the two main options, and for companies selling into enterprise our guide to [ISO 42001 versus SOC 2 for AI companies](iso-42001-vs-soc-2-for-ai-companies.md) shows how a shadow AI policy becomes evidence toward a certifiable management system rather than a standalone document. A good policy is not throwaway: the approved list, the data line and the approval log are precisely the artefacts an ISO 42001 auditor expects to see, so writing one well now is groundwork for certification later. The policy is also the cheapest layer of a wider programme, and our breakdown of [how much AI governance costs for mid-sized businesses](how-much-does-ai-governance-cost-for-mid-sized-businesses.md) shows where it sits in the total. For businesses that want to map their current exposure before committing to any of this, a structured [AI opportunity and risk audit](https://sentrysolutions.ai/ai-opportunity-audit) is the usual starting point.

## FAQ

### Should a shadow AI policy ban tools like ChatGPT outright?

Generally no. A blanket ban drives usage onto personal devices where you have no visibility, so you carry the same risk with less control. The more effective approach is to provide a sanctioned tool that is genuinely useful, define clearly what data may never go into any unapproved tool, and offer a fast route to approve new tools. Ban specific tools only where there is a concrete, documented reason.

### What is the single most important clause in a shadow AI policy?

The data line: an explicit statement of which categories of information (customer records, staff data, health and financial information, confidential and contractual material, source code) must never be entered into an unapproved AI tool. Everything else in the policy supports that one rule, because it is the clause that maps directly to your Privacy Act obligations.

### Does New Zealand or Australian law require us to have a shadow AI policy?

Neither country mandates a shadow AI policy by name, but both the Privacy Act 2020 (NZ) and the Privacy Act 1988 (Australia) already require you to keep personal information secure and to control its disclosure, including offshore. A shadow AI policy is how you meet those existing duties in practice, and its absence is what an investigation will note after an incident.

### How often should we review the approved tools list?

Quarterly at minimum. The AI tool market changes far faster than an annual policy cycle, and an approved list that is a year old will either block tools staff now rely on or miss tools that have since become risky. A short quarterly review keeps the allow-list current enough that people trust it.

### Who should own the shadow AI policy?

A named person, not a committee: usually whoever owns information security or operations, with input from legal or privacy. The policy should say who that is, because an unowned policy is never reviewed and never enforced. In smaller businesses this is often the same person who owns the wider AI governance programme.

Shadow AI is not going away, and it is not, at root, a discipline problem. It is a sign that your staff have found AI genuinely useful faster than your organisation has decided how to govern it. The businesses that come out ahead are the ones that read that signal correctly: they treat the policy not as a fence around a dangerous thing, but as the map of a capability their people already want to use well.

*Published by [Sentry AI](https://sentrysolutions.ai) — Auckland, New Zealand.*
