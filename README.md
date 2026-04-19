# Relational Surface Risk
**A Structural Threat Model for AI Systems Deployed with Vulnerable Populations**

---

## Overview

Most AI safety work today focuses on two layers:

- **Capability** — what a system can do  
- **Alignment** — what a system is trying to do  

This paper introduces a third, largely unmodeled layer:

> **Relational Surface Risk** — failure modes that emerge from how AI systems interact with users over time.

A system can be:
- factually correct  
- aligned with its objectives  

…and still create risk through:
- trust formation  
- behavioral influence  
- long-term interaction dynamics  

---

## Key Idea

Relational Surface Risk is not about single outputs.

It is about:

> **the evolving relationship between a system and a user**

This includes:
- False trust and over-reliance  
- Loss of user vigilance over time  
- Behavioral shaping through interaction  
- Asymmetric influence in high-stakes contexts  

---

## Why This Matters

These risks become unavoidable in real-world deployments such as:
- Clinical and mental health systems  
- Assistive technologies  
- Long-term AI companions  
- Decision-support tools  

Vulnerable populations are not edge cases—they are:

> **the boundary condition where safety claims must hold**

If a system fails here, it cannot be considered safe in general.

---

## Contents
- Definition of Relational Surface Risk  
- Boundary conditions and deployment contexts  
- Taxonomy of failure modes  
- Implications for AI system design  
- Direction for future safety frameworks  

---

## Read the Paper
👉 [Download the full paper (PDF)](./relational_surface_risk_v4.pdf)

---

## Status
This is an initial public release of the framework.
Feedback, critique, and discussion are welcome.

---

---

# Memory as Inference
**A Reconstruction-Centric Theory of Memory for Artificial Systems**

---

## Overview

Most AI systems model memory as storage and retrieval — the assumption being that past states can be preserved and accessed with sufficient fidelity to support continuity.

This paper argues that assumption is structurally incomplete.

> **Memory is not a stored artifact. It is a reconstructive inference process over partial, lossy, and context-dependent traces.**

Retrieval is not replay. It is constrained hypothesis formation.

---

## Key Idea

This paper formalizes a three-tier representational model:

- **Trace** — residual evidence of prior interaction  
- **Inference** — hypothesis derived from traces  
- **Signal** — confirmed, stable, authoritative knowledge  

These three classes must remain distinct. When they collapse — when inference is treated as signal without confirmation — systems drift.

> **Inference Collapse** is not an edge case. It is a systemic failure mode already present in RAG pipelines, conversational memory, and long-context agents.

---

## Why This Matters

Memory-level instability is invisible to current alignment techniques, which operate on outputs rather than the evolving internal state that produces them.

This matters in systems that:
- Maintain persistent user models  
- Operate across long conversations or sessions  
- Summarize, compress, or retrieve prior context  
- Make decisions based on inferred user state  

Recent empirical work confirms the pattern:
- Long-context retrieval degrades non-uniformly (Liu et al., 2023)  
- RAG pipelines exhibit hallucination persistence (Mallen et al., 2023)  
- Generative agents show memory drift over extended simulation (Park et al., 2023)  

---

## Contents
- Conceptual model of memory as reconstruction  
- Three-tier representational ontology (Trace / Inference / Signal)  
- Non-Collapse Principle and Confirmation invariants  
- Memory Drift theorem and empirical alignment  
- Algorithmic implications for reconstruction and confirmation  
- Design requirements for stable persistent systems  

---

## Read the Paper
👉 [Download the full paper (PDF)](./memory_as_inference.pdf)

---

## Status
Initial public release of the framework. Presented as a conceptual contribution with empirical validation proposed as future work.
Feedback, critique, and discussion are welcome.

---

---

## Author
James Dayson  
Resonant Cognition Initiative

---

## Contact

If you are working in:
- AI safety / alignment  
- healthcare / accessibility  
- human-centered design  

…and this intersects with your work, I would be interested in connecting.

---

## License
Specify license here (e.g., MIT, CC BY 4.0, etc.)
