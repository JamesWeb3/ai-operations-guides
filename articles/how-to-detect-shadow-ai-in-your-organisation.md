---
title: "How to Detect Shadow AI in Your Organisation"
description: "Detect shadow AI by reading five signals you already hold: SaaS billing, network and DNS logs, browser telemetry, OAuth grants, and a staff survey."
date: 2026-09-10
keyword: "how to detect shadow ai in your organisation"
---

# How to Detect Shadow AI in Your Organisation

> Detecting shadow AI does not require new spyware or a forensic project. It means reading five signals your business already generates: expense and SaaS billing records, network and DNS logs, browser or endpoint telemetry, the OAuth and single sign-on grants staff have approved, and an honest anonymous survey. Each one surfaces a different slice of unsanctioned AI use, and no single one is complete, so the reliable method is to triangulate across all five. The point of finding shadow AI is not to punish it but to see what your people actually need, then pull that use into a sanctioned path where the data going into these tools can be governed. Across Sentry AI's own AIOS telemetry, 93,763 agent tool calls were logged in a single instrumented control plane over this period, 84,535 of them in the last 30 days across 115 distinct agents, which is the visibility standard you are trying to recreate for human AI use: every action carrying an identity and a timestamp.

The short answer: you detect shadow AI by combining five sources you already control. Pull the last three months of card and SaaS spend and search for AI vendor names. Query your DNS or firewall logs for traffic to known AI domains. Check browser or endpoint management for AI extensions and web apps. Review the OAuth grants staff have given third-party AI tools access to your Google Workspace or Microsoft 365. Then run a short, genuinely anonymous survey asking what people use. Cross-reference the five, because each catches what the others miss: billing finds paid tools, network logs find free web tools, and the survey finds the personal-device usage that never touches your systems at all.

The rest of this guide walks through each signal, what it catches and misses, how to read it under New Zealand and Australian privacy law, and what to do with what you find.

## Why detection comes before policy

Shadow AI is any use of artificial intelligence tools inside your business that leadership and IT have not sanctioned: a consultant summarising a client brief in a free chatbot, a salesperson running customer emails through a writing assistant, a developer pasting code into whichever model answers fastest. You cannot write a workable [shadow AI policy for your business](shadow-ai-policy-for-businesses.md) until you know what is actually in use, because a policy built on guesswork either bans tools people depend on or ignores the ones creating real exposure. Detection is the survey that makes the map accurate.

It is worth saying plainly that the goal is not surveillance. Most shadow AI is not malicious, it is unmet demand: staff found a tool useful faster than the organisation decided how to govern it. Detection done well is diagnostic, not disciplinary.

## The five signals, and what each one catches

### 1. Expense and SaaS billing records

Start here because it is the fastest and least intrusive. Pull the last three months of company card statements, expense claims and any SaaS management tool, and search for the obvious AI vendor names plus generic terms like "AI", "assistant", "copilot" and "GPT". This catches paid subscriptions, including the ones expensed as a personal productivity tool. It misses everything free, which is most of it, so treat billing as the floor of your estimate, never the ceiling.

### 2. Network and DNS logs

Your firewall, secure web gateway or DNS resolver already logs the domains devices on your network reach. Query them for traffic to known AI service domains over a representative fortnight. This is the single richest source for free web-based tools, because a staff member does not need to pay or install anything to trigger a DNS lookup. Its blind spots are traffic on mobile data rather than your network, and personal devices, which is exactly why the survey below is not optional.

### 3. Browser and endpoint telemetry

If you manage browsers or endpoints, you can enumerate installed AI extensions and frequently visited AI web apps. This catches the tools that live in the browser rather than as a subscription, and it tells you not just which tools but how heavily each is used, which matters when you decide what to sanction. It reaches only managed devices, so contractors and bring-your-own hardware sit outside it.

### 4. OAuth and single sign-on grants

The most overlooked signal. When staff "sign in with Google" or connect an AI tool to their Microsoft 365 mailbox or Google Drive, they create an OAuth grant your admin console lists. Reviewing those grants shows which third-party AI services have been given standing access to company data, which is a sharper risk than a one-off paste because the access persists. This is where a tool quietly reading a shared drive shows up, and it is directly relevant to the data residency questions New Zealand and Australian buyers ask most.

### 5. An anonymous staff survey

The four technical signals all share one gap: they cannot see a person typing a customer's details into a chatbot on their own phone. Only asking closes it. A short, credibly anonymous survey ("which AI tools help you at work, and what do you use them for") consistently surfaces usage no log captured, provided people believe the answer will not be used against them. Pair it with an amnesty: the aim is the map, not a list of names.

## Score your detection coverage

Tick the signals you can read today. The tool restates which slice of shadow AI each one covers and where your blind spots remain. Nothing leaves your browser.

<div class="aog-tool" id="aog-sai">
  <label><input type="checkbox" id="aog-sai-bill" checked> Expense and SaaS billing review</label><br>
  <label><input type="checkbox" id="aog-sai-net" checked> Network or DNS logs</label><br>
  <label><input type="checkbox" id="aog-sai-brow"> Browser or endpoint telemetry</label><br>
  <label><input type="checkbox" id="aog-sai-oauth"> OAuth and single sign-on grant review</label><br>
  <label><input type="checkbox" id="aog-sai-survey"> Anonymous staff survey</label>
  <output id="aog-sai-out" for="aog-sai-bill aog-sai-net aog-sai-brow aog-sai-oauth aog-sai-survey"></output>
  <small>Five signals triangulate: billing finds paid tools, network logs find free web tools, the survey finds personal-device use. No single signal is complete.</small>
