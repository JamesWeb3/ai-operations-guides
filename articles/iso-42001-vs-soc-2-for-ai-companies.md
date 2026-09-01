---
title: "ISO 42001 vs SOC 2 for AI Companies: Which One Do You Need?"
description: "ISO 42001 governs how your AI is built and overseen; SOC 2 attests your data controls. AI companies selling to enterprise usually end up needing both."
date: 2026-09-01
keyword: "iso 42001 vs soc 2 for ai companies"
---

# ISO 42001 vs SOC 2 for AI Companies: Which One Do You Need?

> ISO 42001 and SOC 2 answer two different buyer questions, so for an AI company they are not competitors, they are a sequence. SOC 2 is an attestation that you protect the data and systems you run: security, availability and confidentiality, audited by a CPA firm and issued as a report. ISO 42001 is a certificate that you govern the AI itself: risk assessment, human oversight, transparency and traceability, issued by an accredited body against the first management-system standard written for artificial intelligence. Most AI companies selling into enterprise or government end up needing both, because a procurement team asks for SOC 2 to trust your infrastructure and increasingly asks for ISO 42001 to trust your models. The good news is that roughly two thirds of the evidence overlaps, so the second one is far cheaper than the first.

If a customer has asked which standard you need, the short answer is SOC 2 first if your buyers are US-centric or asking today, ISO 42001 first if your differentiator is the AI itself and your buyers are in the EU, government or regulated sectors, and both within eighteen months if you sell to enterprise on either side of the Tasman. They cover different ground, they do not substitute for each other, and the controls that pass one build most of the evidence for the other. This guide sets out what each proves, where they overlap, and how a New Zealand or Australian AI company should sequence them.

## What SOC 2 actually is

SOC 2 is an attestation report defined by the American Institute of CPAs (AICPA). An independent CPA firm examines your controls against the Trust Services Criteria: security (always in scope), and optionally availability, processing integrity, confidentiality and privacy. The output is not a certificate you can frame, it is a report a customer's security team reads under NDA. A Type I report describes your controls at a point in time. A Type II report, the one enterprise buyers actually want, tests that those controls operated over a period, usually three to twelve months. SOC 2 is about how you protect data and keep systems running. It says nothing specific about whether your AI is fair, explainable or overseen, because that is not what it was written to measure.

## What ISO 42001 actually is

ISO/IEC 42001, published in December 2023, is the first certifiable management-system standard for artificial intelligence. It asks you to build and run an Artificial Intelligence Management System (AIMS): a set of policies, roles, risk assessments and controls around the AI you develop or deploy. Its Annex A controls are AI-specific in a way SOC 2 is not: AI system impact assessment, data governance for training and inference, human oversight of consequential decisions, logging and traceability, and transparency to the people your AI affects. It is issued by an accredited certification body, valid for three years, and carries an annual surveillance audit. It sits in the same family as ISO 27001 and shares its structure, which matters for cost. If you want the full breakdown, see our guide on [how much ISO 42001 certification costs](how-much-does-iso-42001-certification-cost.md).

## The overlap, and why the second one is cheaper

The two standards were written by different bodies, but the controls a modern AI company needs sit in the middle of both. Access control, change management, logging, incident response, risk assessment and vendor management all appear in a SOC 2 examination and in an ISO 42001 audit. If you have done one properly, you have already built the machinery the other reuses: the policies, the owners, the review cadence and the audit trail. What does not transfer is the AI-specific half of ISO 42001 (impact assessments, model transparency, human oversight of automated decisions) and the CPA-attestation format of SOC 2. Companies that hold one report reach the other by closing gaps rather than starting over, which is why the order you choose is a budgeting decision, not just a compliance one.

| | SOC 2 | ISO 42001 |
| --- | --- | --- |
| What it proves | You protect data and keep systems running | You govern how AI is built and overseen |
| Governing body | AICPA (US) | ISO/IEC (international) |
| Output | Attestation report (Type I or Type II) | Certificate, valid three years |
| Assessed by | CPA firm | Accredited certification body |
| Core focus | Security, availability, confidentiality | AI risk, human oversight, transparency, traceability |
| Buyers who ask for it | US enterprise, SaaS procurement | EU, government, regulated, AI-specific buyers |
| Renewal | Annual Type II report | Annual surveillance, three-year recertification |

## Which one an AI company should get first

The right sequence depends on who is asking and why. Use the situation, not the acronym, to decide.

