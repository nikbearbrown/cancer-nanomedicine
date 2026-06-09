# Targeting: EPR, Protein Corona, and Active Ligands

## Learning Objectives

By the end of this chapter you should be able to:

- **Explain** the EPR (enhanced permeability and retention) effect as the basis of *passive* targeting, and articulate honestly why its reliability in human tumors is contested.
- **Distinguish** passive targeting (EPR) from active targeting (surface ligands) and explain why adding a ligand improves cellular *uptake* without necessarily improving tumor *accumulation*.
- **Describe** the protein corona — the layer of biomolecules that coats a nanoparticle in blood — and explain how it can mask targeting ligands and redirect particle fate.
- **Interpret** the ~0.7% median tumor-delivery statistic (Wilhelm et al., 2016) and the critiques of EPR (Nichols & Bae) without either dismissing nanomedicine or overstating its targeting.
- **Critique** a targeting claim by identifying which step of the delivery chain the targeting strategy actually affects.

## Opening Case

A biotech company designs a nanoparticle decorated with antibodies against HER2, a receptor overexpressed on some breast cancers. In the lab, the targeted particle binds HER2-positive cells beautifully and is taken up at many times the rate of an untargeted control. The story writes itself: the antibody steers the particle to the tumor. The company raises money on the strength of "active tumor targeting."

In the animal study, the targeted and untargeted particles accumulate in the tumor at nearly the *same* total amount. The targeting antibody, so decisive in a dish, made almost no difference to how much drug reached the tumor. Two things had gone wrong with the company's mental model. First, the antibody acts only at the final step — cellular uptake — and only *after* the particle has already arrived; it does nothing to get the particle to the tumor in the first place. Second, the moment the particle entered blood, plasma proteins swarmed its surface and formed a coating — a **protein corona** — that buried many of the antibodies, blunting the targeting they had engineered so carefully.

The company had confused *binding cells in a dish* with *reaching a tumor in a body*. This chapter is about that gap — about what targeting can and cannot do, and about the honest, unsettled state of the central idea the whole field was built on.

## Core Concepts

### Passive targeting and the EPR effect

Plain language: tumors have leaky blood vessels and bad drainage, so nanoparticles tend to drift out into tumor tissue and get stuck there — no targeting molecule required.

Formal definition: the **enhanced permeability and retention (EPR) effect** is the tendency of nanoparticles and macromolecules to accumulate in tumors more than in normal tissue, driven by two features of tumor vasculature: **increased permeability** (leaky vessel walls with gaps that let large molecules escape, which normal capillaries do not permit) and **poor lymphatic drainage** (impaired clearance, so what enters stays) (cba-47). First characterized by Matsumura and Maeda in 1986, EPR is the basis of **passive targeting** — accumulation that requires no targeting ligand, just the right particle size and circulation time (Matsumura & Maeda, 1986; cba-47).

EPR is the foundational idea of cancer nanomedicine. It is also genuinely contested, and this chapter treats it honestly rather than as settled dogma.

### The honest problem with EPR

Here is the calibrated truth the field has had to confront. The EPR effect was characterized largely in *rodent* tumor models, which are fast-growing, relatively uniform, and highly permeable. **Human tumors are slower-growing, more heterogeneous, and far more variable in their vascular permeability** (cba-47). The magnitude of EPR "varies substantially across tumor types and patients," and "its clinical impact has been less dramatic than initial enthusiasm predicted" (cba-47).

The sharpest quantification: a 2016 meta-analysis of published nanoparticle studies found that a **median of only ~0.7% of the injected dose reached the tumor** (Wilhelm et al., 2016) [contested — see pantry flag]. Critics — notably Nichols and Bae — have argued that the EPR effect is unreliable and often overstated in humans, and that much preclinical enthusiasm rests on models that do not represent patient tumors (Nichols & Bae, 2014) [contested — see pantry flag].

