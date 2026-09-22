# CDK1 activity and protein abundance

↑ **Parent:** [Cyclin-dependent kinase 1](cyclin-dependent-kinase-1.md)

[CDK1 activity and protein abundance](cdk1-activity-and-protein-abundance.md) are different observables. A total-[CDK1](cyclin-dependent-kinase-1.md) [Western blot](western-blot.md) estimates [protein](protein-split.md) amount under its calibration and loading assumptions. A phosphosite-specific [Western blot](western-blot.md) asks about a particular [CDK1 phosphorylation state](cdk1-phosphorylation-state.md). A [histone H1 kinase assay](histone-h1-kinase-assay.md) asks how much [substrate](substrate-biochemistry.md) modification occurs under specified assay conditions. Any conversion between them needs a model and suitable controls.

An original counting example stipulates $100$ [CDK1](cyclin-dependent-kinase-1.md) [molecules](molecule-split.md), with $60$ bound to [cyclin B](cyclin-b.md) in each of two hypothetical samples. In sample A, $10$ bound [molecules](molecule-split.md) are activity-permissive and $50$ are inhibited; in sample B, $40$ are activity-permissive and $20$ are inhibited. The other $40$ are unbound in both samples. Total [CDK1](cyclin-dependent-kinase-1.md) and bound [CDK1](cyclin-dependent-kinase-1.md) agree, but activity-permissive counts differ fourfold. These are invented counts for bookkeeping, not measured biological populations.

If each activity-permissive [molecule](molecule-split.md) contributes the same [reaction rate](reaction-rate.md), [substrate](substrate-biochemistry.md) and [ATP](adenosine-triphosphate.md) remain available, and the assay stays linear in time, a simple illustrative readout is

$$
R-R_0=\alpha N_{\mathrm{active}}t.
$$

Here $R$ is the recorded signal, $R_0$ is a matched blank signal, $N_{\mathrm{active}}$ is the activity-permissive count, $t$ the reaction interval, and $\alpha$ a common signal contribution per active [molecule](molecule-split.md) per unit time. The corrected signals in the stipulated samples have [ratio](ratio.md) $40/10=4$, although their total [protein](protein-split.md) amounts agree. This is an assay accounting assumption, not an [ordinary differential equation](ordinary-differential-equation.md) for the [cell cycle](cell-cycle-split.md). The no-added-[cyclin B](cyclin-b.md) baseline in the inspected experiment can itself contain catalytic activity; it need not equal an enzyme-free blank $R_0$.

[Substrate](substrate-biochemistry.md) depletion, differing inhibitory conditions or a saturated detector can break the simple proportionality. Comparing samples therefore requires matched reaction intervals, [substrate](substrate-biochemistry.md) supply, loading and detector response, rather than assuming that brighter [histone H1](histone-h1.md) labeling automatically means more total [CDK1](cyclin-dependent-kinase-1.md).

## ↑ Ancestors (7)

1. [Cyclin-dependent kinase 1](cyclin-dependent-kinase-1.md)
2. [Cell-cycle activation feedback](cell-cycle-activation-feedback.md)
3. [Positive feedback](positive-feedback.md)
4. [Signaling feedback](signaling-feedback.md)
5. [Signal transduction](signal-transduction-split.md)
6. [Biology](biology-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [CDK1 activity and protein abundance](cdk1-activity-and-protein-abundance.md)
- [Cyclin B](cyclin-b.md)
