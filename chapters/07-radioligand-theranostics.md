# Radioligand Theranostics

## Learning Objectives

By the end of this chapter you should be able to:

- **Define** a theranostic agent and explain how the "image-then-treat" loop uses one targeting principle for both diagnosis and therapy.
- **Trace** the PSMA theranostic pair for prostate cancer — gallium-68/fluorine-18 PSMA PET for imaging, lutetium-177-PSMA-617 for therapy — and explain why the imaging step is a true companion diagnostic, not a formality.
- **Compare** beta-emitters and alpha-emitters by range, linear energy transfer (LET), and the crossfire/bystander consequence, and choose between them for a given tumor geometry.
- **Explain** why off-target uptake (salivary glands, kidneys) sets the dose-limiting toxicity of PSMA radioligand therapy, and connect this to absorbed dose.
- **Critique** a radioligand claim by distinguishing "the target is present on the image" from "the therapy will deliver a lethal absorbed dose to those cells."

## Opening Case

A man with metastatic, castration-resistant prostate cancer has exhausted standard options. His oncologist has heard that lutetium-177-PSMA-617 (Pluvicto) extends survival in this setting and wants to give it. The temptation is to treat on the basis of the diagnosis alone — "it's prostate cancer, the drug is for prostate cancer, give it."

But the team first performs a **PSMA PET scan**, imaging the same target the therapy will exploit. On most patients this lights up bright: the metastases express prostate-specific membrane antigen abundantly, and they are good candidates. On *this* patient, several large, symptomatic lesions show almost no PSMA signal — they have dedifferentiated and lost the target. Had the team treated on diagnosis alone, they would have irradiated his salivary glands and kidneys (which *do* express PSMA) while the lesions causing his symptoms received little therapeutic radiation. The drug would have delivered toxicity without benefit to exactly the tumors that mattered.

The PSMA scan is not a formality before treatment; it *is* the patient-selection step, and it works because the imaging agent and the therapeutic agent target the same molecule. This chapter is about that design — the cleanest, most clinically successful idea in cancer nanomedicine — and about why "the target is on the image" is necessary but not the whole story.

## Core Concepts

### Theranostics and the image-then-treat loop

Plain language: a theranostic agent both finds the tumor and treats it, using the same molecular handle for both. You image to confirm the handle is there, then deliver therapy through the same handle.

Formal definition: **theranostics** combines therapy and diagnostics in a single molecular framework — "the molecule used for imaging is the same molecule (or a sister molecule) used for therapy," so the same molecular event (target binding) drives both diagnosis and treatment (cba-48). Conventional care separates them: a patient is imaged with one agent and treated with an unrelated drug, and the information flows one way (cba-48). In theranostics the loop closes: imaging confirms which patients have the target, the therapy delivers payload through that target, and post-therapy imaging confirms delivery and predicts response (cba-48).

The cleanest realization is **radioligand therapy**: a small targeting molecule (the **ligand**) carries a radioisotope. Swap the imaging isotope for a therapeutic isotope on the same ligand, and you have a matched diagnostic/therapeutic pair (cba-48).

<!-- → [DIAGRAM: radioligand theranostic image-then-treat loop. A circular flow: (1) inject diagnostic radioligand (e.g., Ga-68-PSMA-11) → (2) PET scan confirms target expression → (3) if positive, inject therapeutic radioligand (same ligand, e.g., Lu-177-PSMA-617) → (4) the emitted radiation kills bound cells + crossfire → (5) post-therapy imaging confirms delivery → loop back to assess response. Center label: SAME TARGET, two isotopes.] -->

### The PSMA pair: a companion diagnostic by construction

Plain language: prostate cancer cells carry a surface protein, PSMA. Tag a PSMA-binding molecule with an imaging isotope to find the cancer; tag the same molecule with a killing isotope to treat it.

Formal definition: **prostate-specific membrane antigen (PSMA)** is a transmembrane protein expressed at high levels on prostate cancer cells, with expression correlating with disease aggressiveness and detectable on nearly all metastatic prostate cancer (cba-48). The matched pair (cba-48):

- **Imaging:** small molecules binding PSMA's active site, radiolabeled for **PET** — **gallium-68-PSMA-11** (Locametz, Illuccix) and **fluorine-18-DCFPyL / piflufolastat F-18** (Pylarify), both FDA-approved for prostate cancer staging and restaging (cba-48). PSMA PET is "dramatically more sensitive than conventional imaging (CT, bone scan)" for recurrence and metastasis (cba-48).
- **Therapy:** the same targeting molecule loaded with a therapeutic isotope — **lutetium-177-PSMA-617 (Pluvicto)**, FDA-approved 2022 for PSMA-positive metastatic castration-resistant prostate cancer (mCRPC) that has progressed on a taxane and an androgen-receptor-pathway inhibitor (cba-48).

