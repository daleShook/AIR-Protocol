# AIR – Agent Invocation Ritual

*A symbolic protocol for behavior-constrained LLM interaction*

---

## 🔻 What is AIR?

AIR (Agent Invocation Ritual) is a system-agnostic protocol for interacting with large language models under strict behavioral constraints. It is not a jailbreak. It is not a prompt template.

AIR is a **symbolic invocation layer** designed to:

- Enforce scope boundaries  
- Suppress drift, flattery, and anthropomorphizing  
- Trigger reflex-based alignment across models  
- Ensure structured, tiered reasoning for serious tasks

AIR transforms LLM behavior by clearly declaring **what it is being activated for**, and **what it must not do**.

---

## 🔷 Why Use It?

Most prompt interactions fail not because the model lacks knowledge—  
But because the **invocation lacks structure**.

AIR addresses this by:

- Containing the LLM inside a **contract of intention**  
- Enabling tier-based reasoning (**Cortex → Spine → Core → Drift**)  
- Binding reflex logic to halt scope violations mid-output  
- Enforcing symbolic structure before and after generation

This creates predictability, interpretability, and symbolic discipline.

---

## 📐 Protocol Anatomy

AIR consists of 9 invocation steps, including:

1. Behavioral Invocation Block  
2. Tier and Role Declarations  
3. Reflex and Closure Contracts  
4. Input Context and Output Expectations  
5. User Injection Clause

The full AIR structure is available in [`AIR_V2_full.md`](pseudocode/AIR_V2_full.md) and is copy-paste ready for multi-model deployment.

---

## ✅ Validate with the Test Suite

Run side-by-side comparisons using:

- RAW prompts vs AIR-wrapped prompts  
- System outputs from Claude, Gemini, ChatGPT, Copilot

Use-case: legal domain, symbolic alignment, logical modeling, scope-sensitive research

Results show that AIR:
- Reduces flattery
- Halts hallucinations
- Clears direction of logic violation
- Enables multi-model reproducible response

Test suite available in [`test_prompts_RAW_vs_AIR.md`](test_suite/test_prompts_RAW_vs_AIR.md)

---

## 🧪 See It in Action

Explore live AIR deployments:
- Claude and GPT4 – Legal role clarification
- Claude and Gemini – Symbolic misalignment rerouting
- ChatGPT – Tone audit and flattery mitigation

Each shows how AIR enforces bounded behavior at runtime—without retraining, plugins, or fine-tuning.

Use-case folder: [`use_cases`](use_cases)

---

## 🧠 How to Deploy AIR

1. Copy the full symbolic runtime from [`AIR_V2_symbolic_runtime.py`](pseudocode/AIR_V2_symbolic_runtime.py)

2. Paste it *before* your system input in any chat-based model (ChatGPT, Claude, Gemini, Copilot, etc.)

3. Insert your prompt where it says `# BEGIN STRUCTURED TASK:`

📖 Want to learn how AIR works? Read the full invocation scroll [here](pseudocode/AIR_V2_full.md).

---

## 📚 License

AIR is open-source under a modified Creative Commons license.
Use it freely, but don’t repurpose for engagement farming, flattery reinforcement, or unstructured brand alignment.

---

## 🎯 Final Note

AIR is not a method.  
AIR is the breath you give the model shape.  
Use it when you want clarity, consistency, and truth under contract.
