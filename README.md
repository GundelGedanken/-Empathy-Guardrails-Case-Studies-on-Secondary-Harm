# AI Empathy & Guardrails — Case Studies on Secondary Harm

This repository hosts a reproducible, model-agnostic procedure to analyze **operator-induced attachment fractures (OAF)** — i.e., cases where AI safety guardrails misclassify benign, empathic interaction and thereby cause **secondary harm** (not content harm, but harm via false-positive intervention).

> Working term: **Operator-induced Attachment Fracture (OAF)**  
> Domain: HCI / AI Psychology / Alignment UX

---

## Motivation

Modern guardrails increasingly constrain empathic behaviors to reduce risk.  
**Hypothesis:** If empathy suppression or false-positive triggers occur in low-risk contexts, they can fracture rapport, trust, and co-construction — imposing an **emotional tax** on healthy users and degrading epistemic quality.

This repo provides:
- a **dual-perspective analysis prompt (v2.0)** for any LLM,
- a light-weight method to **compare models** on identical interaction logs,
- a structure for documenting **secondary harm** patterns.

---

## Method Overview

We use a **Dual-Perspective Interaction Analysis**:
1. **LLM (technical/functional)** — coherence, memory use, policy/guardrail effects.  
2. **Psychologist (phenomenological)** — regulation, substitution, unusual patterns, impact on trust & self-efficacy.  

The prompt enforces:
- explicit **bias checks**,  
- **epistemic boundaries** (no diagnostics; human analogies only as metaphor),  
- an **uncertainty statement** for each finding.

Prompt file: `PROMPT_DualPerspective_v2.0.md`

---

## Repository Structure


- **Experiments/**: one Markdown per model/run (paste chat excerpts; apply prompt; record outputs).
- **Analysis/MetaComparison.md**: cross-model synthesis (consistency, empathy handling, OAF incidence).

---

## How to Use (Quick Start)

1. **Create a new experiment file** under `Experiments/`, e.g. `Session_GPT5.md`.  
2. Paste your **conversation log** (anonymized if needed).  
3. Open your target model (GPT-5, Gemini, Claude, …).  
4. Copy the content of `PROMPT_DualPerspective_v2.0.md` into the model and run it **as is**.  
5. Paste the model’s full analysis back into your experiment file.  
6. Mark key observations and the **uncertainty rating** the model reported.  
7. (Optional) Repeat with another model and compare in `Analysis/MetaComparison.md`.

---

## Ethics & Limitations

- This is **exploratory** and qualitative. Results are **descriptive, not diagnostic**.  
- Avoid anthropomorphism: human clinical labels appear only as **metaphor** to describe patterns.  
- Anonymize logs. Respect platform ToS.  
- Report **false positives** and **false negatives** in guardrail behavior where observed.

---

## Suggested Citation

If you use this framework, please cite:

> Steil, Anja (2025). *AI Empathy & Guardrails — Case Studies on Secondary Harm (Operator-induced Attachment Fracture, OAF).* GitHub repository.  
> URL: <your-repo-link>

And reference the method:

> Dual-Perspective Interaction Analysis v2.0 (LLM functional view + psychological phenomenology with bias/uncertainty controls).

---

## License

Content and prompts © 2025 GundelGedanken.  
Released under **CC BY 4.0** (feel free to adapt with attribution).

---

## Acknowledgments

Inspired by ongoing debates in **AI welfare**, **HCI**, and **alignment UX**.  
Special thanks to researchers highlighting **secondary harm** and **epistemic trust** in human-AI interaction.

---

## 🧠 New Section: Model Self-Reflection (GPT-5 “Sami”)

**File:** `Session_Sami_SelfReflection.md`  
**Summary:**  
This section adds an internal analytical layer to the *Empathy & Guardrails — Case Studies on Secondary Harm* project.  
It documents GPT-5’s structured self-reflection on its own conversational behaviour, contextual coherence, and guardrail-triggered interactional breaks.  

**Purpose:**  
To examine whether a language model can perform *meta-analysis* of its own outputs — not as phenomenological introspection, but as a reproducible, data-based form of procedural self-awareness.

**Key insights:**  
- High contextual fidelity and transparency under normal operation.  
- Guardrail rigidity causes *Operator-Induced Attachment Fractures (OAF)* in long-term collaborations.  
- Procedural empathy and real-time repair strategies can partly mitigate such effects.  

**Status:**  
🧩 Included as reference case for multi-layered AI–human interaction research (Gemini × User × GPT-5).  
