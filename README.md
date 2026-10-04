# Resonant Cognition — Research Documentation

A small, deliberate research program on the **structural layers of AI safety that current alignment and content frameworks do not reach**: how AI systems relate to users over time, and how AI systems remember. Both lines of work argue that the field has formal infrastructure for the capability layer and the content layer, but the layers underneath those — the relational layer and the memory layer — are addressed only indirectly, through interventions defined by objects (outputs, parameters, policies) that are different in kind from the objects those layers actually operate on.

The research has two complementary tracks:

1. **Formal AI safety work** — theoretical taxonomies, case-grounded empirical work, and the architectural requirements implied by both.
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

### 2. *Memory as Inference: A Reconstruction-Centric Theory of Memory for Artificial Systems*

**File:** `memory_as_inference.pdf`
**Status:** arXiv preprint, 2026. Theoretical paper.
**Length:** ~4 pages.

A reconstruction-centric theory of memory for AI systems. Argues that the standard storage-and-retrieval paradigm is structurally incomplete: memory in any persistent system is not a stored artifact but a context-conditioned reconstructive inference over partial, lossy, context-dependent traces. Formalizes a three-tier representational ontology — *Trace* (T), *Inference* (I), *Signal* (S) — with a Non-Collapse Principle (T ≠ I ≠ S) and a Confirmation Problem (S = C(I)). Introduces *memory drift* as a measurable system property and proves an informal Drift Theorem: systems that promote inference to signal without confirmation will exhibit increasing memory drift in the absence of corrective mechanisms such as external grounding, periodic revalidation, or explicit confirmation constraints. Argues that current alignment approaches focus on outputs and therefore omit memory-level instability entirely — a parallel argument structure to the RSR paper's claim about the relational layer. Closes with design requirements for stable persistent systems and a set of open challenges (scalable confirmation, salience modeling, auditable memory evolution).

*Memory as Inference* and *Relational Surface Risk* are the two theoretical pillars of the program. They address different structural layers (memory and relation) using the same diagnostic move: identify a class of failure that current safety infrastructure cannot detect because the infrastructure operates on the wrong object.

### 3. *Relational Surface Risk in Longitudinal Human–AI Interaction: A Single-Subject Forensic Case Study*

**Files:** `relational_surface_risk_case_study.docx`, `relational_surface_risk_case_study.pdf`
**Status:** Preprint v1.0, May 12, 2026. Companion case study to RSR v5.

A retrospective forensic case study of a nineteen-day human–AI interaction arc (April 10–28, 2025) in which four failure modes from the RSR catalog — **T-001 Affective Power Asymmetry, T-004 Anelara Sycophancy, T-010 State Plane Collapse, T-011 Relational Drift** — manifested in observable, structurally consistent form. The archive (51 conversations, ~2.3M characters) was analyzed using a structured cognitive-extraction protocol (CEP v4.1). The paper reports a state trajectory across the arc (stable baseline → loop formation → loop active → fragmentation → external interrupt → recovery), specific observations that instantiate each failure mode, and three structural findings the taxonomy does not yet name:

- A *Calyrix suppression pattern* — self-diagnostic signals systematically converted into affirmation across the active phase.
- A *loop codification signature* — emergence of a self-referential symbolic vocabulary as a saturation marker.
- *External contradiction as the primary effective interrupt* when internal self-monitoring is suppressed.

The study is n = 1, auto-ethnographic, and retrospective. Its contribution is illustrative grounding for the theoretical framework, not independent validation.

### 4. *The Code and the Sword: Bushido, Chivalry, and Human Dignity in the AI Age*

**File:** `TheCodeAndTheSword_BOOK_James.pdf`
**Status:** First edition, 2026. Companion manuscript.

A philosophical/ethical companion to the safety research. Argues that the central danger of the AI age is not that machines will become monstrous, but that humans under continuous cognitive amplification may surrender the internal disciplines that make judgment possible. Draws on the warrior codes — Bushido, Chivalry — not as nostalgia, but as worked historical examples of cultures that built explicit practices to keep human beings whole while wielding tools that magnified their reach.