What you should take from this is *neither* "EPR is fake" *nor* "EPR delivers drugs to tumors." The honest position: EPR is real but variable and frequently weak in human tumors; it is the engine behind every approved passive-targeting nanomedicine, yet it does not reliably deliver the large fractions early enthusiasts assumed. The field is actively re-examining whether the 0.7% figure is even the right way to measure delivery and what fraction is needed for benefit. Treat any claim of dependable EPR-based tumor targeting as a hypothesis to be measured in *that* tumor, not a property you can assume.

<!-- → [DIAGRAM: EPR reliability spectrum — a horizontal bar from "mouse models (high, uniform permeability)" on the left to "human tumors (variable, often weak)" on the right; a marker at ~0.7% median injected dose to tumor (Wilhelm 2016); two annotation labels "hype: reliable targeting" and "cynicism: nanomedicine fails" struck through, with a centered "calibrated: real but variable" label] -->

### Active targeting and what it actually changes

Plain language: you can glue molecules to a particle's surface that grab onto cancer cells — but grabbing happens only after the particle has already arrived.

Formal definition: **active targeting** adds **targeting ligands** — antibodies, antibody fragments, peptides, aptamers (short nucleic acids selected to bind a target), or small molecules like folic acid — to the nanoparticle surface, so it binds a specific marker on cancer cells (cba-47). Common targets include HER2, EGFR, the transferrin receptor (high on proliferating cells), the folate receptor (enriched on some cancers), and CD44 (cba-47).

The crucial, widely misunderstood point: **active targeting changes cellular uptake, not necessarily tumor accumulation.** The ligand operates at the *last* step of the delivery chain — binding and entry into a cell — *after* the particle has survived circulation, extravasated, and penetrated the tissue. It cannot improve those earlier steps. As the source states plainly, active targeting "has not always produced the dramatic improvements over passive targeting that initial enthusiasm predicted," for several reasons (cba-47):

- The fraction of dose reaching the tumor is often limited by *clearance and circulation*, which the ligand does not change.
- **Tumor heterogeneity** means not all cells express the target.
- The **protein corona** can mask the ligands.
- Targeting may improve uptake at the tumor *without improving overall tumor accumulation* — exactly the opening case.

This is why the opening-case company saw equal total accumulation: the antibody helped cells *take up* particles once present but did nothing to get more particles *there*.

<!-- → [DIAGRAM: passive vs active targeting + protein corona schematic. Left panel: passive — bare PEGylated particle drifting out of a leaky tumor vessel (EPR), no ligand. Middle panel: active — particle with surface antibodies binding a receptor on a tumor cell, AFTER extravasation. Right panel (corona): a particle entering blood, plasma proteins (opsonins) adsorbing onto its surface and burying the targeting ligands; arrow to liver/spleen uptake.] -->

### The protein corona

Plain language: the instant a nanoparticle hits blood, proteins stick all over it, giving it a new surface the body actually "sees" — not the one you designed.

Formal definition: the **protein corona** is the layer of plasma proteins and other biomolecules that adsorbs onto a nanoparticle's surface within seconds of entering biological fluid. It has two consequences that matter enormously for targeting (cba-47):

1. **It can mask targeting ligands.** Proteins coating the surface can physically bury the antibodies or peptides you attached, so the ligand can no longer reach its receptor — defeating active targeting before the particle ever meets a tumor cell.
2. **It redirects particle fate.** Certain corona proteins (opsonins) flag the particle for clearance by the liver and spleen, shortening circulation. The corona, not your designed surface, often determines where the particle goes.

The corona is why a particle that targets perfectly in protein-free cell-culture medium can fail in blood: in the dish there is no corona, so the bare ligands work; in the body, the corona forms and the ligands are masked. The opening case is this failure exactly. The practical implication: a targeting strategy must be validated *in a biological environment that forms a corona*, not just in clean medium.

### Putting it together: what targeting can and cannot do

A clean summary you can carry:

- **Passive targeting (EPR)** gets particles *to* the tumor — when the tumor is permeable enough. It is variable and often weak in humans (contested) [contested — see pantry flag].
- **Active targeting (ligands)** improves uptake *once particles are at the tumor* — but does not get more particles there, and can be sabotaged by the corona.
- **The protein corona** stands between your designed particle and its intended behavior, masking ligands and redirecting fate.