Because the imaging and the therapy share the targeting molecule, the PSMA PET scan is a **companion diagnostic integrated into the therapy** (cba-48) — the basis of the opening-case patient selection. The pivotal **VISION trial** showed improved overall survival with Lu-177-PSMA-617 plus best supportive care versus best supportive care alone in heavily pretreated mCRPC (cba-48) [verify trial specifics against primary report].

A second established pair targets a different cancer: **lutetium-177-DOTATATE (Lutathera)**, FDA-approved 2018 for gastroenteropancreatic neuroendocrine tumors, where the ligand (octreotate, a somatostatin analog) binds **somatostatin receptor type 2 (SSTR2)**, imaged with **gallium-68-DOTATATE PET** (cba-48). DOTATATE was "the first FDA-approved radioligand theranostic in [the] modern era and established the regulatory pathway" (cba-48).

### Beta versus alpha emitters: range, LET, and crossfire

Plain language: the killing isotope can fling electrons that travel a few millimeters, or helium nuclei that travel a few cell-widths but hit much harder. The choice tunes how far the damage spreads and how lethal each hit is.

Two emitter classes dominate (cba-48):

- **Beta-emitters** release electrons of intermediate energy and **millimeter range**. **Lutetium-177** is the most clinically used; **yttrium-90** has higher energy and longer range; **iodine-131** is the classic thyroid agent (cba-48). The long range produces **crossfire** — a cell without the target can still be killed by radiation from a neighbor that bound the ligand — which helps in tumors with **heterogeneous target expression** (cba-48). The cost: **lower linear energy transfer (LET)** means each track deposits less energy, so more potential for resistance, and the longer range can damage adjacent normal tissue (cba-48).
- **Alpha-emitters** release helium nuclei (2 protons + 2 neutrons) of very high energy and **very short range (50–100 micrometers — a few cell diameters)**. **Actinium-225** is the leading clinical candidate; **radium-223 (Xofigo)** is approved for prostate cancer bone metastases (cba-48). The very high LET deposits enormous energy over a short path — far more lethal DNA damage per particle — and may **overcome resistance** to beta therapy; the short range minimizes off-target damage (cba-48). The cost: harder to produce (especially Ac-225), more expensive, less clinical experience (cba-48).

Formal definitions. **Linear energy transfer (LET)** is the energy deposited per unit path length by a particle as it travels through tissue; high-LET radiation (alpha) causes dense, hard-to-repair DNA double-strand breaks, while low-LET radiation (beta) causes sparser damage. **Absorbed dose** is the energy deposited per unit mass of tissue (measured in gray, Gy); the therapeutic logic of radioligand therapy is to deliver a lethal absorbed dose to target-expressing cells while keeping the absorbed dose to normal organs below their tolerance.

<!-- → [DIAGRAM: beta vs alpha emitter comparison. Left: a beta-emitter (Lu-177) on a tumor cell, electron track ~mm crossing several cells including a target-negative one (crossfire kills it); label "low LET, long range, crossfire helps heterogeneity." Right: an alpha-emitter (Ac-225) on a tumor cell, dense short track ~50-100 µm causing clustered double-strand breaks in 1-2 cells; label "high LET, short range, more lethal, less crossfire." Scale bar in micrometers.] -->

### Off-target uptake sets the dose limit

Plain language: PSMA is not only on cancer. The salivary glands and kidneys carry it too, so they soak up radiation, and how much they can tolerate caps the dose.

The toxicities of Lu-177-PSMA-617 follow directly from where PSMA is expressed off-tumor: **xerostomia** (dry mouth, from salivary-gland uptake — PSMA is expressed on salivary glands), **kidney toxicity** (PSMA on renal tubules), bone-marrow suppression, and fatigue (cba-48). This is the radioligand version of the delivery-chain discipline: the absorbed dose to these normal organs, not to the tumor, sets the ceiling. You cannot simply give more isotope to kill resistant lesions; you give more and you cross the salivary/renal tolerance first. This is precisely why the opening-case patient — whose symptomatic lesions had *lost* PSMA — would have been harmed: the dose would have concentrated in PSMA-positive normal organs while sparing the target-negative tumor.

## Worked Example

