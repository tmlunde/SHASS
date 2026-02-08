# The Languages of Healing: What Clinical AI Cannot Hear

**A Proposal to the SHASS+ Connectivity Fund (Full Proposal)**

**PI:** Per Urlaub, Global Languages, SHASS
**Co-PI:** Leo Anthony Celi, Laboratory for Computational Physiology (IMES) / MIT Critical Data

---

## 1. What Goes Unheard

Science establishes truth through proof. This is its great strength — and its blind spot. What has not been proven is not thereby false. It may simply mean we have not yet looked, or that we have been looking with instruments too narrow to detect what is there. Research on infant cry acoustics has demonstrated that spectral and temporal features of a child's cry carry information about neurological status, pain severity, and disease state — information that experienced caregivers have long detected intuitively and that computational analysis has begun to validate (LaGasse et al., 2005; Manfredi et al., 2009). A community health worker in São Paulo who assesses a child through the timber of the mother's voice and the way the child shifts on her lap is processing diagnostic information that vanishes the moment it enters a medical record as text. These are not exceptions. They are illustrations of a general pattern: clinical encounters are rich, multimodal communicative events, and the text record captures only a fraction of what occurs.

The fact that these communicative dimensions have not been systematically integrated into clinical AI does not mean they lack clinical value. It means we built our systems without listening for them.

On January 15, 2026, we convened approximately 100 participants from diverse backgrounds — clinicians, linguists, AI researchers, ethicists, indigenous knowledge keepers, artists, students — at MIT, with support from the American Medical Association, to ask a question that clinical AI has not yet seriously confronted: *what are the languages of healing, and how many of them can our systems actually hear?* The answer that emerged was stark: clinical AI, as currently built, captures almost none of them.

Clinical artificial intelligence is built on a narrow communicative foundation: typed text in electronic health records, overwhelmingly in English. The global movement toward "multilingual clinical AI" seeks to broaden this by adding more languages — a necessary effort. But it misses a more fundamental problem. Adding more languages to a text-based system is like adding more microphones inside a recording studio while the concert is happening outdoors. The problem is not which languages are represented. The problem is what we have decided counts as clinical language at all.

**The question this project poses — and empirically tests — is: how much clinically relevant communicative information is lost when the clinical encounter is reduced to text?**

This is not a new question in the abstract. A substantial body of research in non-verbal communication, clinical linguistics, and medical anthropology has long documented that paralinguistic cues, body language, and narrative context matter in clinical encounters (Roter & Hall, 2006; Heritage & Maynard, 2006; Mattingly, 1998). What *is* new — and what creates the urgency for this project — is the emergence of clinical AI systems that are being deployed globally on the basis of text alone, at a scale and speed that amplifies the textual reduction from an individual clinical limitation into a systematic, structural one. Every clinical AI system trained on medical records inherits and entrenches the assumption that what was documented is what matters. As these systems reach communities where health knowledge is transmitted orally, prosodically, or through embodied practice, the consequences of this assumption become acute.

This project answers that question. We conduct the first systematic study of **communicative information loss at the documentation boundary** in clinical encounters — measuring what is present in the full multimodal encounter that disappears when it becomes a medical record. We focus on two domains where the loss is likely greatest and most consequential: **prosody and paralinguistic features** (what text strips from speech) and **undocumented oral health narratives** (health communication that occurs entirely outside clinical records). We conduct this analysis in two language contexts — English and one additional language — to generate initial evidence on whether the pattern of loss varies across clinical cultures. The findings will establish an empirical foundation for rethinking what clinical AI needs to hear — and provide concrete design principles for building systems that can.

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

