# The Languages of Healing: What Clinical AI Cannot Hear

**A Proposal to the SHASS+ Connectivity Fund (Full Proposal)**

**PI:** Per Urlaub, Global Languages, SHASS
**Co-PI:** Leo Anthony Celi, Laboratory for Computational Physiology (IMES) / MIT Critical Data

---

## 1. What Goes Unheard

Science establishes truth through proof. This is its great strength — and its blind spot. What has not been proven is not thereby false. It may simply mean we have not yet looked, or that we have been looking with instruments too narrow to detect what is there. A grandmother in rural Uganda who detects malaria in her grandchild from the quality of the child's cry — hours before any biomarker confirms it — is not practicing folk belief. She is reading a communicative signal that no clinical AI system has been designed to hear. A community health worker in São Paulo who assesses a child through the timber of the mother's voice and the way the child shifts on her lap is processing diagnostic information that vanishes the moment it enters a medical record as text.

The fact that these communicative acts have not been systematically integrated into clinical AI does not mean they lack clinical value. It means we built our systems without listening for them.

On January 15, 2026, we convened approximately 100 participants from diverse backgrounds — clinicians, linguists, AI researchers, ethicists, indigenous knowledge keepers, artists, students — at MIT, with support from the American Medical Association, to ask a question that clinical AI has not yet seriously confronted: *what are the languages of healing, and how many of them can our systems actually hear?* The answer that emerged was stark: clinical AI, as currently built, captures almost none of them.

Clinical artificial intelligence is built on a narrow communicative foundation: typed text in electronic health records, overwhelmingly in English. The global movement toward "multilingual clinical AI" seeks to broaden this by adding more languages — a necessary effort. But it misses a more fundamental problem. Adding more languages to a text-based system is like adding more microphones inside a recording studio while the concert is happening outdoors. The problem is not which languages are represented. The problem is what we have decided counts as clinical language at all.

**The question this project poses — and empirically tests — is: how much clinically relevant communicative information is lost when the clinical encounter is reduced to text?**

This is not a new question in the abstract. A substantial body of research in non-verbal communication, clinical linguistics, and medical anthropology has long documented that paralinguistic cues, body language, and narrative context matter in clinical encounters (Roter & Hall, 2006; Heritage & Maynard, 2006; Mattingly, 1998). What *is* new — and what creates the urgency for this project — is the emergence of clinical AI systems that are being deployed globally on the basis of text alone, at a scale and speed that amplifies the textual reduction from an individual clinical limitation into a systematic, structural one. Every clinical AI system trained on medical records inherits and entrenches the assumption that what was documented is what matters. As these systems reach communities where health knowledge is transmitted orally, prosodically, or through embodied practice, the consequences of this assumption become acute.

A recent *Nature* commentary argues that artificial intelligence has achieved general intelligence, and that we must now "accept that there are more kinds of minds than we had previously entertained" (Chen et al., *Nature* 650, 2026). The authors make this case by showing that intelligence is a functional property independent of substrate — it can be realized in biological or computational systems. We suggest the same logic applies to clinical communication: the information relevant to health and healing is not bound to any single medium. It can be carried in text, yes — but also in prosody, in silence, in narrative structure, in rhythm, in the relational dynamics of an encounter. The question is not philosophical but empirical: how much of this information survives the reduction to text, and what are the clinical consequences when it does not?

This project answers that question. We conduct the first systematic, cross-linguistic study of **communicative information loss at the documentation boundary** in clinical encounters — measuring what is present in the full multimodal encounter that disappears when it becomes a medical record. We focus on two domains where the loss is likely greatest and most consequential: **prosody and paralinguistic features** (what text strips from speech) and **undocumented oral health narratives** (health communication that occurs entirely outside clinical records). The findings will establish an empirical foundation for rethinking what clinical AI needs to hear — and provide concrete design principles for building systems that can.

---

## 2. The Textual Presumption: From Individual Limitation to Structural Deafness