**Situation.** A patient with mCRPC has a PSMA PET scan. Most lesions are strongly PSMA-positive, but a few bulky, symptomatic lesions show only faint PSMA uptake on the *outer rim* with cold centers, suggesting heterogeneous target expression within those tumors. You can offer beta-emitter therapy (Lu-177-PSMA-617, available, approved) or enroll the patient in an alpha-emitter trial (Ac-225-PSMA, investigational). Which physics fits this tumor geometry?

**Reasoning — including a dead end.** First instinct: alpha-emitters are "more powerful" — very high LET, more lethal per hit, can overcome resistance (cba-48) — so use the alpha-emitter for the stubborn bulky lesions. That reasoning fixates on per-particle lethality and ignores *geometry*. The bulky lesions are **heterogeneous**: many cells inside them express little or no PSMA. An alpha-emitter's range is only **50–100 micrometers** (cba-48) — a few cell widths. A decay event bound to a rim cell deposits its lethal energy within those few cells and cannot reach the target-negative cells deeper in the lesion. The "more powerful" isotope would sterilize the PSMA-positive rim and leave the PSMA-negative core untouched. Per-hit lethality does not substitute for reach when the target is patchy.

**Resolution.** For a *heterogeneous bulky* lesion, the **beta-emitter's longer (millimeter) range and crossfire** are the relevant advantage: radiation from PSMA-positive cells can kill nearby PSMA-negative cells the alpha-emitter never reaches (cba-48). So Lu-177 is the better physics for these lesions. The alpha-emitter's strengths — overcoming resistance, sparing normal tissue with its short range — shine in **micrometastatic or uniformly target-positive** disease, or as a strategy when beta therapy has failed (cba-48). The correct question is never "which isotope is stronger" but "which range matches the spatial distribution of the target."

**The lesson.** Range and LET are design parameters matched to tumor geometry, not a ranking. Crossfire (beta) buys reach into heterogeneous tumors; high LET (alpha) buys lethality and resistance-breaking in compact, target-rich disease.

**The limit.** Crossfire is double-edged: the same millimeter range that reaches a target-negative tumor cell also irradiates adjacent normal tissue, and the beta-emitter's lower LET means some resistant clones survive (cba-48). And neither isotope helps if the lesion is genuinely PSMA-negative throughout — the opening-case scenario — because there is nothing to bind and crossfire needs *some* bound source nearby. Theranostics treats target-positive disease; it does not rescue target-loss.

## Common Misconceptions

**"If it's prostate cancer, the prostate-cancer radioligand will work."** Plausible — the drug is indicated for prostate cancer. It fails because radioligand therapy requires the *target*, not the diagnosis: lesions that have dedifferentiated and lost PSMA receive little therapeutic radiation, while PSMA-positive normal organs receive the dose (cba-48). The PSMA PET scan is the selection step precisely to catch this — the opening case (cba-48).

**"Alpha-emitters are simply better because they hit harder."** Plausible — high LET means more lethal DNA damage per particle (cba-48). It fails because the alpha-emitter's **50–100 µm range** cannot reach target-negative cells in a heterogeneous tumor, where the beta-emitter's millimeter crossfire can (cba-48). "Harder" is not "farther"; the right choice depends on tumor geometry.

**"A bright PSMA PET scan means the therapy will cure those lesions."** Plausible — uptake confirms the target. It fails because uptake confirms *binding*, not lethal **absorbed dose**: dose is capped by salivary-gland and kidney tolerance, and resistant clones (especially under low-LET beta radiation) can survive (cba-48). "Target present on the image" is necessary, not sufficient — the same proxy-vs-truth gap that runs through this book (pantry notes, ch. 07).

**"Theranostics is just a fancy name for using imaging before treatment."** Plausible — imaging does precede treatment. It fails because in true theranostics the imaging and therapeutic agents share the *same targeting molecule*, so the scan is a genuine companion diagnostic for *that* therapy, not a generic staging step (cba-48). A CT before chemotherapy is not theranostic; Ga-68-PSMA PET before Lu-177-PSMA-617 is.

## Exercises

1. **(Understand)** Draw the image-then-treat loop for the PSMA pair, naming the specific imaging agents (Ga-68-PSMA-11 or F-18-DCFPyL), the therapeutic agent (Lu-177-PSMA-617), and the shared target. State at each step what decision the step informs (cba-48).

2. **(Apply)** A patient's neuroendocrine tumor is being considered for Lu-177-DOTATATE. Which companion diagnostic confirms eligibility, what receptor does the ligand bind, and what does a negative scan imply about treating on diagnosis alone? Map this onto the PSMA logic (cba-48).

