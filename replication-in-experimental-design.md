# Replication in experimental design

↑ **Parent:** [Design of experiments](design-of-experiments-split.md)

[Replication in experimental design](replication-in-experimental-design.md) repeats a [treatment](treatment.md) on multiple independent [experimental units](experimental-unit.md), so that variation between those units can inform a [treatment contrast](treatment-contrast.md) and its [standard error](standard-error.md). Repeated measurements on one [experimental unit](experimental-unit.md) can improve measurement precision without providing additional independent [treatment](treatment.md) [replication](replication-in-experimental-design.md). The [experimental unit](experimental-unit.md) is identified by where the [treatment](treatment.md) is applied, rather than by how many responses are recorded.[Experimental unit, “Why is the experimental unit important?” and “Know your experimental unit”, revised 31 October 2023](experimental-unit-nc3rs-experimental-design-assistant.md)

For a constructed example, grow one [plant](plant.md) in each of eight separate pots. Apply [treatment](treatment.md) A to four pots and [treatment](treatment.md) B to four pots, without sharing drainage water between pots. Measure the [length](length.md) of three [leaves](leaf.md) per pot. The pot is the [experimental unit](experimental-unit.md); the [leaf](leaf.md) is the [observational unit](observational-unit.md). There are four [treatment](treatment.md) [replicates](replicate.md) per group, eight [experimental units](experimental-unit.md) overall, and $8\cdot3=24$ measurements. The three [leaves](leaf.md) in one pot are [nested measurements](nested-measurements.md), because they share the same [plant](plant.md) and [treatment](treatment.md) application. The setup assumes that pots do not affect one another; simply putting them in separate containers does not establish statistical [independence](independent-random-variables.md).

<a id="image-constructed-two-treatment-design-eight-pot-experimental-units-contain-twenty-four-leaf-observational-units"></a>
![](experimental-replication-pots-and-leaves.png)

**[Figure 1](#image-constructed-two-treatment-design-eight-pot-experimental-units-contain-twenty-four-leaf-observational-units). Constructed two-treatment design: eight pot experimental units contain twenty-four leaf observational units**. Each outlined pot receives one [treatment](treatment.md) application and supplies three [nested measurements](nested-measurements.md). A pot label marks an [experimental unit](experimental-unit.md), not a measured response value.

[Randomization](randomization.md) chooses which [experimental units](experimental-unit.md) receive which [treatments](treatment.md); [replication](replication-in-experimental-design.md) supplies multiple [experimental units](experimental-unit.md) receiving the same [treatment](treatment.md). These solve different problems. In the balanced allocation above, choose the four A pots uniformly among the $\binom84=70$ possible [subsets](subset.md). A particular pot has [probability](probability.md) $1/2$ of receiving A. Given that one pot receives A, a second receives A with [conditional probability](conditional-probability.md) $3/7$, rather than $1/2$. Thus the assignments are not [independent random variables](independent-random-variables.md), even though the [experimental units](experimental-unit.md) can supply independent responses conditional on those assignments in a suitable [statistical model](statistical-model-split.md).

An actual [ecology](ecology-split.md) experiment illustrates why the distinction matters. In [Stuart H. Hurlbert](stuart-h-hurlbert.md)'s account, twelve experimental ponds initially received zero, fifty or 450 [fish](fish.md), with five, four and three ponds respectively. Preparation included assessing variation between ponds before introducing [fish](fish.md); allocation considered both location and existing differences between ponds. The zero-[fish](fish.md) ponds supplied the [scientific control](scientific-control.md). These were repeated [treatment](treatment.md) applications to ponds, not twelve samples from one pond.[Pseudoreplication and the Design of Ecological Field Experiments, pp. 194–195, combined or hybrid allocation approach and the Hurlbert–Mulla experiment](pseudoreplication-and-the-design-of-ecological-field-experiments-by-stuart-h-hurlbert.md)

The original article followed the southern California ponds for ten months. Its readouts included [zooplankton](zooplankton.md) populations and total [phytoplankton](phytoplankton.md); it reported decreases in some [zooplankton](zooplankton.md) populations and increased total [phytoplankton](phytoplankton.md).[Impacts of mosquitofish (Gambusia affinis) predation on plankton communities, abstract, Hydrobiologia 83, pp. 125–151, August 1981](impacts-of-mosquitofish-gambusia-affinis-predation-on-plankton-communities-by-stuart-h-hurlbert-and-mir-subhan-mulla.md) Repeated sampling within a pond helps describe its response through time, while ponds supply [treatment](treatment.md) [replication](replication-in-experimental-design.md). Unequal group sizes and initial pond variation matter for the [statistical model](statistical-model-split.md); the [treatment](treatment.md) counts alone do not establish equal [variances](variance-split.md) or independent responses.

**Table of contents**

- [Replicate](replicate.md)
- [Nested measurements](nested-measurements.md)
  - [Variance of nested measurements](variance-of-nested-measurements.md)
- [Biological replicate](biological-replicate.md)
  - [Between-replicate variation](between-replicate-variation.md)
- [Technical replicate](technical-replicate.md)

## ↑ Ancestors (7)

1. [Design of experiments](design-of-experiments-split.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Pseudoreplication](pseudoreplication.md)
- [Replication in experimental design](replication-in-experimental-design.md)
