---
title: "NIST AI RMF vs ISO 42001: Which AI Governance Framework Do You Need?"
description: "The NIST AI RMF is a free framework you run; ISO 42001 is a certificate an auditor issues. Most businesses run the framework first, then certify."
date: 2026-09-08
keyword: "nist ai rmf vs iso 42001"
---

# NIST AI RMF vs ISO 42001: Which AI Governance Framework Do You Need?

> The NIST AI Risk Management Framework and ISO/IEC 42001 are not competitors, they are two stages of the same work. The NIST AI RMF is a free, voluntary framework you use to organise AI risk into four functions (Govern, Map, Measure, Manage); ISO 42001 is a certifiable management-system standard an accredited body audits you against and issues a certificate for. You cannot be certified against the NIST framework, and the ISO standard is not a step-by-step method. Most businesses run the NIST AI RMF first because it is free and immediate, then pursue ISO 42001 once a buyer, tender or regulator asks for external proof. The work done under the framework becomes most of the evidence the audit needs, so the order is a budgeting decision, not a fork in the road.

If someone has asked which one you need, the short answer is: start with the NIST AI RMF if you want to stand up AI governance now at no licence cost, and add ISO 42001 when a customer, government tender or regulator asks for an independent certificate rather than your own word. They operate at different levels. NIST gives you the framework to run; ISO 42001 gives you the certificate that proves the framework demonstrably runs. Neither substitutes for the other, and because the framework produces the operating evidence the certificate is audited on, doing the NIST work first makes the ISO work cheaper. This guide sets out what each one is, where they overlap, how they map onto New Zealand and Australian obligations, and how to tell which stage you are at.

## What the NIST AI RMF is

NIST released AI RMF 1.0 on 26 January 2023. It is a voluntary, technology-neutral framework, not a law and not a certification. It organises AI risk work into four functions: Govern (the cross-cutting culture, policy and accountability layer), Map (context: what the system is for and who it affects, which for AI already in unofficial use starts with [how to detect shadow AI in your organisation](how-to-detect-shadow-ai-in-your-organisation.md)), Measure (analysing and tracking risks with evidence such as logging and testing), and Manage (deciding what to treat, tolerate or avoid, and responding when things change). NIST also publishes a free Playbook of suggested actions and a Generative AI Profile added in July 2024. Because it costs nothing to adopt and any organisation can use it, it is the most common practical starting point for AI governance. The Govern function's policy layer is also where a staff-facing [shadow AI policy for businesses](shadow-ai-policy-for-businesses.md) lives: the document that controls which AI tools employees may use and what data they may put into them. The full breakdown of the four functions is in our guide to [the NIST AI Risk Management Framework](nist-ai-risk-management-framework-for-australian-businesses.md).

## What ISO 42001 is

ISO/IEC 42001, published in December 2023, is the first certifiable management-system standard written for artificial intelligence. It asks you to build and operate an Artificial Intelligence Management System (AIMS): policies, roles, risk assessments and Annex A controls covering AI system impact assessment, data governance, human oversight of consequential decisions, logging and traceability, and transparency to affected people. It sits in the same family as ISO 27001 and shares its structure. Crucially, it is issued by an accredited certification body, valid for three years with an annual surveillance audit. That external issuance is the whole point: it converts your internal governance into an artefact a buyer or auditor can trust without taking your word for it. What that certificate costs and how the audit runs is covered in our guide to [ISO 42001 certification for New Zealand businesses](iso-42001-certification-for-new-zealand-businesses.md).

## The core difference in one line

A framework is something you run; a standard is something you are certified against. The NIST AI RMF tells you how to organise the work. ISO 42001 tells you what an auditor will check and gives you a certificate when you pass. This is why the phrase "NIST AI RMF vs ISO 42001" is slightly misleading: for most businesses the honest answer is both, in sequence, because the framework is the method and the certificate is the proof.

| | NIST AI RMF | ISO/IEC 42001 |
| --- | --- | --- |
| What it is | Voluntary risk-management framework | Certifiable management-system standard |
| Governing body | NIST (US) | ISO/IEC (international) |
| Cost to adopt | Free | Implementation plus certification-body fees |
| Output | An internal way of working | A certificate, valid three years |
| Assessed by | Nobody: you self-apply | Accredited certification body |
| Structure | Four functions: Govern, Map, Measure, Manage | Management system plus Annex A controls |
| Best for | Standing up governance now, at no licence cost | Proving governance to buyers, tenders, regulators |
| Renewal | Ongoing internal review | Annual surveillance, three-year recertification |

## How the two map onto each other

The four NIST functions line up closely with the ISO 42001 management-system controls, which is why work under one is rarely wasted on the other. Govern maps onto the leadership, policy and roles clauses. Map maps onto AI system impact assessment and scoping. Measure maps onto the logging, testing and performance controls in Annex A. Manage maps onto risk treatment, human oversight and incident response. A business that has genuinely stood up all four NIST functions has already built most of the AIMS an ISO 42001 auditor asks to see; the certificate then formalises what already runs rather than starting a new project. If your buyers also ask for the US SOC 2 attestation, the different question that answers is set out in [ISO 42001 vs SOC 2 for AI companies](iso-42001-vs-soc-2-for-ai-companies.md).

## The demand signal in our own data

