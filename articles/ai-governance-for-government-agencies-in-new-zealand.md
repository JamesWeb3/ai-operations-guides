---
title: "AI Governance for Government Agencies in New Zealand: What the Public Sector Has to Build"
description: "New Zealand government agencies govern AI through the Algorithm Charter, the Privacy Act 2020, the OIA and NZISM, with ISO 42001 added when a tender needs proof."
date: 2026-09-22
keyword: "ai governance for government agencies in new zealand"
---

# AI Governance for Government Agencies in New Zealand: What the Public Sector Has to Build

> A New Zealand government agency does not govern AI with one policy: it assembles a stack of instruments it is already bound by. The base is the law and public-sector commitments that apply by default, chiefly the Privacy Act 2020, the Official Information Act 1982, the Public Records Act 2005 and the Algorithm Charter for Aotearoa New Zealand. The operating layer is an internal framework, usually the NIST AI Risk Management Framework, run against the security controls in the NZISM and the Protective Security Requirements. The proof layer, added for a tender or an inter-agency data share, is certification against ISO/IEC 42001. Two controls run through all three: log every AI action, and put a human on every consequential decision. Across Sentry AI's own AIOS telemetry, more than 129,000 agent tool calls have been written to an immutable audit log and 132 sensitive actions were held for explicit human approval before they ran, which is the shape of the evidence a public-sector AI system has to be able to produce on request.

For a New Zealand government agency, AI governance is the discipline of making the duties you already carry apply to automated decisions. Start with the instruments that bind the public sector by default: the Privacy Act 2020 for personal information, the Official Information Act 1982 for the public's right to ask how a decision was made, the Public Records Act 2005 for keeping the record of it, and the Algorithm Charter for Aotearoa New Zealand for the transparency and human-oversight commitments an agency has signed. Run an internal framework over the top, align it to the New Zealand Information Security Manual (NZISM) and the Protective Security Requirements (PSR), and reach for ISO/IEC 42001 only when another party needs proof they can verify. The rest of this guide explains why the public-sector context changes the order, and what each layer asks of an agency.

## Why the public sector carries more than a private business

A private company using AI answers mainly to the Privacy Act and its own customers. An agency answers to the public, and that difference loads the base layer. The Official Information Act 1982 means a person can ask how an automated system reached a decision that affected them, and the agency has to be able to answer, which is impossible without a record of what the model saw and did. The Public Records Act 2005 requires that record to be kept and disposed of properly, so an AI system that leaves no durable trail is a records-management failure before it is a governance one. The Algorithm Charter for Aotearoa New Zealand, signed by most large agencies, commits signatories to transparency about how algorithms inform decisions, to human oversight of significant ones, and to considering Te Ao Māori perspectives in their design.

Layered on top are the security instruments. The NZISM sets the baseline for how government information is protected, and the PSR governs the wider protective-security posture, including where information may be hosted and how third-party providers are assured. An agency cannot adopt an offshore AI tool the way a small business can: the hosting location, the data classification and the provider's assurances all have to clear those frameworks first. This is why "ai data residency" is one of the governance queries we see most often from this market. For an agency it is not a preference, it is a control.

## Māori Data Sovereignty is not optional context

The instrument that has no private-sector equivalent is Māori Data Sovereignty. Data about, from or affecting Māori carries obligations grounded in Te Tiriti o Waitangi and articulated by frameworks such as those from Te Kāhui Raraunga and the Data Iwi Leaders Group. For an AI system, that means governance has to account for who holds the data, who decides how it is used, and whether an automated inference about Māori individuals or communities is one an agency has the standing to make. The Algorithm Charter points at this directly. Treating it as a late compliance check rather than a design input is the most common way a public-sector AI project has to be rebuilt, because the question of authority over the data cannot be retrofitted once the system is running on it.

## The three layers, in order

Think of the framework as three layers, each producing the evidence the next one reuses.

| Layer | What it is | The question it answers | Cost |
| --- | --- | --- | --- |
| Legal and charter base | Privacy Act 2020, OIA, Public Records Act, Algorithm Charter, NZISM, PSR | What am I already bound to do as an agency? | None, it applies by default |
| Operating framework | NIST AI RMF (Govern, Map, Measure, Manage) run against NZISM controls | How do I organise the ongoing work? | Free to adopt |
| Proof | ISO/IEC 42001 certification | How do I prove it to another agency or a tenderer? | Implementation plus audit fees |

