# Causal inference

↑ **Parent:** [Probability and statistics](probability-and-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Causal_inference)

Causal inference studies effects of interventions by comparing [potential outcomes](#potential-outcome) under different treatments.

**Table of contents**

- [Outcome standardization](#outcome-standardization)
- [Causal mediation analysis](#causal-mediation-analysis)
  - [Total causal effect](#total-causal-effect)
    - [Natural direct effect](#natural-direct-effect)
    - [Natural indirect effect](#natural-indirect-effect)
  - [Mediator-outcome confounding](#mediator-outcome-confounding)
- [Confounding by indication](#confounding-by-indication)
- [Causal identification](#causal-identification)
- [G-computation](#g-computation)
  - [Sequential exchangeability](#sequential-exchangeability)
- [Exposure](#exposure)
- [Treatment](#treatment)
- [Statistical association](#statistical-association)
  - [Observational study](#observational-study)
    - [Case–control study](#case-control-study)
    - [Longitudinal study](#longitudinal-study)
    - [Cross-sectional study](#cross-sectional-study)
    - [Reverse causality](#reverse-causality)
- [Instrumental variable](#instrumental-variable)
  - [Wald estimator](#wald-estimator)
  - [Instrument relevance](#instrument-relevance)
    - [Weak instrument](#weak-instrument)
  - [Instrumental-variable independence](#instrumental-variable-independence)
  - [Exclusion restriction](#exclusion-restriction)
  - [Mendelian randomization](#mendelian-randomization)
    - [Within-family Mendelian randomization](#within-family-mendelian-randomization)
    - [MR-Egger regression](#mr-egger-regression)
      - [InSIDE assumption](#inside-assumption)
    - [Weighted-median Mendelian randomization estimator](#weighted-median-mendelian-randomization-estimator)
    - [Two-sample Mendelian randomization](#two-sample-mendelian-randomization)
    - [Horizontal pleiotropy](#horizontal-pleiotropy)
    - [Residual exposure stratification](#residual-exposure-stratification)
  - [Confounder-instrument interaction](#confounder-instrument-interaction)
  - [Instrumental-variable monotonicity](#instrumental-variable-monotonicity)
    - [Local average treatment effect](#local-average-treatment-effect)
- [Interference in causal inference](#interference-in-causal-inference)
- [Ecological fallacy](#ecological-fallacy)
  - [Aggregate composition does not identify offender composition](#aggregate-composition-does-not-identify-offender-composition)
- [Causal directed acyclic graph](#causal-directed-acyclic-graph)
  - [Causal minimality](#causal-minimality)
    - [Causally minimal nonfaithful Gaussian model](#causally-minimal-nonfaithful-gaussian-model)
  - [PC algorithm](#pc-algorithm)
    - [Population PC correctness under faithfulness](#population-pc-correctness-under-faithfulness)
    - [PC initialization from a conditional independence graph](#pc-initialization-from-a-conditional-independence-graph)
  - [Directed acyclic graph factorization](#directed-acyclic-graph-factorization)
    - [Global Markov property for a directed acyclic graph](#global-markov-property-for-a-directed-acyclic-graph)
  - [Faithfulness of a directed acyclic graph](#faithfulness-of-a-directed-acyclic-graph)
  - [Nonparametric structural equation model](#nonparametric-structural-equation-model)
  - [Acyclic directed mixed graph](#acyclic-directed-mixed-graph)
    - [Verma constraint](#verma-constraint)
    - [District of an acyclic directed mixed graph](#district-of-an-acyclic-directed-mixed-graph)
      - [Fixable vertex](#fixable-vertex)
    - [M-separation](#m-separation)
  - [Front-door adjustment](#front-door-adjustment)
    - [Conditional front-door adjustment](#conditional-front-door-adjustment)
  - [Backdoor (causal analysis)](#backdoor-causal-analysis)
    - [Backdoor path](#backdoor-path)
      - [Backdoor adjustment set](#backdoor-adjustment-set)
        - [Sufficient adjustment set](#sufficient-adjustment-set)
          - [Minimal sufficient adjustment set](#minimal-sufficient-adjustment-set)
  - [Linear structural equation model](#linear-structural-equation-model)
    - [Wright path tracing rule](#wright-path-tracing-rule)
- [Potential outcomes framework](#potential-outcomes-framework)
  - [Principal stratification](#principal-stratification)
    - [Principal stratum](#principal-stratum)
  - [Potential outcome](#potential-outcome)
    - [Causal effect](#causal-effect)
      - [Homogeneous treatment effect](#homogeneous-treatment-effect)
      - [Causal null hypothesis](#causal-null-hypothesis)
        - [Structural zero](#structural-zero)
      - [Average treatment effect](#average-treatment-effect)
        - [Conditional average treatment effect](#conditional-average-treatment-effect)
          - [Overlap-weighted average treatment effect](#overlap-weighted-average-treatment-effect)
        - [Heterogeneous treatment effect](#heterogeneous-treatment-effect)
        - [Average treatment effect on the treated](#average-treatment-effect-on-the-treated)
      - [Causal risk ratio](#causal-risk-ratio)
- [Confounding](#confounding)
  - [Case mix](#case-mix)
    - [Risk-adjusted provider comparison](#risk-adjusted-provider-comparison)
  - [Simpson's paradox](#simpson-s-paradox)
  - [Confounder](#confounder)
- [Ignorability](#ignorability)
  - [Conditional exchangeability](#conditional-exchangeability)
- [Positivity assumption](#positivity-assumption)
- [Inverse probability weighting](#inverse-probability-weighting)
  - [Propensity score](#propensity-score)
  - [Inverse-probability-weighted estimator of the average treatment effect](#inverse-probability-weighted-estimator-of-the-average-treatment-effect)
  - [Overlap weight](#overlap-weight)
- [Consistency in causal inference](#consistency-in-causal-inference)
- [Effect modifier](#effect-modifier)
- [Selection bias](#selection-bias)
  - [Survivorship bias](#survivorship-bias)
  - [Collider bias](#collider-bias)
- [Internal validity](#internal-validity)
- [External validity](#external-validity)
- [Regression discontinuity design](#regression-discontinuity-design)
- [Difference-in-differences](#difference-in-differences)
- [Matching (statistics)](#matching-statistics)
  - [Covariate balance](#covariate-balance)
    - [Standardized mean difference](#standardized-mean-difference)
  - [Caliper matching](#caliper-matching)
- [Negative control outcome](#negative-control-outcome)
  - [Negative control group](#negative-control-group)
- [Sensitivity analysis for unmeasured confounding](#sensitivity-analysis-for-unmeasured-confounding)
  - [Bivariate probit model for endogenous treatment](#bivariate-probit-model-for-endogenous-treatment)
- [Randomized controlled trial](#randomized-controlled-trial)
  - [Care-seeking effects on a recorded injury outcome](#care-seeking-effects-on-a-recorded-injury-outcome)
  - [Risk compensation in a prevention trial](#risk-compensation-in-a-prevention-trial)
  - [Cluster-randomized trial](#cluster-randomized-trial)
  - [Selective outcome reporting](#selective-outcome-reporting)
  - [Number needed to treat](#number-needed-to-treat)
  - [Blinded outcome assessment](#blinded-outcome-assessment)
  - [Intention-to-treat analysis](#intention-to-treat-analysis)
    - [Treatment contamination](#treatment-contamination)
      - [Symmetric treatment crossover attenuates a risk difference](#symmetric-treatment-crossover-attenuates-a-risk-difference)
    - [Post-randomization adjustment changes a treatment estimand](#post-randomization-adjustment-changes-a-treatment-estimand)
  - [Randomization](#randomization)
    - [Randomized minimization in clinical trials](#randomized-minimization-in-clinical-trials)
    - [Stratified randomization](#stratified-randomization)
      - [Permuted-block randomization](#permuted-block-randomization)
    - [Allocation concealment](#allocation-concealment)
    - [Restricted randomization](#restricted-randomization)
    - [Complete randomization](#complete-randomization)

## Outcome standardization

↑ **Parent:** [Causal inference](causal-inference.md)

Outcome standardization averages fitted conditional outcome risks over a specified target population's pretreatment covariate distribution. The same target distribution is used for each treatment strategy. Under [conditional exchangeability](#conditional-exchangeability), the [positivity assumption](#positivity-assumption) and consistency, this average identifies the target mean of the corresponding [potential outcomes](#potential-outcome). For a target consisting of treated subjects, average over their covariate distribution. A conditional [odds ratio](statistical-modelling.md#odds-ratio) cannot generally be applied directly to an aggregate mean risk: the nonlinear odds-to-probability conversion must be performed before averaging. [Outcome standardization](#outcome-standardization) supplies that individual-risk calculation.

## Causal mediation analysis

↑ **Parent:** [Causal inference](causal-inference.md)

Causal mediation analysis decomposes a [total causal effect](#total-causal-effect) into effects transmitted through a designated mediator and effects operating through other pathways. Identification generally requires assumptions about exposure-outcome, exposure-mediator, and mediator-outcome confounding.

### Total causal effect

↑ **Parent:** [Causal mediation analysis](#causal-mediation-analysis)

For binary exposure $A$, the total causal effect on an additive scale is $\mathbb E[Y(1)-Y(0)]$. With mediator potential outcome $M(a)$ and nested outcome $Y(a,m)$, consistency gives $Y(a)=Y(a,M(a))$.

#### Natural direct effect

↑ **Parent:** [Total causal effect](#total-causal-effect)

One natural direct effect is

$$
\mathbb E[Y(1,M(0))-Y(0,M(0))],
$$

which changes exposure while holding the mediator at its natural value under no exposure.

#### Natural indirect effect

↑ **Parent:** [Total causal effect](#total-causal-effect)

One natural indirect effect is

$$
\mathbb E[Y(1,M(1))-Y(1,M(0))],
$$

which changes the mediator between its two natural values while holding exposure fixed.

### Mediator-outcome confounding

↑ **Parent:** [Causal mediation analysis](#causal-mediation-analysis)

Mediator-outcome confounding occurs when a common cause of the mediator and outcome is not adequately controlled. If exposure itself affects such a common cause, ordinary adjustment can fail to identify natural direct and indirect effects.

## Confounding by indication

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Confounding_by_indication)

Confounding by indication occurs when treatment choice depends on disease severity or prognosis. The treated group can then have worse outcomes because it was at higher baseline risk, even if treatment is beneficial.

## Causal identification

↑ **Parent:** [Causal inference](causal-inference.md)

A causal estimand is identified when every causal model satisfying the stated assumptions and inducing the same observed-data distribution gives it the same value. An identifying formula expresses that value entirely through the observed-data distribution.

## G-computation

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/G-computation)

The g-formula identifies an interventional outcome distribution by averaging observed conditional outcome laws over the covariate distribution under suitable consistency, exchangeability, and positivity assumptions.

### Sequential exchangeability

↑ **Parent:** [G-computation](#g-computation)

For treatment history $\bar A_t$, observed history $H_t$, and final [potential outcome](#potential-outcome) $Y(\bar a)$, sequential exchangeability requires

$$
Y(\bar a)\mathrel\perp A_t\mid H_t
$$

at every treatment time. Together with [consistency of potential outcomes](#consistency-in-causal-inference) and [positivity in causal inference](#positivity-assumption), it identifies longitudinal effects by [G-computation](#g-computation).

## Exposure

↑ **Parent:** [Causal inference](causal-inference.md)

An exposure is a condition, behavior, intervention, or environmental factor whose association or causal effect on an outcome is studied.

## Treatment

↑ **Parent:** [Causal inference](causal-inference.md)

A treatment is an intervention assigned or received by a study unit. In causal inference it indexes the unit's [potential outcomes](#potential-outcome).

## Statistical association

↑ **Parent:** [Causal inference](causal-inference.md)

A statistical association is a systematic dependence between variables. It need not represent a [causal effect](#causal-effect), because it may arise from [confounding](#confounding), selection, or reverse causation.

### Observational study

↑ **Parent:** [Statistical association](#statistical-association)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Observational_study)

An observational study measures exposures and outcomes without assigning the exposure by an intervention. Its causal interpretation therefore requires assumptions that address [confounding](#confounding) and [selection bias](#selection-bias).

<h4 id="case-control-study">Case–control study</h4>

↑ **Parent:** [Observational study](#observational-study)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Case–control_study)

A case–control study selects subjects according to an outcome: cases have the outcome and controls represent an appropriate comparison population. It compares their prior exposures or genetic variants to study association. Its retrospective sampling must be accounted for when interpreting risks; [selection bias](#selection-bias) and [confounding](#confounding) can distort an unadjusted association. In genetics, matched [family pseudo-control genotypes](biology.md#family-pseudo-control-genotype) can replace unrelated controls for a conditional [transmission disequilibrium test](biology.md#transmission-disequilibrium-test).

#### Longitudinal study

↑ **Parent:** [Observational study](#observational-study)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Longitudinal_study)

A [longitudinal study](#longitudinal-study) observes the same individuals repeatedly. Within-person changes distinguish temporal development from persistent differences between people, although calendar-period changes, selective dropout and [measurement error](probability-and-statistics.md#measurement-error) still require attention. A [random-intercept linear mixed model](statistical-modelling.md#random-intercept-linear-mixed-model) can represent persistent individual differences and correlated repeated measurements.

#### Cross-sectional study

↑ **Parent:** [Observational study](#observational-study)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cross-sectional_study)

A [cross-sectional study](#cross-sectional-study) measures different individuals during one observation period. Differences between ages can reflect [confounding](#confounding) or birth-cohort differences as well as changes within individuals; a [longitudinal study](#longitudinal-study) is needed to measure the latter directly.

#### Reverse causality

↑ **Parent:** [Observational study](#observational-study)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reverse_causality)

Reverse causality occurs when an apparent exposure-outcome association is partly or wholly generated by the outcome, or by an early stage of it, affecting the measured exposure.

## Instrumental variable

↑ **Parent:** [Causal inference](causal-inference.md)

An instrumental variable changes an [exposure](#exposure) or [treatment](#treatment) but affects the outcome only through that exposure. Together, [instrument relevance](#instrument-relevance), [instrumental-variable independence](#instrumental-variable-independence), and the [exclusion restriction](#exclusion-restriction) identify causal effects under suitable structural assumptions.

### Wald estimator

↑ **Parent:** [Instrumental variable](#instrumental-variable)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wald_estimator)

For a binary [instrumental variable](#instrumental-variable) $Z$, exposure $X$, and outcome $Y$, the Wald estimator is the ratio of the instrument's effect on the outcome to its effect on the exposure:

$$
\widehat\beta_{\rm Wald}
=\frac{\overline Y_{Z=1}-\overline Y_{Z=0}}
{\overline X_{Z=1}-\overline X_{Z=0}}.
$$

Under instrumental-variable assumptions it estimates a causal effect.

### Instrument relevance

↑ **Parent:** [Instrumental variable](#instrumental-variable)

Instrument relevance requires the [instrumental variable](#instrumental-variable) to change the conditional distribution of the exposure. A nearly irrelevant instrument is a [weak instrument](#weak-instrument) and can produce unstable estimates.

#### Weak instrument

↑ **Parent:** [Instrument relevance](#instrument-relevance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weak_instrument)

A weak instrument has only a small association with the endogenous exposure, making instrumental-variable estimators imprecise and potentially badly biased in finite samples.

### Instrumental-variable independence

↑ **Parent:** [Instrumental variable](#instrumental-variable)

Instrumental-variable independence requires the instrument to be independent of unmeasured causes of the outcome, usually conditionally on specified observed covariates.

### Exclusion restriction

↑ **Parent:** [Instrumental variable](#instrumental-variable)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exclusion_restriction)

The exclusion restriction requires an [instrumental variable](#instrumental-variable) to affect the outcome only through the exposure whose causal effect is being studied.

### Mendelian randomization

↑ **Parent:** [Instrumental variable](#instrumental-variable)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mendelian_randomization)

Mendelian randomization uses inherited [genetic variants](biology.md#genetic-variant) associated with an [exposure](#exposure) as [instrumental variables](#instrumental-variable). Its causal interpretation requires [instrument relevance](#instrument-relevance), [instrumental-variable independence](#instrumental-variable-independence), and the [exclusion restriction](#exclusion-restriction).

#### Within-family Mendelian randomization

↑ **Parent:** [Mendelian randomization](#mendelian-randomization)

Within-family [Mendelian randomization](#mendelian-randomization) uses genetic contrasts within families, such as differences between siblings. Conditioning on shared parental background can reduce [population stratification](biology.md#population-stratification) and family-level sources of [confounding](#confounding), although the [exclusion restriction](#exclusion-restriction) and sufficient [instrument relevance](#instrument-relevance) remain necessary.

#### MR-Egger regression

↑ **Parent:** [Mendelian randomization](#mendelian-randomization)

MR-Egger regression fits genetic outcome associations to genetic [exposure](#exposure) associations with a free intercept. Its slope estimates a [causal effect](#causal-effect) under the [InSIDE assumption](#inside-assumption) and appropriate instrument-strength assumptions; its intercept assesses average directional [horizontal pleiotropy](#horizontal-pleiotropy). A nonsignificant intercept, especially with few [genetic variants](biology.md#genetic-variant), does not prove the [exclusion restriction](#exclusion-restriction) for every instrument.

##### InSIDE assumption

↑ **Parent:** [MR-Egger regression](#mr-egger-regression)

InSIDE stands for instrument strength independent of direct effect. It requires the genetic associations with the [exposure](#exposure) to be independent of the direct, pleiotropic effects of those [genetic variants](biology.md#genetic-variant) on the outcome. It is a key identifying assumption for [MR-Egger regression](#mr-egger-regression).

#### Weighted-median Mendelian randomization estimator

↑ **Parent:** [Mendelian randomization](#mendelian-randomization)

This weighted median of genetic variant ratio estimates consistently estimates a common [causal effect](#causal-effect) when more than half of its asymptotic weight comes from valid [instrumental variables](#instrumental-variable), subject to the usual sampling regularity conditions. It is a [sensitivity analysis](probability-and-statistics.md#sensitivity-analysis) for [horizontal pleiotropy](#horizontal-pleiotropy), not an unconditional guarantee of validity.

#### Two-sample Mendelian randomization

↑ **Parent:** [Mendelian randomization](#mendelian-randomization)

Two-sample [Mendelian randomization](#mendelian-randomization) combines [genetic variant](biology.md#genetic-variant) associations with an [exposure](#exposure) estimated in one sample and their associations with an outcome estimated in another. It requires the [instrumental variable](#instrumental-variable) assumptions and compatible associations across the populations; sample overlap can change the behaviour of [weak instruments](#weak-instrument).

#### Horizontal pleiotropy

↑ **Parent:** [Mendelian randomization](#mendelian-randomization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horizontal_pleiotropy)

Horizontal pleiotropy occurs when a genetic instrument affects an outcome through a pathway other than the exposure under study. It violates the [exclusion restriction](#exclusion-restriction) in [Mendelian randomization](#mendelian-randomization).

#### Residual exposure stratification

↑ **Parent:** [Mendelian randomization](#mendelian-randomization)

Residual exposure stratification subtracts the genetically predicted component of an exposure before forming exposure strata. Under a suitable additive first-stage model, this avoids directly conditioning on the component caused by the instrument and can reduce the resulting [collider bias](#collider-bias).

### Confounder-instrument interaction

↑ **Parent:** [Instrumental variable](#instrumental-variable)

A confounder-instrument interaction occurs when an instrument's effect on treatment varies with a variable that also affects the outcome. If the conditional first-stage effect is $\delta(U)=\mathbb E[A\mid Z=1,U]-\mathbb E[A\mid Z=0,U]$, absence of this interaction means that $\delta(U)$ is constant.

### Instrumental-variable monotonicity

↑ **Parent:** [Instrumental variable](#instrumental-variable)

Instrumental-variable monotonicity requires changing the instrument in its encouraging direction never to move any unit's exposure in the opposite direction.

#### Local average treatment effect

↑ **Parent:** [Instrumental-variable monotonicity](#instrumental-variable-monotonicity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_average_treatment_effect)

The local average treatment effect is the average [causal effect](#causal-effect) among compliers, the units whose treatment status changes in the direction encouraged by the instrument.

## Interference in causal inference

↑ **Parent:** [Causal inference](causal-inference.md)

Interference occurs when one unit's treatment changes another unit's [potential outcome](#potential-outcome). It violates the usual assumption that each unit's potential outcomes depend only on that unit's own treatment.

## Ecological fallacy

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ecological_fallacy)

The ecological fallacy is an invalid inference about individuals from associations measured only for groups or populations.

### Aggregate composition does not identify offender composition

↑ **Parent:** [Ecological fallacy](#ecological-fallacy)

A positive association between a community's demographic composition and its incidence rate does not establish what proportion of incidents involved people from that demographic group. The same aggregate totals can be generated by different offender compositions and mechanisms. Individual incident records with age, sex and role would be needed to identify such proportions; aggregate regression coefficients concern community-level association.

## Causal directed acyclic graph

↑ **Parent:** [Causal inference](causal-inference.md)

A causal directed acyclic graph represents variables by vertices and direct causal relations by arrows. Its graphical separation rules encode conditional independences implied by the causal model.

### Causal minimality

↑ **Parent:** [Causal directed acyclic graph](#causal-directed-acyclic-graph)

A [probability distribution](probability-theory.md#probability-distribution) is causally minimal for a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) when it satisfies the [global Markov property for a directed acyclic graph](#global-markov-property-for-a-directed-acyclic-graph) for that graph and for no proper subgraph obtained by deleting edges on the same vertex set. It excludes redundant edges without excluding every extra [conditional independence](random-variable.md#conditional-independence).

#### Causally minimal nonfaithful Gaussian model

↑ **Parent:** [Causal minimality](#causal-minimality)

Let $E_1,E_2,E_3$ be [independent random variables](random-variable.md#independent-random-variables) with the [standard normal distribution](probability-theory.md#standard-normal-distribution) and set $Z_1=E_1$, $Z_2=Z_1+E_2$, $Z_3=Z_2-Z_1+E_3$. The complete acyclic graph with edges $1\to2$, $1\to3$, $2\to3$ is causally minimal: deleting each edge imposes a false marginal or conditional independence. Yet $Z_1\perp Z_3$ because $Z_3=E_2+E_3$, so [faithfulness of a directed acyclic graph](#faithfulness-of-a-directed-acyclic-graph) fails. Nonzero structural coefficients alone do not ensure faithfulness.

### PC algorithm

↑ **Parent:** [Causal directed acyclic graph](#causal-directed-acyclic-graph)

The PC algorithm starts with a candidate undirected graph, removes edges using [conditional independence](random-variable.md#conditional-independence) tests over increasing conditioning-set sizes, records separating sets, then orients unshielded colliders and propagates orientations. Under oracle tests and [faithfulness of a directed acyclic graph](#faithfulness-of-a-directed-acyclic-graph), it estimates the graph's Markov equivalence class.

#### Population PC correctness under faithfulness

↑ **Parent:** [PC algorithm](#pc-algorithm)

With an exact [conditional independence](random-variable.md#conditional-independence) oracle and [faithfulness of a directed acyclic graph](#faithfulness-of-a-directed-acyclic-graph), the skeleton phase of the [PC algorithm](#pc-algorithm) deletes precisely the nonedges. A true edge cannot be [D-separated](combinatorics.md#d-separation) by a set excluding its endpoints. For nonadjacent vertices, choose the later vertex $v$ in a [topological ordering](combinatorics.md#topological-ordering); its parents separate it from the earlier nonparent. True parent edges survive throughout, so this separator remains available among the algorithm's candidate neighbour sets. For an unshielded triple $u-v-w$, any recorded separator of $u,w$ excludes $v$ exactly when the triple is an [unshielded collider](combinatorics.md#unshielded-collider). The [skeleton and collider characterization of Markov equivalence](combinatorics.md#skeleton-and-collider-characterization-of-markov-equivalence) therefore identifies the correct equivalence class. Directions compelled throughout that class give its [completed partially directed acyclic graph](combinatorics.md#completed-partially-directed-acyclic-graph).

#### PC initialization from a conditional independence graph

↑ **Parent:** [PC algorithm](#pc-algorithm)

Initialize the PC skeleton search with an estimated [conditional independence graph](random-variable.md#conditional-independence-graph) to reduce candidate pairs and conditioning sets. An exact graph contains the true [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) skeleton because it equals its [moral graph](combinatorics.md#moral-graph) under faithfulness. For initially absent pairs record the full complement as a separating set; an empty default can create false collider orientations. Estimation errors can affect this screening step.

### Directed acyclic graph factorization

↑ **Parent:** [Causal directed acyclic graph](#causal-directed-acyclic-graph)

A distribution factorizes according to a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) when its joint density is the product of the conditional density of each variable given its graphical parents. This factorization implies the graph's [global Markov property of a directed acyclic graph](combinatorics.md#global-markov-property-of-a-directed-acyclic-graph).

#### Global Markov property for a directed acyclic graph

↑ **Parent:** [Directed acyclic graph factorization](#directed-acyclic-graph-factorization)

A distribution has the global Markov property for a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) when every [D-separation](combinatorics.md#d-separation) of vertex sets by a conditioning set implies the corresponding [conditional independence](random-variable.md#conditional-independence) of their random variables.

### Faithfulness of a directed acyclic graph

↑ **Parent:** [Causal directed acyclic graph](#causal-directed-acyclic-graph)

A distribution is faithful to a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) when, for all disjoint vertex sets $A,B,S$, $Z_A\perp Z_B\mid Z_S$ holds if and only if $A$ and $B$ are [D-separated](combinatorics.md#d-separation) by $S$. This includes the graph's [global Markov property of a directed acyclic graph](combinatorics.md#global-markov-property-of-a-directed-acyclic-graph) and excludes additional independences caused by parameter cancellations. If faithfulness is used to name only the reverse implication, the Markov property must be assumed separately.

### Nonparametric structural equation model

↑ **Parent:** [Causal directed acyclic graph](#causal-directed-acyclic-graph)

A nonparametric structural equation model assigns each observed variable an arbitrary measurable function of its graphical parents and an exogenous variable. Independence or dependence among exogenous variables determines the graph's latent-confounding structure.

### Acyclic directed mixed graph

↑ **Parent:** [Causal directed acyclic graph](#causal-directed-acyclic-graph)

An acyclic directed mixed graph contains directed edges without directed cycles and bidirected edges representing latent dependence. It extends a directed acyclic graph to causal models with unobserved common causes.

#### Verma constraint

↑ **Parent:** [Acyclic directed mixed graph](#acyclic-directed-mixed-graph)

A Verma constraint is an equality restriction on an observed distribution implied by a latent-variable causal graph that need not be a conditional independence. Such constraints can therefore distinguish latent causal models whose ordinary observed conditional-independence relations coincide.

#### District of an acyclic directed mixed graph

↑ **Parent:** [Acyclic directed mixed graph](#acyclic-directed-mixed-graph)

A district is a maximal set of vertices connected by a path consisting entirely of bidirected edges.

##### Fixable vertex

↑ **Parent:** [District of an acyclic directed mixed graph](#district-of-an-acyclic-directed-mixed-graph)

A vertex is fixable when its district contains no proper directed descendant of that vertex. Equivalently, $\operatorname{dis}(v)\cap\operatorname{de}(v)=\{v\}$.

#### M-separation

↑ **Parent:** [Acyclic directed mixed graph](#acyclic-directed-mixed-graph)

M-separation extends d-separation to mixed graphs: a path is open given a conditioning set when every noncollider is unconditioned and every collider has a conditioned descendant.

### Front-door adjustment

↑ **Parent:** [Causal directed acyclic graph](#causal-directed-acyclic-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Front-door_adjustment)

Front-door adjustment identifies an exposure effect through an observed mediator when the mediator intercepts every directed exposure-outcome path, the exposure-mediator relation has no unblocked backdoor path, and exposure blocks every backdoor path from mediator to outcome.

#### Conditional front-door adjustment

↑ **Parent:** [Front-door adjustment](#front-door-adjustment)

Conditional front-door adjustment applies the front-door argument within strata of observed covariates and then averages over those covariates. The covariates must remove exposure-mediator confounding, while the exposure together with the covariates must remove mediator-outcome confounding.

### Backdoor (causal analysis)

↑ **Parent:** [Causal directed acyclic graph](#causal-directed-acyclic-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Backdoor_(causal_analysis))

A backdoor path creates noncausal association by entering the exposure through an arrowhead rather than beginning with a causal arrow leaving it.

#### Backdoor path

↑ **Parent:** [Backdoor (causal analysis)](#backdoor-causal-analysis)

A backdoor path from exposure $X$ to outcome $Y$ begins with an arrow entering $X$. An adjustment set identifies the total effect when it blocks every such path without conditioning on descendants of $X$.

##### Backdoor adjustment set

↑ **Parent:** [Backdoor path](#backdoor-path)

A backdoor adjustment set contains no descendant of the exposure and blocks every [backdoor path](#backdoor-path) from the exposure to the outcome. Averaging the conditional outcome distribution over such a set identifies the total causal effect.

###### Sufficient adjustment set

↑ **Parent:** [Backdoor adjustment set](#backdoor-adjustment-set)

A sufficient adjustment set is a collection of pretreatment variables for which treatment and every relevant [potential outcome](#potential-outcome) are conditionally independent. Adjustment for that set identifies the corresponding causal contrast under consistency and positivity.

###### Minimal sufficient adjustment set

↑ **Parent:** [Sufficient adjustment set](#sufficient-adjustment-set)

A minimal sufficient adjustment set is a [sufficient adjustment set](#sufficient-adjustment-set) none of whose proper subsets is sufficient. Minimality is by set inclusion and does not imply minimum cardinality or uniqueness.

### Linear structural equation model

↑ **Parent:** [Causal directed acyclic graph](#causal-directed-acyclic-graph)

In a linear structural equation model, each variable is a linear combination of its graphical parents and an exogenous error term. Edge coefficients quantify direct effects.

#### Wright path tracing rule

↑ **Parent:** [Linear structural equation model](#linear-structural-equation-model)

Wright's path tracing rule expresses a covariance in a standardized linear structural equation model as a sum of products of edge coefficients over admissible unblocked paths.

## Potential outcomes framework

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Potential_outcomes_framework)

The potential outcomes framework represents causal effects by comparing outcomes assigned to the same unit under different hypothetical interventions.

### Principal stratification

↑ **Parent:** [Potential outcomes framework](#potential-outcomes-framework)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_stratification)

Principal stratification groups units by the joint values of their potential values of an intermediate variable under every treatment assignment. With a binary instrument and binary treatment, the principal strata are always-takers, never-takers, compliers, and defiers.

#### Principal stratum

↑ **Parent:** [Principal stratification](#principal-stratification)

A principal stratum is one group in a [principal stratification](#principal-stratification).

### Potential outcome

↑ **Parent:** [Potential outcomes framework](#potential-outcomes-framework)

A potential outcome $Y(a)$ is the outcome that would be observed under intervention $a$.

#### Causal effect

↑ **Parent:** [Potential outcome](#potential-outcome)

A causal effect compares potential outcomes under different interventions.

##### Homogeneous treatment effect

↑ **Parent:** [Causal effect](#causal-effect)

A treatment effect is homogeneous when the relevant contrast of [potential outcomes](#potential-outcome) is constant across units. For an additive treatment, this takes the form $Y(a)-Y(0)=\beta a$.

##### Causal null hypothesis

↑ **Parent:** [Causal effect](#causal-effect)

A causal null hypothesis states that an intervention has no effect on a specified potential-outcome contrast. A sharp causal null sets every unit's treated and untreated potential outcomes equal; an average causal null sets their population mean difference to zero.

###### Structural zero

↑ **Parent:** [Causal null hypothesis](#causal-null-hypothesis)

A structural zero is an outcome value fixed at zero by the data-generating mechanism under a specified intervention or condition, rather than a zero arising by chance.

##### Average treatment effect

↑ **Parent:** [Causal effect](#causal-effect)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Average_treatment_effect)

The average treatment effect is $\mathbb E[Y(1)-Y(0)]$ in a target population.

###### Conditional average treatment effect

↑ **Parent:** [Average treatment effect](#average-treatment-effect)

The conditional average treatment effect at covariates $X=x$ is

$$
\tau(x)=\mathbb E[Y(1)-Y(0)\mid X=x].
$$

###### Overlap-weighted average treatment effect

↑ **Parent:** [Conditional average treatment effect](#conditional-average-treatment-effect)

The overlap-weighted average treatment effect averages the [conditional average treatment effect](#conditional-average-treatment-effect) with weight proportional to $e(X)\{1-e(X)\}$, where $e(X)$ is the [propensity score](#propensity-score). It emphasizes covariate strata in which both treatments are plausible.

###### Heterogeneous treatment effect

↑ **Parent:** [Average treatment effect](#average-treatment-effect)

A heterogeneous treatment effect varies across units or covariate values rather than being constant throughout the population. The [conditional average treatment effect](#conditional-average-treatment-effect) describes one common form of this heterogeneity.

###### Average treatment effect on the treated

↑ **Parent:** [Average treatment effect](#average-treatment-effect)

The average treatment effect on the treated is $\mathbb E[Y(1)-Y(0)\mid A=1]$.

##### Causal risk ratio

↑ **Parent:** [Causal effect](#causal-effect)

For binary potential outcomes, the causal risk ratio compares intervention risks:

$$
\operatorname{CRR}=\frac{\mathbb E[Y(1)]}{\mathbb E[Y(0)]}.
$$

## Confounding

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Confounding)

Confounding is distortion of an exposure-outcome association by common causes or associated background variables.

### Case mix

↑ **Parent:** [Confounding](#confounding)

Case mix describes the distribution of patient characteristics affecting prognosis, such as age, severity, comorbidity and urgency. Comparing provider outcomes without accounting for case mix may confuse differences in patients with differences in care. Adjustment requires comparable, reliably measured baseline variables and does not remove all possible [confounding](#confounding).

#### Risk-adjusted provider comparison

↑ **Parent:** [Case mix](#case-mix)

A risk-adjusted provider comparison contrasts observed outcomes with outcomes expected from a prespecified patient-risk model, or standardizes providers to a common patient population. For individual fitted risks $p_i$, the expected event count is $\sum_i p_i$. Patient selection, model calibration, omitted risk factors, small samples and dependence between outcomes can still affect interpretation. [Funnel plots](statistical-inference.md#funnel-plot) display precision differences that an ordered league table can obscure.

<h3 id="simpson-s-paradox">Simpson's paradox</h3>

↑ **Parent:** [Confounding](#confounding)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simpson's_paradox)

A comparison can have the same direction within every background stratum but reverse after pooling strata with different group compositions. For example, let unexposed event risks be $0.001$ in a low-risk stratum and $0.05$ in a high-risk stratum, and multiply the odds by $2.7$ for exposure within each stratum. The exposed risks are then approximately $0.002695$ and $0.124424$. If 80% of unexposed subjects but only 1% of exposed subjects belong to the high-risk stratum, the pooled unexposed risk is $0.0402$ while the pooled exposed risk is about $0.003913$. Every conditional [odds ratio](statistical-modelling.md#odds-ratio) is above one, yet the pooled exposed risk is smaller. The differing background distributions create the reversal; this example does not identify a [causal effect](#causal-effect) without assumptions on how exposure was assigned.

### Confounder

↑ **Parent:** [Confounding](#confounding)

A confounder predicts both treatment assignment and outcome and can create a noncausal association.

## Ignorability

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ignorability)

Ignorability is an assumption under which treatment assignment carries no information about relevant potential outcomes after conditioning on specified covariates.

### Conditional exchangeability

↑ **Parent:** [Ignorability](#ignorability)

Conditional exchangeability requires $(Y(0),Y(1))\perp A\mid X$ for sufficient pretreatment covariates $X$.

## Positivity assumption

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positivity_assumption)

Positivity requires every compared treatment to have positive probability at each target covariate value.

## Inverse probability weighting

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_probability_weighting)

Inverse probability weighting reweights each observed outcome by the reciprocal probability of receiving its observed treatment, creating a weighted population in which treatment is balanced across measured covariates.

### Propensity score

↑ **Parent:** [Inverse probability weighting](#inverse-probability-weighting)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Propensity_score)

The propensity score is the conditional probability $\pi(X)=\mathbb P(A=1\mid X)$ of receiving a binary treatment given observed covariates. Under conditional exchangeability, conditioning on the propensity score balances the covariate distribution between treatment groups.

### Inverse-probability-weighted estimator of the average treatment effect

↑ **Parent:** [Inverse probability weighting](#inverse-probability-weighting)

For binary treatment, outcomes $Y_i$, and estimated [propensity score](#propensity-score) $\widehat e(X_i)$, the inverse-probability-weighted estimator is

$$
\widehat{\operatorname{ATE}}_{\rm IPW}
=\frac1n\sum_{i=1}^n\left\{
\frac{A_iY_i}{\widehat e(X_i)}-
\frac{(1-A_i)Y_i}{1-\widehat e(X_i)}
\right\}.
$$

It is consistent under [conditional exchangeability](#conditional-exchangeability), [consistency of potential outcomes](#consistency-in-causal-inference), [positivity in causal inference](#positivity-assumption), and a consistent propensity-score estimator.

### Overlap weight

↑ **Parent:** [Inverse probability weighting](#inverse-probability-weighting)

For binary treatment with propensity score $\pi(X)$, the overlap weight $\pi(X)\{1-\pi(X)\}$ emphasizes covariate strata in which both treatments occur with appreciable probability.

## Consistency in causal inference

↑ **Parent:** [Causal inference](causal-inference.md)

Consistency equates the observed outcome with the potential outcome under the treatment received.

## Effect modifier

↑ **Parent:** [Causal inference](causal-inference.md)

An effect modifier is a variable across whose values the causal effect differs.

## Selection bias

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Selection_bias)

Selection bias occurs when inclusion in the analyzed sample depends on variables related to the exposure and outcome, making the observed association differ from its target-population counterpart.

### Survivorship bias

↑ **Parent:** [Selection bias](#selection-bias)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Survivorship_bias)

Survivorship bias occurs when analysis conditions on remaining observable or event-free long enough to enter a sample, thereby excluding earlier failures and overrepresenting longer survivors.

### Collider bias

↑ **Parent:** [Selection bias](#selection-bias)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Collider_bias)

Collider bias arises when analysis conditions on a common effect of two variables, thereby creating a statistical association between its causes.

## Internal validity

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Internal_validity)

Internal validity is the extent to which an estimate identifies the intended effect within the population and setting actually studied.

## External validity

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/External_validity)

External validity is the extent to which a result transports or generalizes from the studied sample and setting to a target population.

## Regression discontinuity design

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regression_discontinuity_design)

A regression discontinuity design compares units immediately on either side of a treatment-assignment cutoff. Its causal interpretation requires potential outcomes to vary continuously through that cutoff in the absence of treatment.

## Difference-in-differences

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Difference-in-differences)

Difference-in-differences compares outcome changes across exposed and unexposed groups. Its standard identifying condition is that their untreated outcomes would have followed parallel trends.

## Matching (statistics)

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matching_(statistics))

Matching compares treated and control units with similar pretreatment covariates.

### Covariate balance

↑ **Parent:** [Matching (statistics)](#matching-statistics)

Covariate balance means treatment groups have similar pretreatment covariate distributions.

#### Standardized mean difference

↑ **Parent:** [Covariate balance](#covariate-balance)

A standardized mean difference divides a group mean difference by a pooled standard deviation.

This gives a dimensionless [effect size](statistical-inference.md#effect-size), so mean differences can be compared across measurement scales.

### Caliper matching

↑ **Parent:** [Matching (statistics)](#matching-statistics)

Caliper matching rejects candidate pairs whose distance exceeds a tolerance.

## Negative control outcome

↑ **Parent:** [Causal inference](causal-inference.md)

A negative control outcome cannot plausibly be caused by treatment, so an estimated effect can reveal bias.

Unlike treatment comparison alone, this [scientific control](statistical-modelling.md#scientific-control) checks for an association that should vanish under the intended causal model.

### Negative control group

↑ **Parent:** [Negative control outcome](#negative-control-outcome)

A negative control group is chosen so that the proposed causal mechanism should not operate in it. Reproducing the target association in that group is evidence for residual bias or an alternative mechanism.

## Sensitivity analysis for unmeasured confounding

↑ **Parent:** [Causal inference](causal-inference.md)

This sensitivity analysis quantifies how strong an omitted association must be to alter a causal conclusion.

### Bivariate probit model for endogenous treatment

↑ **Parent:** [Sensitivity analysis for unmeasured confounding](#sensitivity-analysis-for-unmeasured-confounding)

A bivariate probit model for a binary treatment and outcome uses latent equations

$$
A=\mathbf1_{\{X^T\alpha+U>0\}},\qquad
Y=\mathbf1_{\{A\beta+X^T\gamma+V>0\}},
$$

where $(U,V)$ has a [bivariate normal distribution](probability-and-statistics.md#bivariate-normal-distribution). Its correlation parameter represents dependence between the two latent disturbances; when nonzero, treatment is endogenous in the outcome equation.

## Randomized controlled trial

↑ **Parent:** [Causal inference](causal-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Randomized_controlled_trial)

Random treatment assignment makes treatment independent of baseline potential outcomes in expectation.

### Care-seeking effects on a recorded injury outcome

↑ **Parent:** [Randomized controlled trial](#randomized-controlled-trial)

A recorded medically attended injury depends both on an injury occurring and on care being sought and recorded. An intervention that changes recognition of injuries or the threshold for seeking care can change recorded attendance even without changing underlying injury incidence. A [randomized controlled trial](#randomized-controlled-trial) identifies an assignment effect on the measured endpoint; attributing that effect to biological injury prevention alone requires additional information about ascertainment and care seeking.

### Risk compensation in a prevention trial

↑ **Parent:** [Randomized controlled trial](#randomized-controlled-trial)

Risk compensation is a possible behavioral response to a prevention intervention: feeling better protected can reduce vigilance or increase exposure to hazards, partially offsetting the intervention's direct protective effect. It is a hypothesis to investigate, not a conclusion established merely by an unfavorable treatment comparison. A [randomized controlled trial](#randomized-controlled-trial) of the overall package estimates its net assignment effect, which can include both physical protection and behavioral changes.

### Cluster-randomized trial

↑ **Parent:** [Randomized controlled trial](#randomized-controlled-trial)

A cluster-randomized trial assigns whole groups, such as institutions, to an intervention rather than assigning individuals separately. Positive [intraclass correlation](variance.md#intraclass-correlation-coefficient) reduces independent information: the equal-size exchangeable approximation has [design effect](statistical-inference.md#design-effect) $1+(m-1)\rho$ for cluster size $m$. The number of independent randomized clusters also matters for inference. Cluster assignment does not itself remove requirements for [informed consent](biology.md#informed-consent) or justify dropping outcome ascertainment in the control arm.

### Selective outcome reporting

↑ **Parent:** [Randomized controlled trial](#randomized-controlled-trial)

Reporting a favorable prespecified outcome while omitting a less favorable one can give an exaggerated impression of consistency of evidence. Multiple primary outcomes should be summarized transparently even when some lack statistical significance. A short abstract can prioritize results, but should not hide a materially different primary result; absence of information does not by itself establish deliberate misconduct.

### Number needed to treat

↑ **Parent:** [Randomized controlled trial](#randomized-controlled-trial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Number_needed_to_treat)

For a beneficial intervention reducing an adverse-event risk from $p_C$ to $p_I$ over a stated follow-up period, the [number needed to treat](#number-needed-to-treat) is the reciprocal of the absolute risk reduction. Its clinical interpretation requires the population, outcome, horizon and comparison to be specified. Invert confidence limits for the risk difference in reversed order if both are positive. If the interval includes zero, the transformed confidence set is unbounded and may include both benefit and harm, rather than being one ordinary finite interval.

### Blinded outcome assessment

↑ **Parent:** [Randomized controlled trial](#randomized-controlled-trial)

An outcome assessor is kept unaware of randomized treatment assignment to limit differential questioning, interpretation and recording. This does not require the participant or intervention provider to be blinded. Participants can reveal their assignment, so standardized interviews and restricted records help preserve blinding. Blinding after assignment is different from [allocation concealment](#allocation-concealment) before enrollment.

### Intention-to-treat analysis

↑ **Parent:** [Randomized controlled trial](#randomized-controlled-trial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intention-to-treat_analysis)

An intention-to-treat analysis compares participants according to their randomized assignment, retaining that assignment even when they do not use the assigned intervention. Its [causal effect](#causal-effect) is the effect of assignment under the study's actual adherence pattern, rather than the effect of perfect adherence. [Randomization](#randomization) protects this comparison from baseline [confounding](#confounding); [missing data](probability-and-statistics.md#missing-data) can still require assumptions or additional analysis.

#### Treatment contamination

↑ **Parent:** [Intention-to-treat analysis](#intention-to-treat-analysis)

Treatment contamination occurs when participants in one arm of a [randomized controlled trial](#randomized-controlled-trial) receive an intervention assigned to another arm. This is distinct from [contamination](statistical-inference.md#contamination-statistics) in robust estimation. The [intention-to-treat analysis](#intention-to-treat-analysis) still compares randomized assignments, but intervention receipt becomes less separated between the arms, often diluting the assignment effect. Receipt-based comparisons can introduce [confounding](#confounding) because receipt need not be randomized.

##### Symmetric treatment crossover attenuates a risk difference

↑ **Parent:** [Treatment contamination](#treatment-contamination)

Assume treatment receipt gives event risk $p_1$, nonreceipt gives risk $p_0$, and a fraction $c$ in each equally sized randomized arm crosses to the opposite treatment. The two assignment risks are $(1-c)p_1+cp_0$ and $cp_1+(1-c)p_0$. Subtracting yields the displayed attenuation, with $\Delta_{\rm receipt}=p_0-p_1$. It depends on the stated equal crossover fractions and unchanged receipt-specific risks; it is not a universal formula for every form of [treatment contamination](#treatment-contamination).

#### Post-randomization adjustment changes a treatment estimand

↑ **Parent:** [Intention-to-treat analysis](#intention-to-treat-analysis)

A treatment consequence is not interchangeable with a [baseline covariate](statistical-model.md#baseline-covariate) in an [intention-to-treat analysis](#intention-to-treat-analysis). Let randomized $Z$ be independent of $U,\varepsilon$, and let actual intervention use be $D=Z+U$, with $Y=D+\varepsilon$ and independent centered errors. The assignment changes the mean outcome by one. But the [conditional expectation](measure-theory.md#conditional-expectation) $\mathbb E[Y\mid Z,D]=D$ has coefficient zero on $Z$. Thus adjustment for the post-randomization variable $D$ changes the [estimand](statistical-inference.md#estimand) even in a simple identified [linear regression](linear-regression.md).

### Randomization

↑ **Parent:** [Randomized controlled trial](#randomized-controlled-trial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Randomization)

Randomization assigns experimental units to treatments using a random mechanism, allowing treatment-group differences to be calibrated against the known assignment distribution.

#### Randomized minimization in clinical trials

↑ **Parent:** [Randomization](#randomization)

For each new eligible participant, compare the imbalance that would result from each treatment assignment across prespecified baseline [covariate](statistical-model.md#covariate) margins. Assign with a probability favoring the less imbalanced choice, while retaining a random component and [allocation concealment](#allocation-concealment). This targets marginal balance when a large number of joint strata makes [stratified randomization](#stratified-randomization) with blocks inefficient. It is a sequential allocation rule, and inference should respect its design.

#### Stratified randomization

↑ **Parent:** [Randomization](#randomization)

Divide participants into strata defined by prespecified baseline prognostic variables and randomize independently within each [stratum](survival-analysis.md#stratum). Permuted blocks can keep treatment counts close throughout recruitment. This balances the stratification variable between arms by design, while [allocation concealment](#allocation-concealment) keeps upcoming assignments hidden. Analyses should account for important design strata where appropriate.

##### Permuted-block randomization

↑ **Parent:** [Stratified randomization](#stratified-randomization)

Within each prespecified [stratum](survival-analysis.md#stratum), choose a block containing fixed equal counts of the two treatment assignments, then randomly permute their order. Every completed block gives exact treatment balance. Variable block sizes and [allocation concealment](#allocation-concealment) protect against predicting the next assignment. Incomplete final blocks permit a small unavoidable imbalance; odd stratum sizes cannot have exact equal allocation.

#### Allocation concealment

↑ **Parent:** [Randomization](#randomization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Allocation_concealment)

Allocation concealment prevents those deciding whether to enroll an eligible participant from knowing the upcoming randomized assignment. It protects the [randomized controlled trial](#randomized-controlled-trial) against selection based on that assignment. It concerns access to the assignment before enrollment; keeping participants or assessors unaware after assignment is a separate design feature.

#### Restricted randomization

↑ **Parent:** [Randomization](#randomization)

[Restricted randomization](#restricted-randomization) samples assignments from a specified subset preserving features such as block balance, fixed group sizes or allowable treatment sequences. Inference must respect the chosen allocation scheme rather than treating all label permutations as admissible.

#### Complete randomization

↑ **Parent:** [Randomization](#randomization)

Complete randomization chooses uniformly among all treatment assignments having prespecified treatment-arm sizes.

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (7)

- [Calcium intake](biology.md#calcium-intake)
- [Mephedrone](biology.md#mephedrone)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-34.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#3/f/solution)
- [Psychoactive drug](biology.md#psychoactive-drug)