The insight that clinical communication extends beyond words is not new. Decades of research in medical interaction analysis have shown that physician-patient communication involves prosodic cues, gaze, gesture, touch, spatial positioning, and silence, and that these features predict outcomes including adherence, satisfaction, and diagnostic accuracy (Roter & Hall, 2006; Ambady et al., 2002). Narrative medicine has argued compellingly that the patient's story — in its full, unstructured form — carries clinical information that standardized documentation cannot capture (Charon, 2006). Medical anthropology has documented that healing systems worldwide operate through communicative modalities — song, ritual, environmental reading — that Western clinical frameworks do not recognize (Kleinman, 1988; Koss-Chioino, 2006).

What none of this work has yet confronted is the **scale amplification** introduced by clinical AI. When an individual clinician ignores prosodic cues, one patient may be affected. When a clinical AI system is trained on millions of text records that have already stripped those cues, the loss becomes structural — baked into the model's architecture, propagated at deployment scale, and invisible to standard evaluation. We call this the **textual presumption**: the unexamined assumption, inherited from the documentary tradition of Western medicine, that if something is not written, it is not clinically real. Clinical AI does not merely inherit this assumption. It industrializes it.

The textual presumption operates through two mechanisms:

**Communicative truncation at the documentation boundary.** Every clinical encounter involves a multimodal communicative event — spoken words, prosody, silence, gesture, spatial dynamics, narrative structure — that is then reduced to a text record. This reduction is not neutral. Research in clinical linguistics has shown that documentation systematically favors biomedical content over psychosocial content, active complaints over contextual information, and physician interpretation over patient expression (Hobbs, 2003; Patel et al., 2000). What is lost is not random; it is patterned, and the pattern reflects existing power structures within medicine.

**Epistemic exclusion of non-textual health communication.** Beyond what happens inside clinical encounters, a vast domain of health-relevant communication occurs entirely outside documented systems: health conversations within families and communities, oral transmission of medical knowledge in cultures without written traditions, healing practices that operate through sound, rhythm, or environmental attention. An estimated 40% of the world's languages have no writing system. For the communities that speak them, clinical AI is not merely linguistically limited — it is architecturally incapable of engaging with the communicative forms through which health knowledge is produced and transmitted.

These two mechanisms — truncation and exclusion — are analytically distinct but converge in their consequences. Both result in clinical AI systems that are systematically deaf to communicative signals that carry clinical value. This project empirically investigates the first mechanism (truncation) while developing a theoretical framework for understanding both.

---

## 3. Research Program

We propose a 12-month program with two empirical studies and one synthesis component. The program is designed to produce measurable findings, a validated analytical methodology, and a theoretical framework — grounding the broader vision in concrete results.

### Study 1: Quantifying Communicative Loss at the Documentation Boundary (Months 1–8)
*Lead: Per Urlaub and Leo Celi (joint)*

**Research question:** How much clinically relevant communicative information is present in the full multimodal clinical encounter but absent from the corresponding text record?

**Method:** We analyze clinical encounters that exist in both audio/video and text form, comparing the communicative content available in each modality. We draw on three data sources:

1. **MIMIC and PhysioNet infrastructure.** The MIMIC database includes clinical notes that correspond to documented encounters. Where audio or video recordings of clinical encounters are available through affiliated research programs (e.g., through existing clinical communication research corpora), we pair them with the corresponding documentation.

2. **Prospective multimodal recordings.** Working with clinical partners through MIT Critical Data's network, we record a targeted sample of clinical encounters (with full informed consent and IRB approval) in at least two language contexts — English and one additional language (Portuguese via Brazil or Luganda via Uganda partnerships). Each encounter is analyzed in both its full multimodal form and its documented text form.

3. **Cross-linguistic comparison.** By conducting the study in two language contexts, we test whether the *pattern* of communicative loss differs across languages — whether different languages and clinical cultures lose different information at the documentation boundary.

**Analytical framework:** Per Urlaub leads the development of a **Communicative Content Analysis (CCA)** protocol — a systematic method for coding the communicative content of clinical encounters across modalities. The protocol identifies categories of clinically relevant communicative acts and tracks which survive the documentation boundary and which do not. Categories include:

