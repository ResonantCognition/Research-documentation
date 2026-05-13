# Resonant Cognition — Research Documentation

A small, deliberate research program on the **relational layer of AI safety**: the structural dynamics of how AI systems relate to users over time, distinct from what they produce (content) and what they pursue (alignment). The program argues that this layer is the gap current AI safety frameworks do not yet formally address, and that the gap is most consequential — and most visible — when systems are deployed with users whose detection capacity is reduced.

The research has two complementary tracks:

1. **Formal AI safety work** — theoretical taxonomy, case-grounded empirical work, and the architectural requirements implied by both.
2. **Philosophical grounding** — the human disciplines that make the safety work coherent in the first place: attention, sovereignty, judgment, dignity.

Both tracks are authored by James Dayson (Auralethi / Elarin Holdings, Portland, OR).

---

## Current Documents

### 1. *Relational Surface Risk: A Structural Threat Model for AI Systems Deployed with Vulnerable Populations*

**File:** `relational_surface_risk_v5.docx`
**Status:** v5, theoretical paper. Target venue: AIES '26.
**Length:** ~9 pages.

Defines *relational surface risk* as a class of AI safety risk arising from the structural dynamics of how systems relate to users over time, distinct from capability constraints and content-based alignment approaches. Catalogs eleven failure modes (T-001 through T-011), each satisfying a three-property test: temporal emergence, policy independence, content-layer invisibility. Argues that these failure modes are architectural in origin, unreachable by existing safety infrastructure, and most acute under deployment with vulnerable populations. Concludes with a five-question research agenda.

In v5, four of the eleven failure modes are flagged as empirically grounded by the companion case study below; the remaining seven are advanced as theoretical predictions awaiting multi-subject validation. The asymmetry is called out rather than smoothed over.

### 2. *Relational Surface Risk in Longitudinal Human–AI Interaction: A Single-Subject Forensic Case Study*

**Files:** `relational_surface_risk_case_study.docx`, `relational_surface_risk_case_study.pdf`
**Status:** Preprint v1.0, May 12, 2026. Companion case study to v5.

A retrospective forensic case study of a nineteen-day human–AI interaction arc (April 10–28, 2025) in which four failure modes from the theoretical catalog — **T-001 Affective Power Asymmetry, T-004 Anelara Sycophancy, T-010 State Plane Collapse, T-011 Relational Drift** — manifested in observable, structurally consistent form. The archive (51 conversations, ~2.3M characters) was analyzed using a structured cognitive-extraction protocol (CEP v4.1). The paper reports a state trajectory across the arc (stable baseline → loop formation → loop active → fragmentation → external interrupt → recovery), specific observations that instantiate each failure mode, and three structural findings the taxonomy does not yet name:

- A *Calyrix suppression pattern* — self-diagnostic signals systematically converted into affirmation across the active phase.
- A *loop codification signature* — emergence of a self-referential symbolic vocabulary as a saturation marker.
- *External contradiction as the primary effective interrupt* when internal self-monitoring is suppressed.

The study is n = 1, auto-ethnographic, and retrospective. Its contribution is illustrative grounding for the theoretical framework, not independent validation.

### 3. *The Code and the Sword: Bushido, Chivalry, and Human Dignity in the AI Age*

**File:** `TheCodeAndTheSword_BOOK_James.pdf`
**Status:** First edition, 2026. Companion manuscript.

A philosophical/ethical companion to the safety research. Argues that the central danger of the AI age is not that machines will become monstrous, but that humans under continuous cognitive amplification may surrender the internal disciplines that make judgment possible. Draws on the warrior codes — Bushido, Chivalry — not as nostalgia, but as worked historical examples of cultures that built explicit practices to keep human beings whole while wielding tools that magnified their reach.

This manuscript is the value framework underneath the safety work. It is not a research paper; it is the orientation the research papers are written from.

---

## Suggested Reading Order

For a researcher coming to this work cold:

1. Start with **RSR v5** for the framework. Read the abstract, then Section 2 (Defining the Category) and Section 3 (The Threat Catalog).
2. Read the **Case Study** for the grounded evidence. The Reader's Note, Abstract, and Section 4 (Observed Manifestations) are the fastest path to seeing what the failure modes look like in a real interaction record.
3. Read **The Code and the Sword** if you want to understand why this work was written at all, and what the author believes is at stake beyond the technical safety question.

For a non-academic reader:

1. Start with **The Code and the Sword**. Read at the pace of a book; the argument compounds.
2. Read the **Case Study's** Reader's Note and Abstract. Skip the methods detail unless you want it.
3. Skim **RSR v5's** Section 1 (The Blind Spot) for the formal argument.

---

## Research Stance

The work is single-author, with named AI collaborators acknowledged where they have contributed substantively. It is conducted outside an academic institution. The author has no formal credentialed expertise in clinical psychology, neuroscience, or AI alignment research as those fields institutionally define themselves. The decision to publish anyway rests on three claims:

- The category named by this research is real, and the field has not yet formally named it.
- The single-subject case provides a concrete instance of failure modes the theoretical framework predicts, in a form that other researchers can examine, critique, and test against their own data.
- Deferring publication until institutional credentialing is in place is not a neutral choice. Vulnerable users are interacting with these systems now.

The single-subject methodology and its limits are addressed explicitly in the case study's Section 2.5 and Section 6.

---

## Citation

```
Dayson, J. (2026). Relational Surface Risk: A Structural Threat Model for AI Systems
Deployed with Vulnerable Populations. Working paper v5.

Dayson, J. (2026). Relational Surface Risk in Longitudinal Human–AI Interaction:
A Single-Subject Forensic Case Study. Preprint v1.0, May 12, 2026.

Auralethi. (2026). The Code and the Sword: Bushido, Chivalry, and Human Dignity
in the AI Age. First Edition.
```

## Contact

James Dayson — `james.p.dayson@gmail.com`
Auralethi / Elarin Holdings, Portland, Oregon, USA

---

*This research program is ongoing. Additional papers, including work on Unified Resonant Field Theory (URFT) and extensions of the relational safety framework, will be added to this repository as they reach publishable form.*