The order matters because skipping it wastes public money. Mapping AI use against the Privacy Act and classifying the data under NZISM produces the inventory the NIST Map function needs. Running the NIST functions produces the operating evidence an ISO 42001 auditor asks to see. An agency that jumps to certification before the base and operating layers run pays for an audit it is not ready to pass. Our guide to the [AI governance framework for New Zealand businesses](ai-governance-framework-for-new-zealand-businesses.md) sets out the same three-layer logic for the private sector, and the public-sector version simply carries a heavier base layer.

## Run the operating framework with logging and a human gate

The operating layer is where daily governance lives, and the NIST AI RMF is the pragmatic choice because it is free, detailed and technology-neutral. Its four functions map cleanly onto public-sector duties: Govern (policy, named accountable owners, the Algorithm Charter commitments), Map (an inventory of every AI system in use, including tools staff adopted without asking), Measure (the logging and testing that make an OIA response possible), and Manage (deciding what to treat, tolerate or avoid). The first move under Map is almost always an inventory, because an agency cannot govern AI it has not found. When you operationalise these functions in software, our guide to the [best AI governance platform for New Zealand businesses](best-ai-governance-platform-for-new-zealand-businesses.md) covers what the tooling actually has to do, and the requirements for an agency are stricter on audit logging and access control.

Two controls carry disproportionate weight for the public sector: complete logging of what each AI system did, and a human approval gate on consequential decisions. These are the two the Algorithm Charter names, the two the OIA depends on, and the two an ISO 42001 auditor will look for first.

## The demand signal in our own data

The reason to build this now is that the answers are already being searched for and barely met. Across Sentry AI's own Search Console data for the ninety days to 22 September 2026, more than twenty distinct queries naming ISO/IEC 42001 drew over 140 impressions with zero clicks, at an average position around the sixth or seventh page, while governance queries such as "ai governance services nz", "ai data residency" and "ai readiness assessment new zealand" surfaced repeatedly and ranked well outside the first page. The pattern is consistent: New Zealand buyers, public and private, are reaching for governance answers by name and the first page is not answering them. Alongside that external signal sits our own operating evidence. Across Sentry AI's AIOS telemetry, more than 129,000 agent tool calls have been captured to an immutable audit log and 132 sensitive actions were routed to a human for explicit approval before running, across 2,919 automated agent runs. That ratio, near-total logging with a deliberate human gate on the consequential few, is exactly the operating shape a public-sector AI governance framework is meant to produce.

## Which layer is your agency ready for?

Use your situation, not the acronym. The selector below maps where an agency is onto which layer to work on next. Every outcome restates the sequence set out above.

<div class="aog-tool" id="aog-govnz">
  <label for="aog-govnz-base">Have you mapped your AI use against the Privacy Act, the OIA and NZISM, including Māori data considerations and where data is hosted?</label>
  <select id="aog-govnz-base"><option value="0" selected>Not yet</option><option value="1">Yes</option></select>
  <label for="aog-govnz-run">Have you stood up an operating framework: named owners, an AI inventory, complete logging and a human approval gate on consequential decisions?</label>
  <select id="aog-govnz-run"><option value="none" selected>Not really</option><option value="some">Some of it</option><option value="most">Most or all of it</option></select>
  <label for="aog-govnz-ask">Is another agency, a tender or a data-share partner asking you to prove AI governance with a certificate right now?</label>
  <select id="aog-govnz-ask"><option value="0" selected>No, not yet</option><option value="1">Yes</option></select>
  <output id="aog-govnz-out" for="aog-govnz-base aog-govnz-run aog-govnz-ask"></output>
  <small>Indicative guidance against the three layers in this guide, not an audit.</small>