- **Prosodic markers:** Pitch contours, speech rate changes, pauses, and vocal quality features that indicate uncertainty, distress, emphasis, or minimization
- **Paralinguistic signals:** Sighs, laughter, crying, throat clearing, silence duration — acts that carry affective and diagnostic information
- **Discourse structure:** How the conversation unfolds — topic initiation, interruptions, hedging, narrative sequencing — versus how it is documented
- **Relational dynamics:** Expressions of trust, hesitation, deference, or resistance that are legible in interaction but invisible in records

**Deliverables:**
- A validated CCA protocol applicable to clinical encounters in any language
- Quantified estimates of communicative information loss at the documentation boundary, broken down by category and language context
- Identification of specific clinical scenarios where the loss is greatest (we hypothesize: mental health assessment, pain evaluation, pediatric encounters, end-of-life conversations, and any encounter mediated by an interpreter)
- At least one empirical publication documenting these findings

### Study 2: The Undocumented Health Conversation (Months 3–10)
*Lead: Per Urlaub, with Leo Celi*

**Research question:** What clinically relevant communicative acts occur in community health conversations that exist entirely outside clinical documentation systems?

**Method:** Working with community health workers in MIT Critical Data's partner sites, we document and analyze health conversations that occur outside clinical encounters: family discussions about symptoms, community advice-giving, oral transmission of health knowledge, storytelling about illness and recovery. These conversations are recorded (with consent), transcribed, and analyzed using the CCA protocol developed in Study 1 — extended to capture narrative structure, communal reasoning, and intergenerational knowledge transmission.

This study addresses the second mechanism of the textual presumption: not what is lost when encounters are documented, but what is never captured because it occurs outside the clinical system entirely. We analyze:

- What health knowledge is communicated in these conversations (symptom interpretation, treatment decisions, prognostic reasoning, emotional regulation)
- What communicative modalities carry this knowledge (oral narrative, prosodic emphasis, communal deliberation)
- How this knowledge relates to formal clinical assessments — where it converges, diverges, or provides information unavailable through clinical channels
- Whether and how clinical AI systems could be designed to engage with this communicative domain, and what ethical constraints must govern such engagement