</div>
<script>
(function () {
  var ids = ['bill', 'net', 'brow', 'oauth', 'survey'];
  var labels = {
    bill: 'paid subscriptions',
    net: 'free web tools on your network',
    brow: 'browser extensions on managed devices',
    oauth: 'standing third-party access to company data',
    survey: 'personal-device use no log can see'
  };
  var out = document.getElementById('aog-sai-out');
  function box(id) { return document.getElementById('aog-sai-' + id); }
  function render() {
    var have = ids.filter(function (id) { return box(id).checked; });
    var miss = ids.filter(function (id) { return !box(id).checked; });
    var msg = have.length + ' of 5 signals in place. Covered: ' + (have.length ? have.map(function (id) { return labels[id]; }).join('; ') : 'none') + '.';
    if (miss.length) {
      msg += ' Blind spots: ' + miss.map(function (id) { return labels[id]; }).join('; ') + '.';
    } else {
      msg += ' Full coverage across all five signals.';
    }
    out.textContent = msg;
  }
  ids.forEach(function (id) { box(id).addEventListener('change', render); });
  render();
})();
</script>

## Reading the results under NZ and Australian privacy law

Detection itself has a legal frame. In New Zealand, monitoring staff network activity is lawful where it is reasonable and staff are informed, and the Privacy Act 2020 governs how you handle any personal information you gather in the process. In Australia, the Privacy Act 1988 and the Australian Privacy Principles apply the same way, and several states regulate workplace surveillance directly. The practical rule on both sides of the Tasman is to be transparent that you monitor for security and governance, aggregate wherever you can, and resist the temptation to turn a governance exercise into individual performance management. The moment staff believe detection is a trap, your best signal, the survey, goes dark.

The privacy stakes are also why detection matters in the first place. Every unsanctioned tool that receives customer or staff data is a disclosure your existing obligations already cover, whether or not you authorised it.

## What our own operations data shows

The visibility you are reconstructing for human AI use is the same visibility a governed automated system has by default. Across Sentry AI's own AIOS telemetry for this period, 93,763 agent tool calls were logged through a single instrumented control plane, 84,535 of them in the last 30 days, spanning 115 distinct agents and 41 distinct tools. Every one of those calls carries an identity, a timestamp and an outcome, which is precisely what shadow AI lacks: use with no record. The gap between 93,763 fully logged automated actions and an unknown number of unlogged human ones is the gap detection exists to close. You will never instrument human AI use to that standard, but the five signals above get you from zero visibility to a defensible estimate.

## From detection to a governed path

Detection is a snapshot, and shadow AI regenerates the moment a new tool launches, so the finding has to feed a system rather than a one-off report. What you learn becomes the approved-tools list in your policy, and the recurring detection sweep (quarterly is sensible) becomes evidence for a wider governance programme. If you are weighing which framework to build toward, our comparison of the [NIST AI Risk Management Framework and ISO 42001](nist-ai-rmf-vs-iso-42001.md) sets out the two main routes, and the detection log you build is exactly the kind of artefact an auditor expects. Detection is also the cheapest layer to stand up, and our breakdown of [how much AI governance costs for mid-sized businesses](how-much-does-ai-governance-cost-for-mid-sized-businesses.md) shows where it sits in the total spend. For businesses that want a structured read of their exposure before committing to any framework, a scoped [AI opportunity and risk audit](https://sentrysolutions.ai/ai-opportunity-audit) is the usual starting point.

## FAQ

### What is shadow AI, and how is it different from agent sprawl?

Shadow AI is unsanctioned use of AI tools by people, such as staff pasting company data into a free chatbot. Agent sprawl is the related problem of too many AI agents and automations proliferating without central oversight. Detection techniques overlap: both are ultimately about knowing what AI is running in your business and under whose authority. Shadow AI is the human-driven slice, agent sprawl the automated one.

### Can you detect shadow AI without monitoring staff?

Partly. Billing records and OAuth grants are administrative reviews that involve no active monitoring at all. Network logs and endpoint telemetry are monitoring, and require you to have informed staff that you do it. The survey involves no monitoring but depends on trust. In practice a proportionate mix, transparent monitoring for security plus an anonymous survey, detects most shadow AI without turning into surveillance.

### Is shadow AI a privacy risk under the New Zealand Privacy Act?

Yes. The moment a staff member enters personal information into an unsanctioned tool, the Privacy Act 2020 applies exactly as it would to any other handling of that data, including the principles on security, disclosure and offshore transfer. Because most consumer AI tools process data overseas by default, undetected shadow AI is a live cross-border disclosure risk, which is why detection is a privacy control and not just an IT tidiness exercise.

### How does detecting shadow AI relate to ISO 42001?

ISO 42001, the AI management system standard, expects an organisation to know and control the AI it uses. A repeatable detection process and the register it produces are direct evidence toward that requirement, so the sweep you run for operational reasons doubles as certification groundwork. Detection is the input; the management system is what you build on top of it.

### How often should we run detection?

Quarterly at minimum, aligned with the review cadence of your approved-tools list. The AI tool market changes monthly, so an annual sweep is obsolete long before it repeats. A light quarterly pass across the five signals keeps the picture current enough to trust.

Shadow AI is not, at root, a security failure to be hunted down. It is a demand signal your organisation has not yet answered, and detection is how you read it accurately before you decide what to sanction. The businesses that handle it well treat the first sweep not as an audit of what people did wrong, but as the clearest map they will ever get of the capability their staff already want to use.

*Published by [Sentry AI](https://sentrysolutions.ai) — Auckland, New Zealand.*
