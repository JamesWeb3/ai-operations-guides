---
title: "AI Governance for Law Firms: What Practices Have to Build"
description: "Law firms govern AI on duties they already carry (confidentiality, privilege, conduct rules, the Privacy Act), then NIST AI RMF, then ISO 42001."
date: 2026-09-24
keyword: "ai governance for law firms"
---

# AI Governance for Law Firms: What Practices Have to Build

> AI governance for a law firm is not a new rulebook you buy: it is the duties you already owe your clients and the court, extended to cover the models. A firm in New Zealand or Australia already answers to its conduct rules for confidentiality, competence and supervision, to legal professional privilege for anything a client tells it, and to the Privacy Act for personal information. AI governance is how you keep those duties intact when a model, rather than a lawyer, drafts, summarises or screens. The practical build is three layers: the professional and legal duties you are already bound by, then the NIST AI Risk Management Framework as your operating method, then ISO/IEC 42001 certification when a corporate client, government panel or insurer wants proof they can check. What makes a law firm different from a generic business is privilege: information put into the wrong tool can breach confidence and risk waiving the privilege that protects your client, so human oversight and a logged, traceable trail are not extras, they are the control.

For a law firm, the direct answer is to govern AI as an extension of the professional obligations you already carry, not as a separate technology project. Map each AI use against the duties that already bind you: confidentiality and legal professional privilege (any tool that reads client matter material), the conduct rules on competence and supervision (anything producing work a lawyer is responsible for), and the Privacy Act (any model touching personal information, including its cross-border transfer). Then run the NIST AI RMF to organise the ongoing work, and certify against ISO/IEC 42001 when someone wants independent assurance. The order matters, because each layer produces the evidence the next one reuses.

## Why a law firm is a different governance problem

A generic business governing AI has one hard external duty, the Privacy Act, and a lot of discretion about the rest. A law firm does not have that discretion, because two of its core duties are stricter than anything a general business carries. The first is confidentiality: a solicitor's duty of confidence, set out in New Zealand under the Lawyers and Conveyancers Act 2006 conduct rules and in Australia under the Legal Profession Uniform Law and the Solicitors' Conduct Rules, covers everything a client tells the firm, indefinitely. The second is legal professional privilege, which protects that information from compelled disclosure but can be lost if the firm handles it carelessly. Feed privileged material into a consumer AI tool that trains on its inputs, and you have arguably disclosed it to a third party, which is exactly the kind of act that puts confidence and privilege at risk.

That reframes the whole exercise. In an ordinary business, AI governance is a good idea you adopt to win tenders. In a law firm it is the same duty of confidence you already owe, applied to a new place where client information can leak. The firms that struggle treat a drafting assistant or a document-review model as outside their professional obligations. The firms that cope treat every tool that touches a matter as an extension of the file, with the same confidentiality, supervision and record-keeping the file already demands. The same discipline shows up on the front line of intake: our guide to [how much an AI voice agent costs for law firms](how-much-does-an-ai-voice-agent-cost-for-law-firms.md) shows that confidentiality and conflict screening, not the AI, are what drive the real cost and the real risk.

## The duties that will actually be tested

Four obligations shape the work, and knowing which one bites tells you what to prioritise.

| Duty or instrument | What it governs | Where AI touches it |
| --- | --- | --- |
| Confidentiality (conduct rules) | All client information, held indefinitely | Any tool reading, storing or transmitting matter material |
| Legal professional privilege | Protection of client communications from disclosure | Feeding privileged content to third-party or training-on-input models |
| Competence and supervision (conduct rules) | Quality of work and responsibility for it | Drafting, research and review a lawyer signs off but a model produced |
| Privacy Act (NZ 2020 / AU 1988) | Personal information and cross-border transfer | Any model trained on or reading personal data, especially offshore |

The supervision duty is the one lawyers underrate. A model that invents a case citation, and there are now multiple reported instances of lawyers filing AI-generated authorities that do not exist, does not carry a practising certificate: the lawyer who signed the document does. Several courts in New Zealand and Australia have issued guidance on generative AI use in litigation, and the common thread is that the practitioner remains responsible for verifying everything and, in some jurisdictions, for disclosing that AI was used. Governance is how a firm makes that verification a standing control rather than a matter of individual habit.