**Deliverables:**
- A documented corpus of community health conversations from at least two cultural/linguistic contexts
- Analysis of clinically relevant content in undocumented health communication
- Ethical framework for engaging with community health communication in AI development (building on Celi's BODHI principles and community-partnered research methodology)
- At least one empirical publication

### Synthesis: Framework, Convening, and Future Directions (Months 9–12)
*Lead: Joint*

The empirical findings from Studies 1 and 2 are synthesized into a **Communicative Health Framework** — a formal account of the communicative landscape of health that maps which domains clinical AI currently captures, which it misses, and what would be required to close the gap. The framework is organized along two axes: **modality** (text, prosodic, paralinguistic, narrative, somatic, musical, environmental) and **documentation status** (captured in clinical records, present in encounters but lost at documentation, occurring entirely outside clinical systems).

The framework is deliberately broader than what the empirical studies can validate in 12 months. This is by design: the studies establish rigorous evidence for two key domains (prosodic/paralinguistic features and undocumented oral narratives), while the framework maps the wider communicative territory — including musical, somatic, environmental, and ecological modalities — as an empirically motivated research agenda rather than a speculative claim.

The synthesis phase produces:

1. **A major framework paper** for a high-impact interdisciplinary venue, presenting the empirical findings and the broader communicative health framework. Grounded in evidence, honest about the boundary between what has been demonstrated and what requires further investigation.

2. **Design principles for communicatively expanded clinical AI** — concrete specifications for what data modalities, collection methods, and analytical approaches would be needed to build clinical AI systems that hear beyond text.

3. **A capstone convening at MIT: "The Languages of Healing"** (Month 11). This event brings together researchers, clinicians, community health workers, and practitioners from diverse healing traditions to present the findings, pressure-test the framework, and chart future research directions. Building on the January 15, 2026 event, the convening includes practitioners whose communicative modalities extend beyond the two studied — musicians, artists, indigenous knowledge keepers — to explore how the framework might extend to their domains. The convening is a dissemination and agenda-setting event grounded in the project's empirical results, not a substitute for methodology.

4. **A follow-on proposal** (targeting NIH, NSF, or Wellcome Trust) for a larger program that extends the empirical work to additional modalities and develops prototype AI systems informed by the framework.

---

## 4. Why This Team, Why MIT, Why Now

**Per Urlaub** (SHASS PI, Global Languages) brings expertise in applied linguistics, cross-cultural communication, and multiliteracies — the study of how meaning is constructed across semiotic systems. His work on meaning-making beyond text provides the theoretical foundation for the Communicative Content Analysis protocol and the broader framework. Linguistics is not a service discipline in this project — it provides the core analytical apparatus. The question *what counts as clinical communication?* is a linguistic question, and only a linguist can pose it with the necessary precision.

**Leo Anthony Celi** (Co-PI, IMES / MIT Critical Data) brings the clinical AI infrastructure — the MIMIC database, PhysioNet, and a global network of community partnerships in over 30 countries — along with deep expertise in healthcare AI equity. His BODHI framework (Bridging, Open, Discerning, Humble, Inquiring) provides the ethical architecture for community-engaged research. His DOJO initiative (Distributed Open Justice Oversight — community-operated adversarial testing for healthcare AI) provides a concrete platform for evaluating whether communicatively expanded inputs improve clinical AI performance. Celi's global network, which organized the January 15, 2026 MIT event with AMA support, enables the recruitment of community health workers and practitioners for Study 2 and the capstone convening.

**Why this collaboration is structurally necessary:** The two studies require both deep linguistic expertise (to develop the CCA protocol and analyze communicative features across languages) and clinical AI infrastructure (to connect the analysis to MIMIC data, care phenotype research, and global partnerships). A linguist alone could analyze clinical discourse but not connect it to AI systems being deployed worldwide. A clinical AI researcher alone could identify model failures but not trace them to specific communicative mechanisms. The SHASS contribution — redefining what counts as clinical communication — *is* the core intellectual move. The engineering and clinical infrastructure make it empirically testable and practically relevant.

**Why now:**

- Clinical AI systems are being deployed globally into communities where health communication extends far beyond text — making the textual presumption's consequences urgent and measurable
- The convergence of research on non-verbal clinical communication, narrative medicine, and AI fairness has created the intellectual preconditions for this synthesis, but no one has connected these fields to clinical AI architecture
- The January 15, 2026 convening demonstrated both the demand for and the feasibility of this interdisciplinary conversation
- The recognition that intelligence itself may be substrate-independent (Chen et al., *Nature* 650, 2026) opens conceptual space for taking seriously the idea that health-relevant communication may likewise be medium-independent — an argument this project tests empirically rather than merely asserting

---

## 5. Timeline, Budget, and Expected Impact

### Timeline

| Period | Activity | Lead |
|---|---|---|
| Months 1–2 | CCA protocol development; IRB submissions; data source identification; literature review | Joint |
| Months 2–4 | Study 1 begins: MIMIC paired analysis; prospective recording protocol established | Leo Celi / Per Urlaub |
| Months 3–6 | Study 2 begins: Community health conversation documentation in 2 partner sites | Per Urlaub / Leo Celi |
| Months 5–8 | Study 1 analysis: Cross-linguistic communicative loss quantification | Per Urlaub |
| Months 6–10 | Study 2 analysis: Undocumented health communication content analysis | Per Urlaub / Leo Celi |
| Months 9–11 | Framework synthesis; paper drafting | Joint |
| Month 11 | **MIT Capstone Convening: "The Languages of Healing"** | Joint |
| Month 12 | Design principles; follow-on proposal submission | Joint |

### Budget: $180,000 (direct costs)

| Category | Amount | Notes |
|---|---|---|
| Postdoctoral researcher (clinical linguistics / multimodal discourse analysis) | $65,000 | 60% FTE, joint supervision — leads CCA protocol development and both study analyses |
| Graduate research assistant (SHASS — linguistic analysis) | $25,000 | Study 1 coding and cross-linguistic analysis |
| Prospective clinical encounter recording (Study 1) | $15,000 | Recording equipment, consent coordination, transcription at 2 sites |
| Community health conversation documentation (Study 2) | $20,000 | Field recording, community compensation, transcription/translation across 2 partner sites |
| Computational analysis (MIMIC/PhysioNet) | $10,000 | Computing resources, NLP tools for paired text-audio analysis |
| Capstone Convening: "The Languages of Healing" | $20,000 | Travel support for 15–20 participants including international community practitioners; 2-day event at MIT |
| Translation, interpretation, and accessibility | $10,000 | |
| Publication (open access) and dissemination | $5,000 | |
| PI summer salary support | $10,000 | |

**Supplemental requests:** 2 UROPs (one in linguistics/discourse analysis, one in CS/NLP); part-time use of Building 16 collaborative space.

### Expected Impact

**Empirical:** The first systematic, cross-linguistic quantification of communicative information loss at the clinical documentation boundary. This finding alone has immediate relevance for clinical AI developers, regulators, and health equity advocates — it transforms "text-based AI misses things" from a general intuition into a demonstrated, measurable fact.

**Methodological:** A validated Communicative Content Analysis protocol that can be applied to clinical encounters in any language — a reusable tool for the growing community of researchers studying multimodal clinical communication.

**Theoretical:** The Communicative Health Framework — a formal map of the communicative landscape of health, grounded in empirical evidence for two key domains and extending as a motivated research agenda to additional modalities. This framework provides the conceptual architecture for a new generation of clinical AI systems that attend to more than text.

**For global health equity:** Concrete evidence that clinical AI's textual foundation systematically disadvantages communities whose health communication is oral, prosodic, or communal — and design principles for building systems that do not.

**Transformative potential:** This project moves clinical AI fairness beyond its current focus on which languages are represented to the deeper question of which communicative modalities are heard at all. It positions MIT at the leading edge of a paradigm shift: from asking *how do we make AI speak more languages?* to asking *how do we make AI listen?*

---

### Selected References

Ambady, N. et al. "Surgeons' tone of voice: A clue to malpractice history." *Surgery* 132(1), 5–9 (2002).

Charon, R. *Narrative Medicine: Honoring the Stories of Illness.* Oxford University Press (2006).

Chen, E.K., Belkin, M., Bergen, L. & Danks, D. "Does AI already have human-level intelligence? The evidence is clear." *Nature* 650, 36–40 (2026).

Celi, L.A. et al. "Sources of bias in artificial intelligence that perpetuate healthcare disparities." *PLOS Digital Health* 1(3), e0000022 (2022).

Heritage, J. & Maynard, D.W. *Communication in Medical Care: Interaction Between Primary Care Physicians and Patients.* Cambridge University Press (2006).

Hobbs, P. "The role of progress notes in the professional socialization of medical residents." *Journal of Pragmatics* 35(9), 1323–1344 (2003).

Kleinman, A. *The Illness Narratives: Suffering, Healing, and the Human Condition.* Basic Books (1988).

Koss-Chioino, J.D. "Spiritual transformation, relation, and radical empathy: Core components of the ritual healing process." *Transcultural Psychiatry* 43(4), 652–670 (2006).

Mattingly, C. *Healing Dramas and Clinical Plots: The Narrative Structure of Experience.* Cambridge University Press (1998).

Patel, V.L., Arocha, J.F. & Kushniruk, A.W. "Patients' and physicians' understanding of health and biomedical concepts." *Journal of Biomedical Informatics* 35(1), 8–16 (2002).

Roter, D.L. & Hall, J.A. *Doctors Talking with Patients/Patients Talking with Doctors.* 2nd ed. Praeger (2006).

World Health Organization. *One Health Joint Plan of Action 2022–2026.* WHO (2022).