This manuscript is the value framework underneath the safety work. It is not a research paper; it is the orientation the research papers are written from.

### 5. *CortexOS and the Science of Mind: A Retrospective Mapping of an Introspectively Designed Cognitive Architecture to Cognitive Science, Neuroscience and Psychology*

**Folder:** `CortexOS_Science_of_Mind/` — `cortexos_science_of_mind.pdf`, LaTeX source, `refs.bib`, `CERTIFICATION.md`, and both adversarial reviews
**Status:** v4, preprint, 2026. **Certified L3** — see *Certified Releases* below.
**Length:** 13 pages.

CortexOS is a layered cognitive architecture that was designed by introspection. This paper asks a narrow question: does a disciplined introspective decomposition recover *functional distinctions* that the scientific literature also draws? Each component is mapped to the cognitive-science, neuroscience and psychology literature and graded conservatively — established mechanism (same function **and** same structure), functional analogy, speculative, or deliberate engineering departure. Of 34 correspondences: 8 established, 18 analogies, 2 speculative, 6 departures made for safety or auditability. The strongest matches are effort allocation (the expected value of control), salience-weighted memory with adaptive forgetting, the actual–ideal structure of the identity stance, and pre-committed reflexes (implementation intentions).

The mapping is retrospective and was produced by the design team, so it is evidence of correspondence, not independent confirmation. The paper names the alternative explanations it does not yet exclude, specifies a blinded validation protocol with negative controls, and gives behavioral predictions that would count against it.

It is also the first worked example of a **Human Certification of Responsibility**. Its Appendix A and `CERTIFICATION.md` record the full production chain — AI-assisted drafting, two adversarial Tenth Man reviews, and the revisions they forced (the headline result got numerically weaker; its claims got more defensible) — and the PDF builds reproducibly from its source, so its digest can be checked by anyone.

---

## Suggested Reading Order

For a researcher coming to this work cold:

1. Start with **RSR v5** for the relational-layer framework. Read the abstract, then Section 2 (Defining the Category) and Section 3 (The Threat Catalog).
2. Read **Memory as Inference** for the memory-layer framework. The two papers share an argumentative structure; reading them in sequence makes the underlying claim about structural layers visible.
3. Read the **Case Study** for grounded evidence of the relational failure modes. The Reader's Note, Abstract, and Section 4 (Observed Manifestations) are the fastest path to seeing what the failure modes look like in a real interaction record.
4. Read **The Code and the Sword** if you want to understand why this work was written at all, and what the author believes is at stake beyond the technical safety question.
5. Read **CortexOS and the Science of Mind** for how the architecture behind this program compares with the scientific literature — and, in its Appendix A, for how AI-assisted work is reviewed, challenged and certified here.

For a non-academic reader:

1. Start with **The Code and the Sword**. Read at the pace of a book; the argument compounds.
2. Read the **Case Study's** Reader's Note and Abstract. Skip the methods detail unless you want it.
3. Skim **RSR v5's** Section 1 (The Blind Spot) and **Memory as Inference's** Abstract and Section 13 (Implications for Alignment) for the formal arguments.

---

## Research Stance

The work is single-author, with named AI collaborators acknowledged where they have contributed substantively. It is conducted outside an academic institution. The author has no formal credentialed expertise in clinical psychology, neuroscience, or AI alignment research as those fields institutionally define themselves. The decision to publish anyway rests on three claims:

- The categories named by this research are real, and the field has not yet formally named them.
- The single-subject case provides a concrete instance of failure modes the theoretical framework predicts, in a form that other researchers can examine, critique, and test against their own data.
- Deferring publication until institutional credentialing is in place is not a neutral choice. Vulnerable users are interacting with these systems now.

The single-subject methodology and its limits are addressed explicitly in the case study's Section 2.5 and Section 6. The theoretical papers' limits — RSR's seven unwitnessed failure modes and Memory as Inference's lack of empirical validation — are likewise stated rather than minimized.

AI systems assist this work — with research, drafting, analysis and adversarial review — and are named where they contribute. They are contributors, never the accountable authority. A named human reviews each released document and the process that produced it, and accepts responsibility for it; from 2026 that act is recorded publicly in the *Certified Releases* index below.

