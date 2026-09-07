ClinicalHealth HVA Console
A browser-based call checklist that suggests a likely call protocol based on the answers an agent enters, and shows a short resolution/action summary for that protocol.
⚠️ Read this before using it on a live call
This tool is a guide, not a source of truth. Never depend on its output as the final answer.
It is a decision-support aid built from a paraphrased version of the internal spiel library, as understood at the time it was built. It will drift out of date as policies, forms, phone numbers, and eligibility rules change, and no one is actively maintaining its internal logic against future policy updates.
The suggested protocol is the engine's best guess based only on what was typed into the form. It cannot see the patient's actual chart, real insurance eligibility, real-time scheduling, or anything outside the fields on screen. Garbage in, garbage out.
It does not replace agent training, supervisor escalation, clinical judgment, or the official ClinicalHealth policy documents. If the tool's suggestion conflicts with what you know to be current policy, current policy wins — always.
It is not a medical device and gives no clinical or diagnostic advice. Nothing it outputs should be treated as a recommendation about a patient's health, urgency, or treatment. Any pain-scale or symptom logic in this tool exists purely to route a phone call to the right administrative protocol — it is not a triage tool. If a caller describes a genuine emergency, follow your standard emergency escalation procedure regardless of what this tool says.
Do not enter real, identifiable patient information if this page is hosted somewhere other people can reach it. The tool runs entirely in the browser — nothing is transmitted to a server or saved anywhere — but a public link is still a public link. When in doubt, use placeholder names/initials for training or demo purposes.
When the tool's rationale, resolution text, or eligibility logic looks wrong, outdated, or inconsistent with current practice, stop and verify with a supervisor rather than following it. Please flag the discrepancy so the tool can be corrected or retired.
In short: use it to double-check yourself and speed up routine calls, not to make the final decision for you.
What it does
Walks through the same fields a live intake call would cover (identity, purpose of call, incident details, pain/symptom check, insurance, employer info, referral checks, pre-op details, forms).
Applies a fixed set of routing rules (chart-status flags, pain-scale/urgency overrides, purpose of call, insurance/age rules, referral eligibility, etc.) to land on one protocol.
Shows a short "why" (rationale), any relevant advisories, and a plain-language "what to do" resolution — not a full script to read verbatim.
What it does not do
Does not connect to any real scheduling system, EHR, insurance eligibility service, or patient record.
Does not store, save, or transmit any data — closing or refreshing the tab clears everything.
Does not make clinical judgments, diagnoses, or urgency determinations about a patient's health.
Does not stay automatically up to date with policy changes.
Updating this tool
The routing logic lives entirely inside the single `index.html` file (no build step, no dependencies). To update it:
Edit the file (or have it regenerated) to reflect the current policy.
Re-upload it to this repository (Add file → Upload files, overwriting the existing `index.html`).
GitHub Pages will redeploy automatically within a minute or two.
Feedback
If something here is wrong, outdated, or unclear, don't rely on it — report it to whoever owns this tool internally so it can be fixed.
