<h1 id="p/p4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $R=\epsilon+\delta$. Only the first row disc changes: it now has radius $R$. The other discs keep radii $r_i=1/4+\epsilon$ for $2\le i\le n-1$ and $r_n=1/4$. They remain mutually disjoint. As $R$ grows, the first disc joins an initial segment of these discs. Define $m$ as the largest index joined to it, or one if no other disc is joined. The joining condition for index $i$ is

$$
R+r_i\ge i-1.
$$

For an interior index this starts at $\delta=i-5/4-2\epsilon$, and for the final index at $\delta=n-5/4-\epsilon$. Until its joining threshold, disc $i$ contains a unique real [eigenvalue](../../../../../eigenvalue.md) and retains the bound $|\lambda_i-i|\le r_i$.

After the first $m$ discs have joined, the second theorem places exactly $m$ eigenvalues in their union and exactly one in each remaining disc. The cluster is bounded, for instance, by

$$
|z-1|\le\max\{R,m-1+r_m\}\quad(m\ge2),
$$

and by $|z-1|\le R$ when $m=1$. The union of the actual discs is a sharper enclosure. Once discs overlap, one cannot assign one [eigenvalue](../../../../../eigenvalue.md) to each individual disc merely by its centre; the theorem counts the whole separated cluster.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
