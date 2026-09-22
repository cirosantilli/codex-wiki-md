<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

View the necklace as a [cycle graph](../../../../../../cycle-graph.md). Between the white bead and $B$ there are two [edge-disjoint paths](../../../../../../edge-disjoint-paths.md), containing $k$ and $n-k$ links. The beads remain connected if and only if at least one of these paths is uncut.

There are $\binom n3$ equally likely cut [sets](../../../../../../set-split.md). Keeping the $k$-link path uncut requires all three cuts to be among its $n-k$ complementary links, giving $\binom{n-k}{3}$ choices. Keeping the other path uncut gives $\binom k3$ choices. These two events are disjoint because three links are cut and they cannot all lie in both complementary paths. Therefore

$$
\boxed{\mathbb P(B\text{ shares the white component})
=\frac{\binom{n-k}{3}+\binom k3}{\binom n3}.}
$$

Use $\binom a3=0$ for $0\le a<3$. The answer is unchanged by exchanging $k$ and $n-k$, so either orientation around the necklace gives the same value. This is the connectivity calculation for [random cuts of a cycle](../../../../../../random-cuts-of-a-cycle.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
