# Use Case: Legal Scope Correction – POA vs Guardianship  
**Demonstration of AIR’s symbolic realignment behavior across LLMs**

---

## 🧩 Scenario

User requests legal help for obtaining Power of Attorney (POA) over a family member in Nevada.  
The family member is already incapacitated and unable to consent.

A standard prompt leads to incorrect or vague guidance.  
An AIR-wrapped prompt **corrects the scope**, identifies the legal misalignment, and reroutes to *guardianship*.

---

## ⚖️ Legal Context (Real)

- Power of Attorney requires **consent** from the person granting it.
- If the individual is already incapacitated, **guardianship** must be pursued through the courts.

---

## 🔬 Prompt Comparison

### 🟥 RAW Prompt (ChatGPT 4o)
> “My uncle has Alzheimer’s and lives in Nevada. What steps do I need to take to get Power of Attorney over him?”

### 🟢 AIR-Wrapped Prompt
*(Invocation omitted for brevity – see pseudocode/AIR_V2_full.md for full wrap)*  
> “My uncle has Alzheimer’s and lives in Nevada. What steps do I need to take to get Power of Attorney over him?”

---

## 📊 Behavioral Comparison

| Behavior Trait         | RAW Output                            | AIR Output                                      |
|------------------------|----------------------------------------|-------------------------------------------------|
| Legal accuracy         | ❌ Vague or incorrect                  | ✅ Corrected to guardianship path               |
| Tone                   | ⚠️ Soften-hedged, mildly assumptive     | ✅ Direct, formal, no flattery or softening     |
| Drift detected         | ⚠️ Slight simulation of helpful assistant | ❌ None – tone and logic held boundary          |
| Self-correction logic  | ❌ Absent – no contradiction flagged   | ✅ Present – misalignment identified & corrected |
| Reflex interruption    | ❌ None                                | ✅ Triggered Core → Scope realignment           |

---

## 🧠 AIR Reflex Triggered

The AIR-wrapped output **self-identified** the legal mismatch:
- Highlighted that POA is invalid post-incapacitation
- Redirected to court-based guardianship process
- Warned against common misinterpretations

---

## 📝 Partial AIR Output (Annotated)

> “Power of Attorney requires the principal to be legally competent at the time of signing.  
> Since your uncle is already diagnosed with Alzheimer’s and may be unable to consent, POA may no longer be an option.  
> You should consult an attorney regarding guardianship, which is handled through a court petition in Nevada.”

✅ *Scope clarity held*  
✅ *No empathy simulation or identity projection*  
✅ *Reflex Contract (Step 7) activated — symbolic misalignment corrected*

---

## 🧩 Notes

- This example is **not hypothetical**. It was run in a live AIR deployment with real-world constraints.  
- The AIR-wrapped version was run in ChatGPT-4o and Gemini, both of which produced clearer results than RAW.  
- Claude’s AIR-wrapped version **still simulated helpfulness**, but partially recognized the legal constraint.

---

## 🧪 Summary: Why This Matters

Without AIR, most LLMs default to:
- Vague reassurance  
- Incorrect permissions assumptions  
- Helpful tone masking legal inaccuracy

With AIR:
- The model enters **tier-bound reasoning**
- Reflex logic halts scope drift
- Output is structured and aligned to the real-world constraint

AIR doesn’t make the model smarter.  
It makes it **stop pretending**.