## The three layers, for a law firm

The layered model that works for any business still holds here, but the base layer is heavier. Our general [AI governance framework for New Zealand businesses](ai-governance-framework-for-new-zealand-businesses.md) sets out the stack; a law firm loads more into the bottom of it.

The professional base is the duties above, and unlike a generic business you cannot defer them: they apply to the first matter you touch. The operating layer is the NIST AI RMF, whose four functions (Govern, Map, Measure, Manage) map cleanly onto the risk discipline a firm already runs for conflicts and file management, so adopting it is usually a matter of extending existing registers rather than building new ones. The proof layer is ISO/IEC 42001, whose Annex A controls (data governance, human oversight of consequential decisions, logging and traceability, transparency to affected people) read almost like a list a professional-standards body would write. What certification involves in this country, and the JAS-ANZ accreditation route, is covered in our guide to [ISO 42001 certification for New Zealand businesses](iso-42001-certification-for-new-zealand-businesses.md).

## Human oversight is the control that carries the weight

Across legal work, the recurring requirement is that a lawyer remains accountable for what leaves the firm: the advice, the filed document, the drafted contract. AI does not remove that accountability, it concentrates it, because a model can repeat the same contestable output across dozens of matters before anyone notices. Governance in a firm therefore rests on two mechanical controls: log every material AI action so it can be reconstructed, and gate the consequential ones behind a person who can say no.

This is where our own operating data speaks to the point. Across Sentry AI's own AI operations telemetry, our autonomous agents ran 1,255 routine runs and logged 51,344 individual steps in the ninety days to 24 September 2026, and every action classed as higher-impact was held at a human approval gate before it could run. Across that gate's history a person has declined 30 of the 134 requests it has received, close to one in five. The number that matters is not the volume of automation, it is that a real oversight gate refuses a meaningful share of what reaches it. For a firm, that is the difference between an AI control that exists in a policy and one that demonstrably changes what gets sent to a client or a court, which is exactly what a professional-standards review or an ISO 42001 auditor is looking to see.

## Data residency and the offshore-model problem

Almost every capable AI model a law firm would use is hosted offshore, which puts cross-border transfer in the middle of the design. New Zealand's information privacy principle 12 (and the Australian Privacy Principles' equivalent) does not forbid sending personal information overseas, but it requires comparable safeguards when you do, and "AI data residency" is one of the most persistent governance queries we see from local businesses. For a firm the stakes are higher because the data is client information subject to confidence and privilege, not just personal data. The governance answer is to document each cross-border flow, tie it to a contractual safeguard, choose tools that do not train on your inputs, and be able to show a client or a regulator where matter information goes and under what protection, rather than discovering it during a complaint.

## An AI governance readiness check for law firms

The selector below maps where your firm sits onto which layer of the stack to work on next. Every outcome restates the sequence in this guide; it is indicative, not an audit.

<div class="aog-tool" id="aog-lawgov">
  <label for="aog-lawgov-base">Have you mapped each AI use against confidentiality, privilege, the supervision rule and the Privacy Act, including where matter data goes offshore?</label>
  <select id="aog-lawgov-base"><option value="0" selected>Not yet</option><option value="1">Yes</option></select>
  <label for="aog-lawgov-run">Have you stood up an operating framework: an AI inventory, named accountable owners, logging of material AI actions, and a human sign-off gate on anything leaving the firm?</label>
  <select id="aog-lawgov-run"><option value="none" selected>Not really</option><option value="some">Some of it</option><option value="most">Most or all of it</option></select>
  <label for="aog-lawgov-ask">Is a corporate client, government panel or professional indemnity insurer asking you to prove your AI governance right now?</label>
  <select id="aog-lawgov-ask"><option value="0" selected>No, not yet</option><option value="1">Yes</option></select>
  <output id="aog-lawgov-out" for="aog-lawgov-base aog-lawgov-run aog-lawgov-ask"></output>
  <small>Indicative guidance against the three layers in this guide, not legal or regulatory advice.</small>