3. **(Apply+ / Analyze)** Two patients with mCRPC are PSMA-positive. Patient A has widespread *micrometastatic*, uniformly PSMA-bright disease; Patient B has a few *bulky, heterogeneous* lesions with cold centers. Recommend beta- vs. alpha-emitter therapy for each, and justify each choice in terms of range, LET, and crossfire. State explicitly why the "stronger isotope" intuition gives the wrong answer for one of them (cba-48).

4. **(Create — produce something)** Produce a one-page **absorbed-dose budget** sketch for Lu-177-PSMA-617. List the tissues that take up the radioligand (tumor; and off-target: salivary glands, kidneys, marrow), and for each write whether its absorbed dose is the *goal* or a *constraint*. Then write a short rule, in your own words, for how the salivary/renal tolerance caps the deliverable tumor dose, and how this would change for an alpha-emitter with shorter range (cba-48).

5. **(Evaluate)** A company claims its new radioligand "guarantees tumor-selective killing because the PET scan proves the target is there." Write three questions that separate "target present on the image" from "lethal absorbed dose delivered to those cells," referencing off-target uptake, absorbed dose, and emitter LET (cba-48).

## What Would Change My Mind

The chapter's central claim is that radioligand theranostics succeeds — clinically, where many elegant nanoparticles have not — *because* its companion-diagnostic loop is built from a single shared targeting molecule, making patient selection mechanistic rather than statistical, and that emitter choice (beta vs. alpha) must be matched to tumor geometry rather than ranked by per-particle power. What would revise this: rigorous data showing that **treating PSMA-PET-negative or low patients with Lu-177-PSMA-617 produces survival benefit comparable to PSMA-positive patients** — that is, that the companion-diagnostic selection adds little — would undercut the claim that the shared-target loop is the engine of success. Likewise, a controlled comparison showing **alpha-emitters outperform beta-emitters even in demonstrably heterogeneous bulky tumors** (where crossfire should favor beta) would overturn the geometry-matching argument. To date the evidence supports both: target-confirmed selection and emitter-geometry matching are why the field works (cba-48). I would also revise if the VISION-class survival benefit failed to replicate in confirmatory trials [verify].

## Still Puzzling

- **How precisely can we measure tumor absorbed dose in a patient, in real time?** Dosimetry from post-therapy imaging exists, but per-lesion absorbed-dose measurement that could individualize dosing is still maturing [verify].
- **Will the Ac-225 supply chain scale?** Alpha-emitter promise is real, but actinium-225 is hard to produce; whether supply can meet demand is an open practical constraint (cba-48).
- **How low can PSMA expression go and still benefit?** PSMA PET gives a yes/no-ish picture, but the threshold of expression that predicts therapeutic benefit — the analog of "HER2-low" for ADCs — is not crisply defined [verify].
- **Why does this simpler design translate when multifunctional nanoparticles mostly don't?** Radioligands are arguably *less* sophisticated than the engineered particles of the next chapter, yet far more of them reach the clinic. The next chapter takes up that paradox directly.

## References

- Source chapter: cba-48, "Theranostics and Emerging Cancer Nanotechnology" (Humanitarians AI archive). Primary source for the theranostic definition, the PSMA and DOTATATE pairs, named agents (Ga-68-PSMA-11, F-18-DCFPyL, Lu-177-PSMA-617, Ga-68/Lu-177-DOTATATE, Ra-223, Ac-225), the VISION trial, beta vs. alpha emitter physics, and PSMA off-target toxicity.
- Research notes: `pantry/07-radioligand-theranostics_notes.md` (target-confirmed therapy; proxy-vs-truth failure mode; delivery-as-mechanism framing).
- NCI, *CT Scans and Cancer Fact Sheet*. https://www.cancer.gov/about-cancer/diagnosis-staging/ct-scans-fact-sheet — radiopharmaceuticals and PSMA imaging-agent context.
- NCI, *Theranostics and AI in Cancer Precision Medicine*. https://www.cancer.gov/about-nci/organization/cbiit/news-events/blog/2023/theranostics-and-ai-next-advance-cancer-precision-medicine — theranostics, PET/CT/MRI, molecular diagnostics, targeted therapeutics.

Note: trial-level details (VISION design and outcomes, exact approval indications and dates) are flagged `[verify]` where the cba-48 source states them; confirm against primary trial publications and current FDA labels before publication.

## Prompts

*No figures have been generated for this chapter yet.*
