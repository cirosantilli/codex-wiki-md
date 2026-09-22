# Greedy-choice property

↑ **Parent:** [Greedy algorithm](greedy-algorithm.md)

A [greedy-choice property](greedy-choice-property.md) says that some optimal [feasible solution](feasible-point.md) contains the locally selected choice. Together with [optimal substructure](optimal-substructure.md) in the remaining instance, it allows repeated commitments. An [exchange argument](exchange-argument.md) often establishes this property.[Algorithms by Jeff Erickson; §4.3 General Pattern, printed pp. 164–165: exchange without worsening an optimum](algorithms-by-jeff-erickson/greedy-algorithms.md)

For [interval scheduling](interval-scheduling.md), a safe first choice need not belong to every optimal [feasible solution](feasible-point.md). When several optima exist, a commitment may exclude one while retaining another. The useful [loop invariant](loop-invariant.md) is that the accepted prefix can still be extended to an optimum. Merely keeping the accepted [intervals](interval-mathematics.md) compatible proves feasibility, which is a weaker claim.

**Table of contents**

- [Exchange argument](exchange-argument.md)

## ↑ Ancestors (4)

1. [Greedy algorithm](greedy-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Greedy algorithm](greedy-algorithm.md)
- [Greedy-choice property](greedy-choice-property.md)
- [Shortest-duration interval scheduling counterexample](shortest-duration-interval-scheduling-counterexample.md)