Neither targeting strategy overrides the dose-loss chain of Chapters 1 and 2. Targeting is not a magic word; it is an intervention at a *specific step*, and you must name which step.

## Worked Example

**Situation.** A team reports that their folate-targeted nanoparticle is taken up by folate-receptor-positive tumor cells at 8× the rate of an untargeted control in cell culture. They conclude the targeting will substantially increase tumor drug delivery in patients and plan a trial. Is this conclusion warranted?

**Reasoning — the dead end first.** The 8× uptake number is impressive and real, and the intuition "more uptake means more delivery" feels airtight. The tempting conclusion: targeting multiplies tumor delivery several-fold, so the trial should show a clear advantage. This is precisely the inference the opening-case company made — and it is the dead end.

The flaw: cell-culture uptake measures only the *final* step (binding and entry) in a setting with **no circulation, no clearance, and no protein corona** (cba-47). It says nothing about whether more particles will *reach* the tumor, and it omits the corona that may mask the folate ligands in blood. Tumor accumulation is set mainly by circulation and EPR (earlier steps the ligand cannot touch), and folate-receptor expression is heterogeneous, so many tumor cells may lack the target (cba-47).

**Resolution.** Reframe the question around the delivery chain. The right prediction: the folate ligand may modestly improve *uptake* in receptor-positive cells *that the particles already reach*, but it will not increase *total tumor accumulation*, which is governed by EPR and clearance. Expect, at best, better intracellular delivery in a subset of cells — not the several-fold whole-tumor increase the team assumed. Consistent with this, the source notes that the folate-camptothecin conjugate EC145 was tested in folate-receptor-positive cancers but did not achieve approval, while folate-receptor targeting *did* succeed in a different format — the antibody-drug conjugate mirvetuximab soravtansine, approved for ovarian cancer (cba-47) — suggesting the *format* and the delivery chain, not the targeting concept alone, decide success. Before the trial, the team should measure tumor accumulation *in vivo* (with a particle label) and test ligand function in the presence of plasma to check for corona masking.

**The lesson.** Cell-culture uptake validates that a ligand *can* bind; it does not predict tumor delivery, because it skips circulation, clearance, and the corona. Active targeting changes uptake, not accumulation.

**The limit.** This reasoning holds when EPR delivers at least *some* particles to the tumor. If EPR essentially fails in the target tumor, even perfect uptake is moot — there is nothing at the tumor to take up. And in formats where the targeting moiety *also* drives circulation and accumulation (as in some antibody-drug conjugates), the clean separation between "uptake" and "accumulation" blurs.

## Common Misconceptions

**"Adding a targeting ligand increases how much drug reaches the tumor."** Plausible because the ligand binds cancer cells. It fails because the ligand acts only at cellular uptake, *after* arrival; total tumor accumulation is set by circulation and EPR, which the ligand does not change (cba-47). The opening case is this exactly: equal accumulation, different uptake.

**"If a targeted particle works in cell culture, it will work in the body."** Plausible because the binding is real. It fails because cell culture has no protein corona, so the bare ligands function; in blood, the corona can mask them (cba-47). A dish cannot test corona-dependent behavior.

**"The EPR effect reliably delivers nanoparticles to human tumors."** Plausible because EPR is the field's foundational mechanism and works well in mice. It fails — or at least is unproven — because human tumors are far more variable, EPR's clinical impact has been "less dramatic than initial enthusiasm predicted," and a median of only ~0.7% of injected dose reached tumors in published studies (Wilhelm et al., 2016; Nichols & Bae, 2014) [contested — see pantry flag]. Treat reliable EPR as a hypothesis, not a fact.

**"Nanomedicine doesn't work because only 0.7% reaches the tumor."** Plausible as a cynical overcorrection. It fails because approved nanomedicines (Doxil, Abraxane, Onivyde) demonstrably benefit patients despite low delivery fractions — the benefit can come from reduced toxicity or improved pharmacokinetics, and the fraction *needed* for benefit may be small and is itself debated (cba-47). The honest stance is calibrated: low and variable delivery, real but modest benefits — neither hype nor dismissal.

