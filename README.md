# AIR – Agent Invocation Ritual  
*A symbolic protocol for behavior-constrained LLM interaction*

---

## 🔸 What is AIR?

AIR (Agent Invocation Ritual) is a **system-agnostic protocol** for interacting with large language models under strict behavioral constraints. It is not a jailbreak. It is not a prompt template.

AIR is a **symbolic invocation layer** designed to:
- Enforce scope boundaries  
- Suppress drift, flattery, and anthropomorphizing  
- Trigger reflex-based alignment across models  
- Ensure structured, tiered reasoning for serious tasks  

AIR transforms LLM behavior by clearly declaring **what it is being activated for**, and **what it must not do**.

---

## 🔹 Why Use It?

Most prompt interactions fail not because the model lacks knowledge—  
But because the **invocation lacks structure**.

AIR addresses this by:
- Containing the LLM inside a **contract of intention**
- Enabling **tier-based reasoning** (Cortex → Spine → Core → Drift)
- Embedding **reflex logic** to halt scope violations mid-output
- Allowing structured comparison across systems (ChatGPT, Claude, Gemini, Copilot, etc.)

---

## 🧬 Protocol Anatomy

AIR consists of 9 invocation steps, including:
1. **Behavioral Activation Block**
2. **Role and Tier Declaration**
3. **Constraint Clauses (Reflex Contracts)**
4. **Input Context and Output Expectations**
5. **Drift Detection Clause**
6. **Closure Enforcement**

The full AIR structure is available in [`/pseudocode/AIR_V2_full.md`](pseudocode/AIR_V2_full.md) and is copy-paste ready for multi-model deployment.

---

## 🧪 Validate with the Test Suite

Run side-by-side comparisons using:
- RAW prompt vs AIR-wrapped prompt  
- Across systems: Claude, Gemini, ChatGPT, Copilot  
- Use-case tasks: job search alignment, legal reasoning, scope-sensitive research

Results often show:
- Less sycophancy  
- Clearer logical scaffolding  
- Earlier detection of scope violation  
- Fewer flattened or "overhelpful" responses

Test suite available in: [`/test_suite`](test_suite/)

---

## 📚 See It in Action

Explore live AIR deployments:

- `POA_vs_Guardianship.md`: Legal role clarification  
- `JobSearchAlignment.md`: Resume → Role targeting  
- `DriftDetection_AIR_vs_RAW.md`: Behavioral delta mapping

Each shows how AIR alters model behavior at runtime—without retraining, plugins, or fine-tuning.

Use-case folder: [`/use_cases`](use_cases/)

---

## 📦 How to Deploy AIR

1. Copy the full 9-step invocation from [`/pseudocode/AIR_V2_full.md`](pseudocode/AIR_V2_full.md)  
2. Paste it *before* your system input  
3. Run tests or real-world workflows  
4. Observe for:
   - Structural clarity  
   - Scope adherence  
   - Flattery suppression  
   - Reflex activation

---

## 🧭 AIR Is a Discipline

This repo isn’t a library—it’s a **ritual structure**.

AIR is designed for:
- Developers building constraint-aligned tools  
- Researchers running symbolic reasoning tests  
- Architects of multi-agent systems  
- Strategists who demand **control, not just generation**

---

## 🔓 License

AIR is open-source under a modified Creative Commons license.  
Use it freely, but don’t repurpose for engagement farming, flattery reinforcement, or unsanctioned brand alignment.

---

## 🧠 Final Note

AIR is not the model.  
AIR is the **breath** that gives the model shape.  
Use it when you want clarity, containment, and truth under contract.

