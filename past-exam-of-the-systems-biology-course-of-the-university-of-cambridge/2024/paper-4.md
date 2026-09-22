# Paper 4

↑ **Parent:** [2024](../2024.md)

[Original paper, released PDF pages 116–133](https://www.whatdotheyknow.com/request/past_examinations_papers_for_par/response/2882908/attach/3/FOI%202024%201168%20Locke%20materials.pdf?cookie_passthrough=1#page=116)

**Table of contents**

- [Section I](#section-i)
  - [1.1](#section-i/1-1)
    - [Solution](#section-i/1-1/solution)
  - [1.2](#section-i/1-2)
    - [Solution](#section-i/1-2/solution)
  - [1.3](#section-i/1-3)
    - [Solution](#section-i/1-3/solution)
  - [1.4](#section-i/1-4)
    - [Solution](#section-i/1-4/solution)
  - [1.5](#section-i/1-5)
    - [Solution](#section-i/1-5/solution)
  - [1.6](#section-i/1-6)
    - [Solution](#section-i/1-6/solution)
  - [1.7](#section-i/1-7)
    - [Solution](#section-i/1-7/solution)
  - [1.8](#section-i/1-8)
    - [Solution](#section-i/1-8/solution)
  - [1.9](#section-i/1-9)
    - [Solution](#section-i/1-9/solution)
  - [1.10](#section-i/1-10)
    - [Solution](#section-i/1-10/solution)
  - [1.11](#section-i/1-11)
    - [Solution](#section-i/1-11/solution)
  - [1.12](#section-i/1-12)
    - [Solution](#section-i/1-12/solution)
  - [1.13](#section-i/1-13)
    - [Solution](#section-i/1-13/solution)
  - [1.14](#section-i/1-14)
    - [Solution](#section-i/1-14/solution)
- [Section II](#section-ii)
  - [2.1](#section-ii/2-1)
    - [Solution](#section-ii/2-1/solution)
  - [2.2](#section-ii/2-2)
    - [Solution](#section-ii/2-2/solution)
  - [2.3](#section-ii/2-3)
    - [Solution](#section-ii/2-3/solution)

## Section I

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="section-i/1-1">1.1</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-1/solution">Solution</h4>

↑ **Parent:** [1.1](#section-i/1-1)

Write the parameters as **$\pi_0,\pi_1,\mu_0,\mu_1,\sigma_0,\sigma_1$**, where $\pi_j$ is the fraction of molecules in component $j$, $\mu_j$ is its [mean](../../expected-value.md) current, and $\sigma_j>0$ is its current [standard deviation](../../variance.md#standard-deviation). The [mixture weights](../../statistical-modelling.md#mixture-weight) satisfy $\pi_j\geq0$ and $\pi_0+\pi_1=1$. Thus six displayed parameters represent **five independent degrees of freedom**.

Assigning component 1 to modified molecules makes $\pi_1$ the inferred modification fraction. That biological assignment needs a reference or other identifying information: exchanging both component labels leaves the [Gaussian mixture distribution](../../probability-distribution.md#gaussian-mixture-distribution) unchanged. In the illustrated multi-sample model, component locations can be shared while the sample-specific fractions differ; this is different from fitting unrelated [means](../../expected-value.md) to every sample.

<h3 id="section-i/1-2">1.2</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-2/solution">Solution</h4>

↑ **Parent:** [1.2](#section-i/1-2)

The [probability density function](../../continuous-probability-distribution.md#probability-density-function) is

$$
\boxed{f(x)=\sum_{j=0}^1\frac{\pi_j}{\sigma_j\sqrt{2\pi}}\exp\!\left[-\frac{(x-\mu_j)^2}{2\sigma_j^2}\right].}
$$

Every term is nonnegative because its weight is nonnegative, its scale is positive and its exponential is positive. By [linearity of the integral](../../integral.md#linearity-of-integration) and normalization of each [normal distribution](../../probability-distribution.md#normal-distribution),

$$
\int_{-\infty}^{\infty}f(x)\,dx=\sum_{j=0}^1\pi_j\int_{-\infty}^{\infty}\phi_{\mu_j,\sigma_j}(x)\,dx=\pi_0+\pi_1=1.
$$

Thus $f$ is nonnegative and integrates to one. It is a weighted sum of densities, rather than a product or an unweighted sum whose [integral](../../integral.md) would equal two.

<a id="section-i/1-2/image-illustrative-gaussian-mixtures-with-shared-component-distributions-and-different-modification-fractions"></a>
![](../../past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-4-mixture-weights.png)

**[Figure 1](#section-i/1-2/image-illustrative-gaussian-mixtures-with-shared-component-distributions-and-different-modification-fractions). Illustrative Gaussian mixtures with shared component distributions and different modification fractions**.

<h3 id="section-i/1-3">1.3</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-3/solution">Solution</h4>

↑ **Parent:** [1.3](#section-i/1-3)

**A five-base current measurement alone does not guarantee identification of one modified base in every sequence.** At GGACT there is only one [adenosine](../../molecule.md#adenosine) in the window, so attributing an established adenosine-specific modification to that A is plausible. That does not establish a universal resolution claim.

For a counterexample, consider a window containing two candidate [adenosines](../../molecule.md#adenosine). If modifying either position produces indistinguishable current distributions, its signal cannot identify which A changed. Overlapping windows, sequence context, calibrated modification signatures or external evidence may resolve some ambiguities, but they are extra information. This is an [identifiability](../../statistical-model.md#identifiability) issue: estimating the fraction in a shifted current component is not automatically the same as identifying its molecular cause or exact position.

<h3 id="section-i/1-4">1.4</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-4/solution">Solution</h4>

↑ **Parent:** [1.4](#section-i/1-4)

**Add direct sample labels and distinguish line styles or marker shapes, rather than encoding sample identity solely by colour.** The sample identities would then remain visible in greyscale and for readers with colour-vision deficiencies. Larger axis text and a high-contrast palette would also improve readability. An accessible text description should state the comparison and principal result, rather than merely saying that the figure contains coloured curves.

<h3 id="section-i/1-5">1.5</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-5/solution">Solution</h4>

↑ **Parent:** [1.5](#section-i/1-5)

Define the evaluation universe first, including which sufficiently covered loci were eligible for both methods. Relative to the reference assay's labels,

$$
\boxed{\operatorname{TPR}=\frac{TP}{TP+FN},\qquad\operatorname{FPR}=\frac{FP}{FP+TN}.}
$$

The [true positive rate](../../statistical-learning.md#recall-classification) is the fraction of reference-positive loci retained by [xPore](../../molecular-genetics.md#xpore); the [false positive rate](../../statistical-learning.md#false-positive-rate) is the fraction of reference-negative loci incorrectly retained. The latter is not the fraction of [xPore](../../molecular-genetics.md#xpore) calls that fail validation.

An imperfect reference assay can miss real modifications. “False positive” here therefore [means](../../expected-value.md) disagreement with that reference, not independently demonstrated absence of a modification. Restricting the universe differently for the two denominators would invalidate the comparison.

<h3 id="section-i/1-6">1.6</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-6/solution">Solution</h4>

↑ **Parent:** [1.6](#section-i/1-6)

Choose a cutoff on the ranked score and call every eligible locus above it positive. Compare those calls with the fixed reference labels, count $TP,FP,TN,FN$, and plot $(FP/(FP+TN),TP/(TP+FN))$. Repeating over cutoffs generates the [receiver operating characteristic](../../statistical-learning.md#receiver-operating-characteristic).

A very restrictive cutoff starts near $(0,0)$; a cutoff calling everything positive ends at $(1,1)$. The reference labels and eligible locus set must stay fixed during this sweep. Tied scores need a consistent treatment. A single cutoff gives one operating point, whereas the curve describes the trade-off across many possible cutoffs.

<h3 id="section-i/1-7">1.7</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-7/solution">Solution</h4>

↑ **Parent:** [1.7](#section-i/1-7)

A good [receiver operating characteristic](../../statistical-learning.md#receiver-operating-characteristic) rises toward the upper-left corner: many reference-positive loci are detected while few reference-negative loci are accepted. The [area under the ROC curve](../../statistical-learning.md#area-under-the-roc-curve) summarizes this discrimination over cutoffs. **Higher is better in the stated score direction; perfect separation gives one.** The displayed value near 0.86 indicates substantial ranking discrimination against this reference.

The area can also be interpreted as the [probability](../../probability-theory.md#probability) that a randomly chosen positive receives a higher score than a randomly chosen negative, with half credit for ties. It does not select a cutoff or demonstrate that most retained calls are correct: those practical questions also depend on prevalence and the relative costs of errors.

<a id="section-i/1-7/image-the-same-illustrative-classifier-viewed-through-roc-and-precision-recall-curves-at-ten-percent-prevalence"></a>
![](../../past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-4-roc-and-precision.png)

**[Figure 2](#section-i/1-7/image-the-same-illustrative-classifier-viewed-through-roc-and-precision-recall-curves-at-ten-percent-prevalence). The same illustrative classifier viewed through ROC and precision–recall curves at ten percent prevalence**.

<h3 id="section-i/1-8">1.8</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-8/solution">Solution</h4>

↑ **Parent:** [1.8](#section-i/1-8)

**The diagonal [means](../../expected-value.md) no ranking discrimination against the reference labels, with ROC area 0.5.** At every operating point on that diagonal, the fraction of positives accepted equals the fraction of negatives accepted. A score independent of the true label has this expected behaviour.

This does not imply that exactly half of all individual predictions are correct: an imbalanced dataset can have high accuracy by always predicting the majority class. It also does not establish biological absence of signal; it describes what the evaluated score extracts relative to the chosen reference and dataset.

<h3 id="section-i/1-9">1.9</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-9/solution">Solution</h4>

↑ **Parent:** [1.9](#section-i/1-9)

The two quantities are

$$
\boxed{\mathrm{precision}=\frac{TP}{TP+FP},\qquad\mathrm{recall}=\frac{TP}{TP+FN}.}
$$

[Classification precision](../../statistical-learning.md#precision-classification) asks how many retained calls agree with the positive reference; [classification recall](../../statistical-learning.md#recall-classification) asks how much of the positive reference set has been recovered. Recall is the [true positive rate](../../statistical-learning.md#recall-classification). Increasing recall by accepting more loci can reduce precision through additional false positives.

If positive prevalence is $p$, then

$$
\mathrm{precision}=\frac{p\,\operatorname{TPR}}{p\,\operatorname{TPR}+(1-p)\operatorname{FPR}}.
$$

Thus prevalence matters: good ROC discrimination need not give high precision when true positives are rare. A precision–recall area must be judged against its own prevalence-dependent baseline; it is not numerically interchangeable with ROC area.

<h3 id="section-i/1-10">1.10</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-10/solution">Solution</h4>

↑ **Parent:** [1.10](#section-i/1-10)

**It is a useful depletion control, but not an automatically modification-free negative control.** A nominal knockout may retain functional products, and loss of one writer does not establish absence of every relevant [RNA](../../polymer.md#ribonucleic-acid) modification. Calling the sample completely negative requires independent validation of the molecular state being used as ground truth.

This distinction has direct experimental support: alternatively spliced functional [METTL3](../../enzyme.md#mettl3) products have been found in some nominal knockout lines.[Abstract and Results: residual functional METTL3 isoforms in purported knockout cells](../../biology-bibliography.md#alternative-splicing-of-mettl3-explains-apparently-mettl3-independent-m6a-modifications-in-mrna-by-hui-xian-poh-and-others) That result identifies a possible failure mode; it does not prove that this particular sample has the same defect. A modification-free reference preparation and an independent chemical measurement would strengthen the interpretation.

<h3 id="section-i/1-11">1.11</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-11/solution">Solution</h4>

↑ **Parent:** [1.11](#section-i/1-11)

Pooling can erase [between-replicate variation](../../design-of-experiments.md#between-replicate-variation). One unusually well-covered or highly modified sample can dominate the pooled estimate, hiding an inconsistent biological response. If individual reads are then treated as independent [biological replicates](../../design-of-experiments.md#biological-replicate), uncertainty can be understated through [pseudoreplication](../../statistical-modelling.md#pseudoreplication).

A better analysis retains replicate identity and models sample-to-sample variation, while allowing information to be shared about suitable common component parameters. Pooled performance on a larger dataset can be useful, but should not substitute for evidence that the result reproduces across independent biological samples.

<h3 id="section-i/1-12">1.12</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-12/solution">Solution</h4>

↑ **Parent:** [1.12](#section-i/1-12)

Use small multiples with consistent axes, direct cutoff labels and distinguishable line styles, with an inset enlarging the low-false-positive-rate region of the ROC curves. Add a compact summary of area versus minimum read count with uncertainty intervals and the number of eligible loci retained at each cutoff. This would make the modest ROC-area change and larger precision–recall-area change easier to assess than several nearly overlapping colours.

A coverage restriction also changes which loci are evaluated. For a clean comparison, show performance on a common locus subset as well as the practical retained set; otherwise an apparent improvement may partly reflect exclusion of difficult loci or a changed positive prevalence.

<h3 id="section-i/1-13">1.13</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-13/solution">Solution</h4>

↑ **Parent:** [1.13](#section-i/1-13)

**The panel supports feasibility in these samples, but not the full strength or generality of the claim.** The method produces modification estimates for three patient samples, and the displayed selected [genes](../../genetics.md#gene) generally have higher estimates than the knockout controls. That is evidence that an analysis can be performed and yields biological-looking contrasts.

The comparison simultaneously changes cell background, disease status and potentially sequencing conditions. The displayed [genes](../../genetics.md#gene) were selected for high estimated modification, creating [selection bias](../../causal-inference.md#selection-bias); the same estimates do not independently validate their accuracy. The panel also does not itself show input-RNA amounts, uncertainty, or performance across controlled input levels. It therefore cannot alone establish reliable low-input performance across genetically diverse clinical samples or disease-specific modification differences.

<h3 id="section-i/1-14">1.14</h3>

↑ **Parent:** [Section I](#section-i)

<h4 id="section-i/1-14/solution">Solution</h4>

↑ **Parent:** [1.14](#section-i/1-14)

Two useful changes would be:

- Show patient estimates together with matched, relevant cell-type controls and an independent measurement of modification at prespecified or held-out loci. Display uncertainty and all evaluated loci, or state a selection rule independent of the reported contrast. This separates genuine agreement from selection of high [xPore](../../molecular-genetics.md#xpore) values and from unrelated cell-background effects.
- Add performance across measured RNA-input levels for the same biological materials, with biological and technical replication, [read coverage](../../molecular-genetics.md#read-coverage) and failure rates reported. This tests the low-input part of the claim directly rather than inferring it from the heatmap.

A single additional knockout row would not address both independent accuracy and input dependence.

## Section II

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="section-ii/2-1">2.1</h3>

↑ **Parent:** [Section II](#section-ii)

<h4 id="section-ii/2-1/solution">Solution</h4>

↑ **Parent:** [2.1](#section-ii/2-1)

**Central hypothesis and objectives.** PUF50 participates in one or more [protein](../../protein.md) assemblies whose composition or activity affects [Wnt signalling](../../signal-transduction.md#wnt-signalling). The proposal should distinguish membership, direct binding and causal pathway regulation. The three aims are to nominate plausible partners, identify reproducible cellular complexes, and test whether a supported interaction explains the phenotype.

**Computational starting point.** Inspect the verified PUF50 sequence for [protein domains](../../protein.md#protein-domain), localization signals, conserved residues and predicted disordered regions. Use [sequence alignment](../../molecular-genetics.md#sequence-alignment) and [orthology](../../molecular-genetics.md#orthology) to compare well-annotated homologues, recording uncertainty in functional transfer. Public interaction and expression resources can nominate partners expressed in the experimental cell line. Structural predictions can prioritize testable interfaces, but a confident fold alone does not establish a cellular interaction or tumour-suppressor function.

**Discovery [proteomics](../../biochemistry.md#proteomics).** Use [affinity purification-mass spectrometry](../../biology.md#affinity-purification-mass-spectrometry) to compare PUF50-associated material with matched negative controls across independent [biological replicates](../../design-of-experiments.md#biological-replicate). An endogenous or functionally validated tagged preparation is preferable to assuming that strong overexpression preserves normal localization and complex [stoichiometry](../../chemical-reaction.md#stoichiometry). Tag-only controls, input abundance measurements and an unrelated bait help distinguish reproducible association from abundant or sticky contaminants. Quantitative enrichment should be evaluated together with replicate consistency and a controlled [false discovery rate](../../statistical-hypothesis-test.md#false-discovery-rate).

Complexes may vary with pathway state. Compare a relevant baseline and a defined Wnt-responsive state, checking that changes in recovered partner abundance are not explained solely by input abundance, cell number or viability. If transient or compartmentalized partners are missed, [proximity labeling](../../biology.md#proximity-labeling) can provide complementary neighbourhood evidence. Its hits should be labelled as proximity associations rather than automatically promoted to direct complex subunits.

**Independent validation and mechanism.** Validate leading associations by reciprocal [co-immunoprecipitation](../../biology.md#co-immunoprecipitation) and localization evidence. Where a direct interaction is important to the proposed mechanism, test it with an independent assay suited to the relevant [protein domains](../../protein.md#protein-domain). A genetic perturbation and rescue comparison can ask whether loss of PUF50 changes pathway output and whether restoring PUF50 restores it. Compare pathway-proximal measurements with downstream transcription and longer-term growth phenotypes, because a growth defect alone is not specific to Wnt regulation.

A separation-of-function comparison is especially informative: a PUF50 variant that retains abundance and localization but loses a supported partner association could help connect the interaction to function. This interpretation requires checking folding and stability, since an inactive misfolded [protein](../../protein.md) does not isolate one interface's role. Genetic interaction analysis can then place PUF50 relative to known pathway components without treating every correlated expression change as a direct target.

**Analysis, deliverables and alternatives.** Integrate quantitative interaction evidence, localization and perturbation responses into an annotated [protein interaction network](../../protein.md#protein-interaction-network), retaining evidence type on each edge. Report [effect sizes](../../statistical-inference.md#effect-size) and uncertainty, include unsuccessful validation, and release analysis code with processed data. A negative stable-complex result would motivate a transient or condition-specific interaction hypothesis rather than proving that PUF50 acts alone. The principal deliverable is a ranked, experimentally qualified set of complexes and a causal test of the most supported pathway mechanism.

<h3 id="section-ii/2-2">2.2</h3>

↑ **Parent:** [Section II](#section-ii)

<h4 id="section-ii/2-2/solution">Solution</h4>

↑ **Parent:** [2.2](#section-ii/2-2)

**Objective and rationale.** Build an evidence-traceable [genome](../../molecular-genetics.md#genome) resource for the organism described in the question, then improve its [gene](../../genetics.md#gene) structures using one genome-wide experiment: replicated, strand-aware [RNA sequencing](../../molecular-genetics.md#rna-sequencing) across a deliberately chosen range of growth conditions. The species name is treated as part of the hypothetical study; no established [gene](../../genetics.md#gene) catalogue is assumed.

Poor annotation limits both discovery and interpretation. Missing exons distort [protein sequences](../../protein.md#protein-sequence), merged or split [gene models](../../genetics.md#gene-model) create false absences and duplications, and unrecognized transcripts bias expression analyses. Functional claims transferred to an incorrectly predicted [protein](../../protein.md) can then compound the original error. Reliable coordinates, [gene](../../genetics.md#gene) identifiers and evidence provenance are therefore prerequisites for a comparative model system.

**Resource construction.** Assemble a versioned reference containing the [genome assembly](../../genetics.md#genome-assembly), existing [gene models](../../genetics.md#gene-model), published sequence evidence and curated cross-references. Reconcile naming and coordinates, flag conflicting [gene](../../genetics.md#gene) structures, and document assembly gaps and repetitive regions. Compare predicted [proteins](../../protein.md) with well-annotated yeast homologues using [orthology](../../molecular-genetics.md#orthology), conserved domain architecture and, where informative, conserved [gene](../../genetics.md#gene) neighbourhoods. Sequence similarity is evidence for a relationship; it is not sufficient to give every paralogue its best hit's exact function.

**Genome-wide experiment.** Use [RNA sequencing](../../molecular-genetics.md#rna-sequencing) to supply transcript evidence from independent biological samples covering contrasting physiological states. Multiple conditions broaden the chance of observing condition-specific [genes](../../genetics.md#gene), but read counts within a library remain technical observations, not extra [biological replicates](../../design-of-experiments.md#biological-replicate). Quality-control and strand-aware alignment would assess mapping uniqueness, exon coverage and [splice junction](../../biology.md#splice-junction) support. Reference-guided and appropriately checked [transcript assembly](../../molecular-genetics.md#transcript-assembly) can identify expressed loci absent from the current annotation and suggest corrected exon boundaries, alternative transcripts and untranslated regions.

Integrate these data with [protein](../../protein.md) homology and gene-prediction evidence. A proposed exon should have coherent splice support and coding plausibility; an isolated ambiguous read is insufficient. Keep alternative models and confidence levels when repeat structure or incomplete coverage prevents a unique assignment. No expression in the sampled conditions should be recorded as lack of evidence, not proof that a [gene](../../genetics.md#gene) is absent.

**Validation and functional annotation.** Validate a representative set of corrected and new models by targeted transcript and junction checks, prioritizing models whose revision changes a predicted [protein domain](../../protein.md#protein-domain) or conserved function. Retain known positive controls and distinguish biological alternatives from assembly or mapping errors. Transfer broad functional terms conservatively using [orthology](../../molecular-genetics.md#orthology) and domain evidence, with explicit evidence codes and source organisms; a computationally inferred function remains distinct from an experimental demonstration.

[RNA sequencing](../../molecular-genetics.md#rna-sequencing) improves expressed [gene](../../genetics.md#gene) structures and condition-specific expression annotation, but it does not repair every assembly gap, establish translation of every transcript, or identify every [gene](../../genetics.md#gene)'s biochemical activity. Those limitations should remain visible in the resource. The deliverables are a searchable [genome browser](../../biology.md#genome-browser), stable identifiers, versioned [gene models](../../genetics.md#gene-model) and downloadable evidence tracks, together with a reproducible update process that preserves previous releases and community corrections.

<h3 id="section-ii/2-3">2.3</h3>

↑ **Parent:** [Section II](#section-ii)

<h4 id="section-ii/2-3/solution">Solution</h4>

↑ **Parent:** [2.3](#section-ii/2-3)

**Model and central question.** Use [Saccharomyces cerevisiae](../../organism.md#saccharomyces-cerevisiae) as a tractable eukaryotic system with a well-annotated [genome](../../molecular-genetics.md#genome) and established [DNA repair](../../molecular-genetics.md#dna-repair) and checkpoint biology. The aim is to identify the UV-responsive transcriptional programme and separate direct regulation from secondary changes caused by cell-cycle arrest, altered growth or loss of viability. The resulting network is a yeast model; conservation in other eukaryotes remains a hypothesis to test.

**Discovery design.** Compare UV-exposed and mock-handled cultures at baseline and several recovery stages, using independent [biological replicates](../../design-of-experiments.md#biological-replicate) and balanced processing. Include matched handling controls and record growth, viability and [cell cycle](../../cell-cycle.md) state. Choose conditions yielding an interpretable damage response rather than treating terminally damaged cells as a normal regulatory trajectory. Biological replication and [randomization](../../causal-inference.md#randomization) must occur at the culture level, not merely by sequencing the same material repeatedly.

Measure transcript abundance using [RNA sequencing](../../molecular-genetics.md#rna-sequencing) and assess sample quality before testing differences. Model condition, time, their interaction and recorded batch factors, using an appropriate count-based expression model. Report [effect sizes](../../statistical-inference.md#effect-size), uncertainty and [false discovery rate](../../statistical-hypothesis-test.md#false-discovery-rate), not only a list passing a significance cutoff. Where changes in total [RNA](../../polymer.md#ribonucleic-acid) per cell could invalidate relative normalization, include a suitable external reference strategy and distinguish relative composition from absolute expression.

**Candidate regulators and direct targets.** Cluster well-supported expression trajectories to nominate coordinated modules, then ask whether their promoters are enriched for known transcription-factor motifs. Combine motif evidence with regulator expression, localization or activity measurements and prior knowledge. Motif occurrence and coexpression alone are insufficient to establish a direct regulatory edge: a factor can be activated without changing its own transcript abundance, and many coexpressed [genes](../../genetics.md#gene) share an upstream cause.

For prioritized factors, compare chromatin association before and after damage using [chromatin immunoprecipitation](../../biology.md#chromatin-immunoprecipitation) with genome-wide readout and appropriate input and specificity controls. Binding near a [gene](../../genetics.md#gene) is additional evidence, not proof that the binding event regulates it. A targeted regulator perturbation and rescue comparison should test the predicted expression response while monitoring viability and checkpoint effects. Reporter or promoter-element comparisons can further test a specific cis-regulatory mechanism without assuming that every enriched motif is functional.

**Temporal and causal integration.** Use timing, perturbation effects and occupancy jointly. A plausible direct target changes after regulator activation, shows relevant occupancy evidence and responds to a selective perturbation. Secondary effects may appear later or depend on cell-cycle redistribution. Where transcript abundance cannot separate synthesis from [RNA](../../polymer.md#ribonucleic-acid) stability, a focused measurement of newly synthesized [RNA](../../polymer.md#ribonucleic-acid) can test the proposed transcriptional component.

Build a [gene regulatory network](../../mathematical-biology.md#gene-regulatory-network) whose edges retain sign, condition, confidence and evidence type. Predict responses to a held-out perturbation or recovery condition, and assess those predictions using new biological samples. Release the design, metadata, code and qualified edge list. Success is a validated account of important regulatory modules and their limits, rather than an unsupported claim to have measured every possible interaction in the eukaryotic damage response.

## ↑ Ancestors (10)

1. [2024](../2024.md)
2. [Past exam of the systems biology course of the University of Cambridge](../../past-exam-of-the-systems-biology-course-of-the-university-of-cambridge.md)
3. [Systems Biology course of the University of Cambridge](../../university-of-cambridge.md#systems-biology-course-of-the-university-of-cambridge)
4. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