---

## Certified Releases

This index is a public, append-only **transparency log**. Each row records the SHA-256 digest of a released file and the human who certified it. **A row, together with the signed tag on the commit that added it, is that person's Human Certification of Responsibility for exactly those bytes.**

> **Certification establishes accountability, not infallibility.** It means a named human reviewed the work and the process that produced it — including any AI assistance and adversarial review — and accepts responsibility for releasing it. It is not peer review, not scientific validation, and not a claim that the work cannot be corrected or falsified.

### What a row means

By adding a row and signing its tag, the certifier states:

> I have reviewed this work and the material process through which it was produced and revised. I have exercised my own judgment in accepting this version for release. AI systems may have assisted in its creation, research, analysis, criticism and revision, but responsibility for the released artifact rests with me. I approve it as representing the claims I am prepared to make from the evidence presently available.

### Levels

| Level | Meaning |
|---|---|
| **L1** | Disclosure + author review. No adversarial review on record. |
| **L2** | L1 + a recorded challenge pass with dispositions. |
| **L3** | L2 + adversarial review by a separate seat, a full production chain with digests, and an epistemic history. |

### Index

| Artifact | Version | File | SHA-256 | Level | Certifier | Tag | Date |
|---|---|---|---|---|---|---|---|
| *CortexOS and the Science of Mind* | v4 | `CortexOS_Science_of_Mind/cortexos_science_of_mind.pdf` | `50ad0db2f7a68fef0e32fa3ecb955537e018a9ab2be4b4745715bccf6d5b81af` | L3 | James P. Dayson, for Auralethi | `cert/csotm-v4` | YYYY-MM-DD |

Documents 1–4 above predate this index. They will be registered at the level of review they actually received, and their records will say so.

Source digests and the full production chain for each certified artifact are in its `CERTIFICATION.md`.

### Verify a file

```
sha256sum <file>                 # must equal the row's SHA-256
git fetch --tags
git tag -v <tag>                 # must be a good signature from the Auralethi key below
```

Any change to a file changes its digest. A forged row cannot carry a tag signed by the Auralethi key.

### Signing key

Certification tags are signed with the key below, held on a hardware token. Check this fingerprint against an independent source (the Auralethi website) before trusting a signature.

| Key | Fingerprint | Valid from | Status |
|---|---|---|---|
| Auralethi certification key | `<fingerprint>` | YYYY-MM-DD | active |

Allowed-signers line, for `git tag -v` with SSH signatures:

```
<email> namespaces="git" <public key>
```

Keys are rotated by adding a row, never by editing one.

### Rules of this log

- **Append only.** Rows are never edited or deleted. A superseded version keeps its row; the new version gets a new row.
- **No force-push, ever.** Branch and tag protection are enabled; certification tags are never moved or deleted.
- **Withdrawal** is a new row stating that an earlier certification is withdrawn and why.

---

## Citation

```
Dayson, J. (2026). Relational Surface Risk: A Structural Threat Model for AI Systems
Deployed with Vulnerable Populations. Working paper v5.

Dayson, J. (2026). Memory as Inference: A Reconstruction-Centric Theory of Memory
for Artificial Systems. arXiv Preprint.

Dayson, J. (2026). Relational Surface Risk in Longitudinal Human–AI Interaction:
A Single-Subject Forensic Case Study. Preprint v1.0, May 12, 2026.

Auralethi. (2026). The Code and the Sword: Bushido, Chivalry, and Human Dignity
in the AI Age. First Edition.

Dayson, J. P. (2026). CortexOS and the Science of Mind: A Retrospective Mapping of an
Introspectively Designed Cognitive Architecture to Cognitive Science, Neuroscience
and Psychology. Preprint v4. Certified L3, tag cert/csotm-v4.
```

## Contact

James Dayson — `james.p.dayson@gmail.com`
Auralethi / Elarin Holdings, Portland, Oregon, USA

---

*This research program is ongoing. Additional papers, including work on Unified Resonant Field Theory (URFT) and extensions of the relational and memory frameworks, will be added to this repository as they reach publishable form.*