| Your situation | Start with | Why |
| --- | --- | --- |
| US enterprise buyers, SaaS sales motion, asked in a security questionnaire | SOC 2 Type II | It is the procurement default your buyers already know how to read |
| Your product is the AI, and buyers are in the EU, government or regulated sectors | ISO 42001 | It proves the thing that is actually novel and risky about what you sell |
| You sell to large enterprise on either side of the Tasman | Both, SOC 2 then ISO 42001 | Enterprise procurement increasingly asks for infrastructure and AI governance separately |
| Early stage, one or two pilot customers, limited budget | Whichever your first serious buyer names | Do not certify ahead of demand; let the first real contract set the order |

## What passing either one really tests

Strip away the framework language and both audits converge on the same unglamorous question: can you show, for any consequential thing your system did, what happened and that a human held the reins where it mattered. That is measurable, not aspirational. Across Sentry AI's own agent operations over the 90 days to 1 September 2026, 558 autonomous runs were written to an append-only audit trail of 19,984 recorded steps, and 112 high-impact actions were held at a human approval gate before they executed. That combination, complete traceability plus evidence that human oversight is a gate the system passes through rather than a line in a policy, is exactly what a SOC 2 examiner tests for security and what an ISO 42001 auditor tests for AI governance. An AI company that builds logging and a human approval gate into the product from the start satisfies the hardest part of both standards at once. One that bolts governance on afterwards pays for it twice.

## The New Zealand and Australia angle

Neither standard is a local law, but both interlock with the privacy regimes you already operate under. In New Zealand the Privacy Act 2020 governs how you collect, use and disclose personal information, and its cross-border and data-residency rules (real questions your buyers do search for) are exactly what a SOC 2 confidentiality scope and an ISO 42001 data-governance control document. In Australia the Privacy Act and the Australian Privacy Principles play the same role, with reforms tightening the treatment of automated decisions. For a local AI company, SOC 2 gives an enterprise buyer a familiar security artefact, while ISO 42001 gives assurance on the AI-specific risk that privacy regulators on both sides of the Tasman are moving toward. The market-specific detail, including how the standard maps onto local privacy law and what certification costs here, is in our guides on [ISO 42001 certification for New Zealand businesses](iso-42001-certification-for-new-zealand-businesses.md) and [ISO 42001 certification for Australian businesses](iso-42001-certification-for-australian-businesses.md).

## FAQ

### Do AI companies need both ISO 42001 and SOC 2?

Usually, eventually, if they sell to enterprise or government. They prove different things: SOC 2 that you protect data and infrastructure, ISO 42001 that you govern the AI itself. Neither substitutes for the other, so a buyer that cares about both will ask for both. The saving is that the controls overlap heavily, so the second one is far cheaper to reach than the first.

### Is SOC 2 or ISO 42001 better for a startup selling AI?

Neither is better in the abstract; the better one is whichever your first serious buyer asks for. US-centric SaaS buyers name SOC 2 in their security questionnaires by reflex. Buyers in the EU, government or regulated sectors, and buyers whose concern is the AI itself, increasingly name ISO 42001. Do not certify ahead of demand: let the first real contract decide the order.

### Does ISO 42001 cover data residency?

Indirectly. Data residency is a data-governance and confidentiality concern, and ISO 42001's data-governance controls plus a SOC 2 confidentiality scope are where you document how and where training and inference data is stored and moved. Your underlying obligation still comes from the Privacy Act 2020 in New Zealand or the Australian Privacy Principles; the standards give you the audited evidence that you meet it.

### Does SOC 2 cover the AI model itself?

Not specifically. SOC 2 tests the security, availability and confidentiality of the systems that run your AI, not whether the model is fair, explainable or subject to human oversight. Those are ISO 42001 questions. This is the single clearest reason the two do not substitute for each other: a clean SOC 2 report tells a buyer nothing about how you govern the AI's behaviour.

### How long does each take?

A SOC 2 Type II needs an observation window, usually three to twelve months of controls operating, plus the examination itself. ISO 42001 runs four to twelve months for a small-to-mid organisation depending on how much of your AI is already logged and governed. Because the two share most of their evidence, sequencing them back to back is far faster than treating them as two separate projects.

## Where to start

The honest first move is the same for both standards: a gap analysis against your actual systems, because it turns two abstract frameworks into one costed work list and shows how much of the evidence you already hold. AI companies that already treat their deployments as governed operations, with owners, logging and a human oversight loop, tend to find both audits mostly formalise what they already do. Those running AI as ungoverned tooling pay to build the governance first, and pay for it in both currencies. If you want that gap assessed against your specific systems before committing to an auditor or a certification body, an [AI opportunity and governance audit](https://sentrysolutions.ai/ai-opportunity-audit) is the fastest way to see which standard to start with and what it will take to pass. The framework you choose first matters less than building the logging and oversight both of them test, because that is the evidence that carries from one report to the next.

*Published by [Sentry AI](https://sentrysolutions.ai) — Auckland, New Zealand.*