The market is searching for these answers faster than trustworthy ones are being published. Across Sentry AI's own Search Console data for the ninety days to 8 September 2026, queries naming ISO 42001 (including "iso/iec 42001", "iso 42001 certification" and "iso standards for ai") drew 126 impressions and zero clicks, at an average position past the sixth page of results. Demand for the certifiable standard is real and almost entirely unmet on the first page, while queries naming the NIST framework barely register locally yet: buyers reach for the certificate by name and back into the framework once they learn it is the way to earn it. For a New Zealand or Australian business, that gap is the reason to run the framework quietly now and be ready to certify when the demand reaches you. Running the framework is the managed-programme tier in our breakdown of [how much AI governance costs for mid-sized businesses](how-much-does-ai-governance-cost-for-mid-sized-businesses.md), with certification the layer added on top when a buyer asks.

## Which one to start with

The right first move depends on who is asking and why. Use the situation, not the acronym.

<div class="aog-tool" id="aog-rmf42">
  <label for="aog-rmf42-ask">Is anyone (a buyer, tender or regulator) asking you to prove AI governance with a certificate right now?</label>
  <select id="aog-rmf42-ask"><option value="cert" selected>No, not yet</option><option value="proof">Yes, they want independent proof</option></select>
  <label for="aog-rmf42-stage">Have you stood up governance internally: named owners, an AI inventory, logging and a human approval gate?</label>
  <select id="aog-rmf42-stage"><option value="none" selected>Not really</option><option value="some">Some of it</option><option value="most">Most or all of it</option></select>
  <output id="aog-rmf42-out" for="aog-rmf42-ask aog-rmf42-stage"></output>
  <small>Indicative guidance against the sequence in this guide, not an audit.</small>
</div>
<script>
(function () {
  var ask = document.getElementById('aog-rmf42-ask'),
      stage = document.getElementById('aog-rmf42-stage'),
      out = document.getElementById('aog-rmf42-out');
  function render() {
    var msg;
    if (ask.value === 'proof' && stage.value === 'most') {
      msg = 'Start ISO 42001: someone wants proof and your governance already runs, so certification mostly formalises what you do.';
    } else if (ask.value === 'proof') {
      msg = 'Run the NIST AI RMF to close the gaps first, then move straight to ISO 42001, because the certificate is audited on evidence you do not yet fully produce.';
    } else if (stage.value === 'most') {
      msg = 'Keep running the NIST AI RMF; you are close to ISO 42001 audit-ready and can certify the moment a buyer asks.';
    } else {
      msg = 'Start with the NIST AI RMF: it is free, immediate, and builds the evidence any future ISO 42001 audit will reuse.';
    }
    out.textContent = msg;
  }
  [ask, stage].forEach(function (el) { el.addEventListener('input', render); el.addEventListener('change', render); });
  render();
})();
</script>

## The New Zealand and Australia angle

Neither instrument is local law, but both sit against the regimes you already operate under. In New Zealand the Privacy Act 2020 governs personal information, and its cross-border and data-residency rules are exactly what the NIST Map and Manage functions document and what an ISO 42001 data-governance control evidences. In Australia the Privacy Act and the Australian Privacy Principles play the same role, and the Voluntary AI Safety Standard published in 2024 uses ten guardrails that pair naturally with the NIST framework as the "how". ISO 42001 certification here is issued through a body accredited by JAS-ANZ, the Joint Accreditation System of Australia and New Zealand. The practical read is the same on both sides of the Tasman: use the free framework to organise the work, and reach for the certificate when a tender or enterprise buyer wants assurance they can verify.

## FAQ

### Is ISO 42001 the same as the NIST AI RMF?

No. The NIST AI RMF is a free, voluntary framework you apply yourself to organise AI risk into four functions. ISO/IEC 42001 is a certifiable management-system standard an accredited body audits you against and issues a certificate for. They cover much of the same ground, but one is a method you run and the other is external proof that you run it.

### Do I need ISO 42001 certification, or is the NIST AI RMF enough?

The NIST framework is enough to govern your AI well internally. It is not enough when a buyer, government tender or regulator wants independent proof, because you cannot be certified against it. At that point ISO 42001 is the certificate that carries the assurance. Do not certify ahead of demand: run the framework now and certify when someone asks for the proof.

### Can I use the NIST AI RMF and ISO 42001 together?

Yes, and most organisations should. The four NIST functions produce the operating evidence an ISO 42001 audit reuses, so running the framework first makes the certification cheaper and faster. They are complementary stages, not alternatives.

### Which AI governance framework should a New Zealand business use?

Start with the NIST AI RMF because it is free, detailed and technology-neutral, then certify to ISO 42001 through a JAS-ANZ accredited body when a buyer or tender requires it. Both map onto the Privacy Act 2020, so the governance work is not wasted whichever way your obligations develop. For how the two sit alongside the local law as a single stack, see our guide to the [AI governance framework for New Zealand businesses](ai-governance-framework-for-new-zealand-businesses.md).

### Is either one legally required?

Neither the NIST AI RMF nor ISO 42001 is law in New Zealand or Australia. Both are voluntary. Their force comes from procurement and trust: enterprise and government buyers increasingly ask suppliers to show a recognised AI risk process, and a certificate is the strongest form of that answer.

## Where to start

The honest first move is a gap analysis of your actual AI systems against the four NIST functions, because it turns two abstract instruments into one costed work list and shows how much ISO 42001 evidence you already hold. Businesses that already treat their AI as governed operations, with named owners, logging and a human oversight loop, tend to find the framework formalises what they do and the certificate is a short move rather than a rebuild. If you want that gap assessed against your specific systems before choosing a certification body, an [AI opportunity and governance audit](https://sentrysolutions.ai/ai-opportunity-audit) is the fastest way to see which stage you are at and what certifying would take. The framework versus standard question matters far less than the discipline both of them test: build the logging and the oversight gate once, and every governance step after it, framework or certificate, is a formality.

*Published by [Sentry AI](https://sentrysolutions.ai) — Auckland, New Zealand.*
