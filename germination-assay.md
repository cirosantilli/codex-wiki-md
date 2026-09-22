# Germination assay

↑ **Parent:** [Germination](germination.md)

A specified test for [germination](germination.md), recording the endpoint, conditions and observation window. For a proposed red/far-red [light](light.md) test, use [randomization](randomization.md) to allocate one [seed](seed.md) lot to darkness, red, red then far-red, and red then far-red then red. Match hydration, [temperature](temperature-split.md), handling and elapsed time before counting; use sham waiting periods to equalize schedules. Use dish [replication](replication-in-experimental-design.md), retain the dark [scientific control](scientific-control.md), and record [radicle](radicle.md) emergence using an observation procedure that does not itself provide an uncontrolled [light](light.md) treatment. This is a proposed design, not a claim about the 1952 paper's [randomization](randomization.md) or [replication](replication-in-experimental-design.md).

As an original hypothetical counting example, begin with $N=40$ [seeds](seed.md) in one dish. Suppose 12 first meet the [radicle](radicle.md) endpoint by 24 hours, eight additional [seeds](seed.md) by 48 hours, and four additional [seeds](seed.md) by 72 hours. These invented event counts give

$$
g(24)=12,\qquad g(48)=12+8=20,\qquad g(72)=12+8+4=24,
$$

and cumulative [sample proportions](sample-proportion.md) $\widehat G(24)=0.30$, $\widehat G(48)=0.50$ and $\widehat G(72)=0.60$. The 48-hour increment is $8/40=0.20$, not $0.50$; the latter includes earlier events. Counting the same emerged [radicle](radicle.md) again at each inspection would inflate the total. These numbers illustrate bookkeeping, not biological rates or treatment effects.

With a fixed denominator and irreversible classification of the first endpoint event, the [set](set-split.md) counted at an earlier inspection is a [subset](subset.md) of the [set](set-split.md) counted later. Hence $0\leq\widehat G(t)\leq1$ and $\widehat G(t)$ cannot decrease. This short proof applies to cumulative [germination](germination.md) counts even if a later [seedling](seedling.md) dies. A count of currently surviving [seedlings](seedling.md) has a different definition and can decrease.

For treatment comparisons, the dish may be the [experimental unit](experimental-unit.md): [seeds](seed.md) in the same dish share conditions. Forty [seeds](seed.md) in one dish do not supply forty independent dish replicates. Report the [sample size](sample-size.md), [replication](replication-in-experimental-design.md), endpoint time and denominator; a [sample proportion](sample-proportion.md) by a deadline measures this assay's outcome, not an unconditional fraction with [seed viability](seed-viability.md).

## ↑ Ancestors (7)

1. [Germination](germination.md)
2. [Seed](seed.md)
3. [Plant](plant.md)
4. [Eukaryote](eukaryote.md)
5. [Organism](organism-split.md)
6. [Biology](biology-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Germination](germination.md)
- [Seed viability](seed-viability.md)
