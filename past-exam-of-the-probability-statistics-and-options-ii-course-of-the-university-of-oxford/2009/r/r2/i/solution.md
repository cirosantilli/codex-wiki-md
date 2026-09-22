<h1 id="r/r2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the equivalent bipartite formulation: the left set has $m$ [vertices](../../../../../vertex-graph-theory.md) and a [matching](../../../../../matching-graph-theory-split.md) must cover it. Necessity is immediate, since distinct matched partners for any left subset must all lie in its neighborhood.

For sufficiency, induct on $m$. The cases zero and one are immediate from the neighborhood condition. If a nonempty proper left subset $A$ satisfies $|N(A)|=|A|$, [induction](../../../../../mathematical-induction.md) matches $A$ into $N(A)$. For the remaining left [vertices](../../../../../vertex-graph-theory.md) and remaining right [vertices](../../../../../vertex-graph-theory.md), any subset $B$ has at least $|B|$ available neighbors: applying Hall's inequality to $A\cup B$ and removing the $|A|$ possible neighbors in $N(A)$ proves this. [Induction](../../../../../mathematical-induction.md) supplies the second [matching](../../../../../matching-graph-theory-split.md), and the two combine.

If no nonempty proper subset has equality, all such subsets have at least one extra neighbor. Choose any left [vertex](../../../../../vertex-graph-theory.md) and one of its neighbors and match them. After deleting the pair, each nonempty subset of the remaining left side originally was proper and had at least $|B|+1$ neighbors; losing the chosen right [vertex](../../../../../vertex-graph-theory.md) [leaves](../../../../../leaf-of-a-graph.md) at least $|B|$. [Induction](../../../../../mathematical-induction.md) completes the [matching](../../../../../matching-graph-theory-split.md). Thus

$$
\boxed{|N(A)|\ge|A|\text{ for every left subset }A}
$$

is sufficient as well as necessary. If the right set is infinite, any subset with infinitely many neighbors automatically meets the finite inequalities, and the same finite-left [induction](../../../../../mathematical-induction.md) applies.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [R2](../../r2.md)
3. [R](../../../r.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