</div>
<script>
(function () {
  var base = document.getElementById('aog-govnz-base'),
      run = document.getElementById('aog-govnz-run'),
      ask = document.getElementById('aog-govnz-ask'),
      out = document.getElementById('aog-govnz-out');
  function render() {
    var msg;
    if (base.value === '0') {
      msg = 'Start at the base: map your AI use against the Privacy Act 2020, the OIA and NZISM, and settle who holds authority over any Maori data, before building anything on top.';
    } else if (run.value !== 'most') {
      msg = 'Work the operating layer: run the NIST AI RMF to stand up owners, an AI inventory, complete logging and a human oversight gate. It is free and builds the evidence any later audit or OIA response reuses.';
    } else if (ask.value === '1') {
      msg = 'Move to the proof layer: your governance already runs and someone wants verification, so ISO 42001 certification mostly formalises what you do.';
    } else {
      msg = 'Keep running the framework: you are close to ISO 42001 audit-ready and can certify the moment a tender or data-share partner asks. Certifying ahead of demand spends public money early for no gain.';
    }
    out.textContent = msg;
  }
  [base, run, ask].forEach(function (el) { el.addEventListener('input', render); el.addEventListener('change', render); });
  render();
})();
</script>

## FAQ

### Is AI regulated for government agencies in New Zealand?

Not by a dedicated AI law. New Zealand has no AI-specific statute. For agencies the obligations come from instruments that already apply: the Privacy Act 2020 for personal information, the Official Information Act 1982 for the public's right to understand decisions, the Public Records Act 2005 for keeping the record, and the Algorithm Charter for Aotearoa New Zealand for transparency and human oversight of significant algorithmic decisions. A governance framework is how an agency meets those distributed duties deliberately.

### What is the Algorithm Charter for Aotearoa New Zealand?

It is a voluntary commitment most large public-sector agencies have signed, setting out how they will use algorithms responsibly: being transparent about how algorithms inform decisions, providing human oversight of significant ones, guarding against unintended bias, and considering Te Ao Māori perspectives. It is not legally binding on its own, but it sets the public-sector expectation an agency will be measured against, and it maps closely onto the controls in a formal AI management system.

### Where can a government agency store AI data?

There is no single mandated location, but the constraints are real. The Privacy Act's information privacy principle 12 restricts sending personal information overseas without comparable safeguards, and the NZISM and PSR govern how classified government information is hosted and how offshore providers are assured. In practice that means an agency assesses data classification, hosting location and provider assurances together before adopting an AI tool, which is why "AI data residency" is a recurring public-sector governance question rather than a preference.

### How does Māori Data Sovereignty affect a government AI project?

Data about or affecting Māori carries obligations grounded in Te Tiriti o Waitangi and articulated by Māori data governance frameworks. For an AI system that means deciding who holds the data, who governs its use, and whether an automated inference about Māori individuals or communities is one the agency has the standing to make. It is a design input, not a late compliance check, because authority over the data cannot be retrofitted once a system is already running on it.

### Do agencies need ISO 42001?

Not until someone asks for proof. ISO/IEC 42001 is the first international AI management-system standard, and certification by an accredited body converts internal governance into something another agency or a tenderer can verify. Run the framework now for its own sake, and certify when an all-of-government tender, a data-share partner or a regulator wants assurance they can check. Our guide to [ISO 42001 certification for New Zealand businesses](iso-42001-certification-for-new-zealand-businesses.md) sets out the JAS-ANZ route and the indicative fees.

## Where to start

The honest first move is a gap analysis of your agency's actual AI systems against the three layers, because it turns an abstract set of duties into one costed work list and shows which layer you are on. Agencies that already treat AI as governed operations, with named owners, complete logging and a human on the consequential decisions, tend to find the framework formalises what they do and any later certificate is a short step rather than a rebuild. The public sector has a quiet advantage: the Privacy Act, the OIA and the Public Records Act have already trained agencies to think about who touches information, who can ask about a decision, and how the record is kept, so the distance to a working AI management system is often shorter than it looks. If you want that gap assessed against your specific systems, an [AI opportunity and governance audit](https://sentrysolutions.ai/ai-opportunity-audit) is the fastest way to see which layer to work on before committing budget. The framework is not the hard part: the discipline it tests, logging every AI action and putting a human on the consequential ones, is what makes every governance step after it a formality.

*Published by [Sentry AI](https://sentrysolutions.ai) — Auckland, New Zealand.*
