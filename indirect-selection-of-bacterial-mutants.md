# Indirect selection of bacterial mutants

↑ **Parent:** [Replica plating](replica-plating.md)

[Indirect selection of bacterial mutants](indirect-selection-of-bacterial-mutants.md) recovers a source using a related sample's tested [phenotype](phenotype.md), rather than directly challenging the retained lineage. A positive example uses a surviving replica [biological colony](colony-biology.md) to locate its unexposed source. A negative example uses failure to grow in one condition to locate a source that does grow elsewhere. The second is particularly useful for finding [auxotrophy](auxotrophy.md): dependence on an externally supplied nutrient.

Construct a four-by-four teaching layout with rows A–D and columns 1–4. The master has 13 [biological colonies](colony-biology.md); A4, D1 and D4 are empty. A growth-supporting control replica grows at every occupied master site except B2 and C3. A replica lacking an assumed nutrient X grows at those same control sites except A2 and C1. All other requirements are stipulated equal. These are invented readouts, not observations from the [Lederberg replica plating experiment](lederberg-replica-plating-experiment.md).

<a id="image-an-original-replica-plating-map-separates-retrieval-candidates-unresolved-transfer-and-absent-sources"></a>
![](replica-plating-colony-map-retrieval.png)

**[Figure 4](#image-an-original-replica-plating-map-separates-retrieval-candidates-unresolved-transfer-and-absent-sources). An original replica plating map separates retrieval candidates, unresolved transfer and absent sources**. Constructed four-by-four master, control and nutrient-X-omission readouts, viewed in the same orientation. Blue discs mean growth. Orange rings identify A2 and C1 for recovery from the master. Red crosses mark B2 and C3, which lack growth even on the control; gray dashes mark positions empty on the master. The lower comparison distinguishes these three explanations of an empty restrictive-replica site. No measured data or published plate illustration is reproduced.

Let $M$, $C$ and $S$ be the [finite sets](finite-set.md) of sites with growth on the master, control and X-omission replica respectively. In this construction $S\subseteq C\subseteq M$, with [cardinalities](cardinality.md)

$$
|M|=13,\qquad |C|=11,\qquad |S|=9.
$$

The [set difference](set-difference.md)

$$
C\setminus S=\{\mathrm{A2},\mathrm{C1}\}
$$

contains the two condition-dependent candidates. Pick from A2 and C1 on the master, then compare fresh samples of each recovered source with and without X. Restoration of growth when X is supplied supports an X-requirement [phenotype](phenotype.md), subject to the [scientific controls](scientific-control.md); growth alone does not identify a particular [gene](gene.md) or [mutation](mutation.md).

By contrast,

$$
M\setminus C=\{\mathrm{B2},\mathrm{C3}\}
$$

is unresolved sampling or viability in this first comparison. Neither site should be counted as an X-requirement candidate. The three sites outside $M$ have no master source to recover at all. The short logical argument is membership testing: a candidate must belong to $C$, establishing control growth, and not belong to $S$, establishing the contrasting readout. Being outside $S$ alone supplies only the second condition. Among the seven empty X-omission sites, two are candidates, two are unresolved and three have no master source. The beauty of the method is that a shared location turns this logical distinction into a practical retrieval route.

## ↑ Ancestors (5)

1. [Replica plating](replica-plating.md)
2. [Molecular genetics](molecular-genetics-split.md)
3. [Genetics](genetics-split.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Indirect selection of bacterial mutants](indirect-selection-of-bacterial-mutants.md)
- [Replica plating](replica-plating.md)
- [Replica plating controls](replica-plating-controls.md)