We propose a program with two empirical studies and one synthesis component, designed to produce measurable findings, a validated analytical methodology, and a theoretical framework — grounding the broader vision in concrete results. We present a 12-month timeline below, but note that the SHASS+ Fund permits spreading one year of funding over 18–24 months. We are prepared to use an 18-month timeline if IRB processes or postdoc recruitment require it, which would strengthen rather than weaken the empirical work. Pre-submission consultations with the MIT IRB (for Study 1's US recordings) and with local ethics review contacts at our Brazil and Uganda partner sites (for Study 2) are underway; the timeline below reflects an optimistic but realistic projection based on these conversations.

### Study 1: Quantifying Communicative Loss at the Documentation Boundary (Months 1–8)
*Lead: Per Urlaub and Leo Celi (joint)*

**Research question:** How much clinically relevant communicative information is present in the full multimodal clinical encounter but absent from the corresponding text record?

**Method and data sources:** The core design is a paired comparison: record clinical encounters in full multimodal form (audio at minimum, video where feasible), then compare the communicative content of the recording against the clinician's corresponding text documentation. The primary data source is prospective:

**Prospective multimodal recordings (primary).** Working with clinical partners through MIT Critical Data's network, we record 40–60 clinical encounters (with full informed consent and IRB approval) across two language contexts: English (at a US partner site) and one additional language — Portuguese (via existing Brazil partnerships) or Luganda (via Uganda partnerships). The target of 20–30 encounters per language context provides sufficient material for the CCA protocol to identify patterns of communicative loss while remaining feasible within the project timeline and budget. Each encounter is analyzed in both its full recorded form and its corresponding text documentation.

**Existing clinical communication corpora (supplementary).** Several research groups have assembled recorded clinical encounter datasets for communication research (e.g., the Verilogue physician-patient dialogue database; recorded encounters from medical education programs). Where accessible, we use these to expand the English-language sample and test the CCA protocol on encounters not collected by our team, strengthening the protocol's generalizability.

**MIMIC/PhysioNet contextual analysis.** While MIMIC does not contain encounter audio, its extensive clinical notes provide the landscape against which our findings are interpreted. We use MIMIC to characterize the documentation patterns (note structure, content categories, information density) that our recorded encounters are compared against, and to test whether NLP-detectable features of notes (hedging, uncertainty markers, affective language) correlate with the prosodic and paralinguistic features identified in our recorded sample.

By conducting the study across two language contexts, we generate initial evidence on whether the pattern of communicative loss differs across clinical cultures — recognizing that two languages provide a meaningful paired comparison but not a generalizable claim. The cross-linguistic dimension is framed as hypothesis-generating for a larger follow-on study.

**Analytical framework:** Per Urlaub leads the development of a **Communicative Content Analysis (CCA)** protocol — a systematic method for coding the communicative content of clinical encounters across modalities. The protocol identifies categories of clinically relevant communicative acts and tracks which survive the documentation boundary and which do not. Categories include:

- **Prosodic markers:** Pitch contours, speech rate changes, pauses, and vocal quality features that indicate uncertainty, distress, emphasis, or minimization
- **Paralinguistic signals:** Sighs, laughter, crying, throat clearing, silence duration — acts that carry affective and diagnostic information
- **Discourse structure:** How the conversation unfolds — topic initiation, interruptions, hedging, narrative sequencing — versus how it is documented
- **Relational dynamics:** Expressions of trust, hesitation, deference, or resistance that are legible in interaction but invisible in records

**CCA validation:** The protocol is validated through a structured inter-rater reliability process. Following initial development by the postdoc and PI Urlaub, two independent coders (the graduate RA and one additional trained coder) apply the CCA to a subset of 10 encounters. We measure inter-rater agreement using Cohen's kappa, with a target of κ ≥ 0.70 for each coding category. Categories falling below this threshold are iteratively refined — through discussion, exemplar coding, and category redefinition — until acceptable reliability is achieved. This process is documented as part of the protocol itself, making the validation methodology transparent and replicable by other research groups.

**Deliverables:**
- A validated CCA protocol with documented inter-rater reliability, applicable to clinical encounters in any language
- Quantified estimates of communicative information loss at the documentation boundary, broken down by category and language context
- Identification of specific clinical scenarios where the loss is greatest (we hypothesize: mental health assessment, pain evaluation, pediatric encounters, end-of-life conversations, and any encounter mediated by an interpreter)
- At least one empirical publication documenting these findings

### Study 2: The Undocumented Health Conversation (Months 3–10)
*Lead: Per Urlaub, with Leo Celi*

**Research question:** What clinically relevant communicative acts occur in community health conversations that exist entirely outside clinical documentation systems?

**Method and sample:** Working with community health worker (CHW) networks in MIT Critical Data's partner sites in Brazil and Uganda, we use purposive sampling to record 30–40 community health conversations (15–20 per site) that occur outside clinical encounters. CHWs identify and recruit participants engaged in naturally occurring health communication: family discussions about symptoms or treatment decisions, community advice-giving following a health event, intergenerational transmission of health knowledge, and storytelling about illness and recovery. Conversations are audio-recorded with informed consent, transcribed, translated where necessary, and analyzed using the CCA protocol developed in Study 1 — extended to capture narrative structure, communal reasoning, and intergenerational knowledge transmission.

This study addresses the second mechanism of the textual presumption: not what is lost when encounters are documented, but what is never captured because it occurs outside the clinical system entirely.

**What counts as a finding:** For each recorded conversation, we code whether it contains clinically relevant content in four domains: (1) symptom interpretation or health assessment, (2) treatment reasoning or decision-making, (3) prognostic or preventive reasoning, (4) emotional regulation or psychosocial support related to health. We then assess: what proportion of these conversations contain clinically relevant content that does not appear in any corresponding clinical record for the individuals involved? Where participants have concurrent clinical records (through CHW documentation or facility records), we conduct a direct comparison. Where they do not — which we expect to be common — the absence of any clinical record *is itself the finding*: clinically relevant communication that is entirely invisible to documentation systems.

We further analyze:

- What communicative modalities carry this knowledge (oral narrative, prosodic emphasis, communal deliberation, embodied demonstration)
- Whether the content converges with, diverges from, or supplements formal clinical assessments
- What ethical constraints must govern any engagement of clinical AI with community health communication — particularly regarding consent, surveillance risk, and the right to communicative privacy

**Deliverables:**
- A documented and coded corpus of 30–40 community health conversations from two cultural/linguistic contexts
- Quantified analysis of clinically relevant content in undocumented health communication, broken down by domain and modality
- Ethical framework for engaging with community health communication in AI development (building on Celi's BODHI principles and community-partnered research methodology)
- At least one empirical publication

### Synthesis: Framework, Convening, and Future Directions (Months 9–12)
*Lead: Joint*

The empirical findings from Studies 1 and 2 are synthesized into a **Communicative Health Framework** — a formal account of the communicative landscape of health that maps which domains clinical AI currently captures, which it misses, and what would be required to close the gap. The framework is organized along two axes: **modality** (text, prosodic, paralinguistic, narrative, somatic, musical, environmental) and **documentation status** (captured in clinical records, present in encounters but lost at documentation, occurring entirely outside clinical systems).

The framework is deliberately broader than what the empirical studies can validate in 12 months. This is by design: the studies establish rigorous evidence for two key domains (prosodic/paralinguistic features and undocumented oral narratives), while the framework maps the wider communicative territory — including musical, somatic, environmental, and ecological modalities — as an empirically motivated research agenda rather than a speculative claim.

**If the findings are null — if text captures more communicative content than hypothesized — this is equally valuable.** A finding that documentation preserves most clinically relevant information would provide the first empirical validation of the textual foundation on which clinical AI currently rests. More likely, we expect the degree of loss to vary substantially by encounter type and communicative category, which would allow us to identify *where* the textual presumption is most costly (we hypothesize: mental health, pain, pediatrics, end-of-life, interpreter-mediated encounters) and where text-based AI may be adequate. Either outcome informs clinical AI design; only the absence of measurement leaves the field guessing.

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
- The convergence of research on non-verbal clinical communication, narrative medicine, and AI fairness has created the intellectual preconditions for this synthesis, but no one has yet connected these fields to clinical AI architecture — the gap this project fills
- The January 15, 2026 convening at MIT demonstrated both the demand for and the feasibility of this interdisciplinary conversation
- More broadly, the growing recognition that intelligence and communication may take forms very different from those assumed in Western computational traditions (Chen et al., *Nature* 650, 2026) is creating intellectual openness to re-examining what clinical AI treats as given — an openness this project channels into empirical research

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
| Postdoctoral researcher (clinical linguistics / multimodal discourse analysis) | $65,000 | 60% FTE, joint supervision — leads CCA protocol development and Study 1 analysis. Recruitment begins immediately upon award; both PIs have identified candidates through existing networks in clinical linguistics. If recruitment is delayed, the 18-month timeline option absorbs the gap, and PIs lead initial CCA development directly. |
| Graduate research assistant (SHASS — linguistic analysis) | $25,000 | Study 1 inter-rater coding, cross-linguistic analysis, and primary coding responsibility for Study 2 — distributing analytical load across the team |
| Prospective clinical encounter recording (Study 1) | $15,000 | Recording equipment, consent coordination, transcription at 2 sites |
| Community health conversation documentation (Study 2) | $25,000 | Field recording equipment, local research coordinator support at each site, community compensation for participants (co-designed with local partners following BODHI principles), and transcription/translation across 2 partner sites |
| Computational analysis (MIMIC/PhysioNet) | $10,000 | Computing resources, NLP tools for paired text-audio analysis |
| Capstone Convening: "The Languages of Healing" | $15,000 | Travel support for 12–15 participants including international community practitioners; 2-day event at MIT |
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

LaGasse, L.L., Neal, A.R. & Lester, B.M. "Assessment of infant cry: Acoustic cry analysis and parental perception." *Mental Retardation and Developmental Disabilities Research Reviews* 11(1), 83–93 (2005).

Manfredi, C. et al. "Criteria for estimating fundamental frequency of infant cry." *Journal of Voice* 23(2), 128–137 (2009).

Mattingly, C. *Healing Dramas and Clinical Plots: The Narrative Structure of Experience.* Cambridge University Press (1998).

Patel, V.L., Arocha, J.F. & Kushniruk, A.W. "Patients' and physicians' understanding of health and biomedical concepts." *Journal of Biomedical Informatics* 35(1), 8–16 (2002).

Roter, D.L. & Hall, J.A. *Doctors Talking with Patients/Patients Talking with Doctors.* 2nd ed. Praeger (2006).

World Health Organization. *One Health Joint Plan of Action 2022–2026.* WHO (2022).