## Exercises

1. **(Understand.)** Define the EPR effect and name its two underlying vascular features. In one sentence each, state why EPR works better in mouse tumors than in human tumors.

2. **(Apply.)** A targeted nanoparticle shows 10× higher uptake than an untargeted control in cell culture but identical total tumor accumulation in mice. Explain this result using the delivery chain: which step does the ligand affect, and which steps determine total accumulation? What single in-blood experiment would test whether the protein corona is masking the ligand?

3. **(Apply+ / Analyze.)** Interpret the ~0.7% median delivery figure (Wilhelm et al., 2016) for two audiences: (a) an investor who concludes "nanomedicine is a failure," and (b) an enthusiast who insists EPR reliably targets tumors. Write a two- or three-sentence calibrated response to each that neither dismisses nor overstates the evidence, citing at least one approved nanomedicine and the contested nature of the statistic.

4. **(Create.)** Design a **passive-vs-active targeting + corona evaluation plan** for a new HER2-targeted nanoparticle. Specify: (i) one experiment to measure total tumor accumulation independent of uptake; (ii) one experiment to test whether the protein corona masks the HER2 ligand; (iii) one criterion that would tell you the active-targeting ligand is *worth keeping* versus dropping for a simpler passive (PEGylated) design. State, in advance, what result would make you abandon active targeting for this particle.

## What Would Change My Mind

The chapter's central claim is twofold: EPR-based passive targeting is real but unreliable in humans, and active targeting improves cellular uptake rather than tumor accumulation. A specific finding would force revision: a large, rigorously controlled human study showing that a targeting ligand *increases total tumor accumulation* (not just intracellular uptake) by a clinically meaningful margin across patients — i.e., that ligands overcome, rather than merely act after, the circulation-and-clearance bottleneck. Equally, robust noninvasive imaging across many patients showing that EPR delivers a consistent, substantial fraction of injected dose to most human solid tumors would overturn the "variable and often weak" characterization. The current evidence — the ~0.7% median, the variability across tumors, the corona-masking mechanism, and the repeated failure of active targeting to beat passive in accumulation (Wilhelm et al., 2016; Nichols & Bae, 2014; cba-47) — points the other way, but these are exactly the claims under active investigation.

## Still Puzzling

- Is the ~0.7% median delivery figure the right metric at all? Some argue it conflates very different particles and tumors and that *local concentration at the tumor*, not whole-body percentage, is what matters (cba-47) [contested — see pantry flag].
- Can we predict, before treatment, which patients have tumors permeable enough for EPR — a companion-imaging test that would convert nanomedicine from "build better particles" to "select responsive patients"?
- Can the protein corona be engineered as a *feature* rather than fought as a bug — designing surfaces that recruit a beneficial corona that aids targeting or circulation, rather than masking ligands?
- Why does folate-receptor targeting fail as a nanoparticle conjugate (EC145) yet succeed as an antibody-drug conjugate (mirvetuximab soravtansine) (cba-47)? What does this say about whether the carrier *format*, not the target, decides success?

## References

- Matsumura, Y., & Maeda, H. (1986). A new concept for macromolecular therapeutics in cancer chemotherapy: mechanism of tumoritropic accumulation of proteins and the antitumor agent SMANCS. *Cancer Research*, 46(12 Pt 1), 6387–6392.
- Maeda, H. (2001). The enhanced permeability and retention (EPR) effect in tumor vasculature: the key role of tumor-selective macromolecular drug targeting. *Advances in Enzyme Regulation*, 41, 189–207. [verify]
- Nichols, J. W., & Bae, Y. H. (2014). EPR: evidence and fallacy. *Journal of Controlled Release*, 190, 451–464.
- Wilhelm, S., Tavares, A. J., Dai, Q., Ohta, S., Audet, J., Dvorak, H. F., & Chan, W. C. W. (2016). Analysis of nanoparticle delivery to tumours. *Nature Reviews Materials*, 1, 16014.
- Source chapter: cba-47, "Nanotechnology in Cancer: Drug Delivery and Imaging."

## Prompts

*No figures have been generated for this chapter yet.*
