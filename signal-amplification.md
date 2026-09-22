# Signal amplification

↑ **Parent:** [Signal transduction](signal-transduction.md)

[Signal amplification](signal-amplification.md) is an increase in a specified downstream response relative to an initiating signal. In a molecular-count description, one activated component can generate or activate many downstream [molecules](molecule.md). Repeated [catalysis](catalysis.md) by an [enzyme](enzyme.md) supplies a mechanism: the [enzyme](enzyme.md) remains available for another [chemical reaction](chemical-reaction.md). Successive stages can multiply the response. For a biological example, Cooper describes the [epinephrine](adrenaline.md)-to-[glycogen phosphorylase](glycogen-phosphorylase.md) pathway, where production of many [cAMP](cyclic-adenosine-monophosphate.md) [molecules](molecule.md) and repeated downstream [protein](protein.md) [phosphorylation](phosphorylation.md) provide opportunities for [signal amplification](signal-amplification.md). This is an example, not a claim that every [signal transduction](signal-transduction.md) pathway has the same stages or gain. [Pathways of Intracellular Signal Transduction](the-cell-a-molecular-approach-2nd-edition-by-geoffrey-m-cooper/pathways-of-intracellular-signal-transduction.md)

Here is a counting toy extending the example under [signal transduction](signal-transduction.md). Suppose $N_0$ activated [receptors](receptor-biochemistry.md) each activate $a=5$ distinct relay [proteins](protein.md) during a first interval. During a subsequent interval, each relay activates $b=20$ distinct target [proteins](protein.md). Assume enough inactive relays and targets, no shared targets, and no loss of activity during the count. Then

$$
N_1=aN_0,\qquad N_2=bN_1=abN_0.
$$

For $N_0=1$, this gives $N_1=5$ and $N_2=100$: the target-to-[receptor](receptor-biochemistry.md) count [ratio](ratio.md) is $100$. These are assumed integer counts, not measured rates or a universal physiological amplification factor. The intervals are sequential; the equations do not specify a time course.

<a id="image-a-counting-toy-for-signal-amplification-and-a-finite-target-pool"></a>
![](second-messenger-amplification.png)

**[Figure 3](#image-a-counting-toy-for-signal-amplification-and-a-finite-target-pool). A counting toy for signal amplification and a finite target pool**. Original schematic and computed count curves, not measured biological data. The upper cascade assumes five relays per activated [receptor](receptor-biochemistry.md) and twenty distinct targets per relay. The lower comparison limits the entire target pool to $T=250$ initially inactive [proteins](protein.md), with enough time and access to activate every reachable target and no deactivation. The joining lines only guide the eye between integer counts.

Availability limits the multiplication. As a second toy assumption, let there be only $T=250$ initially inactive target [proteins](protein.md) shared by all branches, and suppose the branches can activate distinct targets until this pool is exhausted. Then

$$
N_2=\min(abN_0,T)=\min(100N_0,250).
$$

Two activated [receptors](receptor-biochemistry.md) give $200$ active targets, whereas three give $250$, not $300$. At three activated [receptors](receptor-biochemistry.md), the total count [ratio](ratio.md) is $250/3\simeq83.3$; adding a fourth activates no additional targets. Thus total output per input and the increment caused by an extra input are different notions of gain. This finite-pool rule is an illustrative bound, not an [enzyme kinetics](enzyme-kinetics.md) law.

[Signal amplification](signal-amplification.md) makes a small initiating signal capable of a larger response, but it does not supply the material or [energy](energy.md) for downstream [chemical reactions](chemical-reaction.md). In the [second messenger](second-messenger.md) transfer experiment, both stages still required added [ATP](adenosine-triphosphate.md) and [magnesium](magnesium.md) [ions](ion.md). Counts, changes in [concentration](concentration.md), and changes in [enzyme](enzyme.md) activity are different readouts; an amplification claim should name its input, output and observation interval. [Rall and Sutherland (1958), methods: production and assay of cAMP](https://doi.org/10.1016/S0021-9258(19)77422-5)

## ↑ Ancestors (3)

1. [Signal transduction](signal-transduction.md)
2. [Biology](biology-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Metabotropic receptor](metabotropic-receptor.md)
- [Receptor binding occupancy](receptor-binding-occupancy.md)
- [Second messenger](second-messenger.md)
- [Signal amplification](signal-amplification.md)
- [Signal transduction](signal-transduction.md)