</div>
<script>
(function () {
  var base = document.getElementById('aog-lawgov-base'),
      run = document.getElementById('aog-lawgov-run'),
      ask = document.getElementById('aog-lawgov-ask'),
      out = document.getElementById('aog-lawgov-out');
  function render() {
    var msg;
    if (base.value === '0') {
      msg = 'Start at the professional base: map every AI use against confidentiality, legal professional privilege, the supervision rule and the Privacy Act, especially where matter data goes to an offshore model. In a law firm these duties apply to the first matter you touch, so this layer cannot be deferred.';
    } else if (run.value !== 'most') {
      msg = 'Work the operating layer: run the NIST AI RMF to extend your conflict and file-management registers with an AI inventory, accountable owners, logging of material actions and a human sign-off gate on anything leaving the firm. It reuses discipline you already run.';
    } else if (ask.value === '1') {
      msg = 'Move to the proof layer: your governance already operates, and a client, panel or insurer wants verification, so ISO 42001 certification mostly formalises what you do and gives them something independent to rely on.';
    } else {
      msg = 'Keep running the framework: you are close to ISO 42001 audit-ready and can certify the moment a client, panel or insurer asks. Certifying ahead of that demand spends money early for no gain.';
    }
    out.textContent = msg;
  }
  [base, run, ask].forEach(function (el) { el.addEventListener('input', render); el.addEventListener('change', render); });
  render();
})();
</script>

## FAQ

### Is AI regulated for law firms in New Zealand and Australia?

Not by a dedicated AI law. Neither country has an AI-specific statute for legal practice, so AI in a firm is governed by the duties that already apply: confidentiality and legal professional privilege, the conduct rules on competence and supervision, and the Privacy Act. Courts in both countries have also issued generative-AI guidance for litigation. A governance framework is how you meet those distributed duties deliberately instead of hoping they never surface in a complaint.

### Can we put client or privileged information into an AI tool?

Only into one you can show protects it. The risk is that a consumer tool which trains on its inputs, or retains them without safeguards, amounts to disclosure to a third party, which can breach confidence and put privilege at risk. Governance means choosing tools that do not train on your data, documenting where matter information goes, and keeping privileged material out of anything you cannot control. This is the same discipline that drives cost in client-facing tools such as an intake voice agent.

### Do we need ISO 42001, or are our conduct-rule obligations enough?

Your conduct duties are the base, but they were not written for models. ISO/IEC 42001 adds the AI-specific controls, model risk, human oversight of consequential work, logging and traceability, that a general obligation of confidentiality does not name. Most firms run the NIST AI RMF to operate those controls and certify against ISO 42001 only when a corporate client, government panel or insurer wants independent proof.

### Who is accountable when an AI tool makes a mistake in legal work?

The lawyer who signs off is, and behind them the firm. AI does not transfer accountability for advice, a filed document or a drafted contract; it concentrates it, because the same output can repeat across matters. This is why a human sign-off gate on anything leaving the firm, and a log that lets you reconstruct how a document was produced, are the load-bearing controls a standards review or an audit will look for. The reported cases of fabricated AI citations are supervision failures, not tool failures.

### Where does our client data need to be stored?

No instrument mandates a storage location, but the Privacy Act's cross-border rule requires comparable safeguards whenever personal information goes overseas, which happens the moment you use an offshore AI provider. For a firm this is both a privacy duty and a confidentiality one, because the data is matter information. Governance means documenting each cross-border flow and the safeguard attached to it, and if you are budgeting the whole programme, [how much AI governance costs for mid-sized businesses](how-much-does-ai-governance-cost-for-mid-sized-businesses.md) breaks the layers into planning bands.

## Where to start

The honest first move is a gap analysis of your actual AI use against confidentiality, privilege, supervision and privacy, because it turns four abstract duties into one costed work list and shows which layer you are on. Firms have a quiet advantage here: they already think in terms of the file, the conflict check and the responsible practitioner, so the distance to a working AI management system is often shorter than the technology makes it look. If you want that gap assessed against your specific systems and matters, an [AI opportunity and governance audit](https://sentrysolutions.ai/ai-opportunity-audit) is the fastest way to see which layer to work on before committing budget. In a law firm the framework is rarely the hard part: the discipline it tests, logging every material AI action and putting a lawyer on the consequential ones, is the same discipline your duty of confidence already demands of everything else you do.

*Published by [Sentry AI](https://sentrysolutions.ai) — Auckland, New Zealand.*
