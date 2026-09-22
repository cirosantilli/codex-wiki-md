<h1 id="2/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There are $6^3=216$ unrestricted placements, since one colour has $\binom42=6$ occupancy vectors. For any specified empty box, the two remaining boxes admit $3^3=27$ placements. For any specified pair of empty boxes, the one remaining box admits one placement. All three boxes cannot be empty.

The [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) therefore gives

$$
\boxed{216-3(27)+\binom32(1)=138.}
$$

The empty-box events are not [disjoint events](../../../../../../disjoint-events.md), so subtracting their counts without restoring their pairwise overlaps would be incorrect.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
