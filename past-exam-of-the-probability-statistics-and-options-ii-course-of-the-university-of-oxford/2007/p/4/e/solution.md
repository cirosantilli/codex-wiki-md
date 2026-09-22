<h1 id="p/4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume $n\ge3$, so the corner entry is separate from the superdiagonal. For $A(\delta)$, the row radii are

$$
r_1=\delta+\epsilon,\qquad r_i=q=\tfrac14+\epsilon\ (2\le i<n),\qquad r_n=\tfrac14.
$$

Thus every [eigenvalue](../../../../../eigenvalue.md) lies in the union $\bigcup_iD(i,r_i)$. The discs with centers $2,\ldots,n$ remain mutually disjoint. The expanding disc centered at one meets the disc centered at $j$ exactly when $j-1\le\delta+\epsilon+r_j$.

Let $I_\delta=\{1\}\cup\{j\ge2:j-1\le\delta+\epsilon+r_j\}$. Then the union of discs indexed by $I_\delta$ contains exactly $|I_\delta|$ [eigenvalues](../../../../../eigenvalue.md); every other disc contains exactly one. Every isolated [eigenvalue](../../../../../eigenvalue.md) is real by conjugation and obeys $|\lambda-j|\le r_j$. Once discs merge, the second [Gershgorin circle theorem](../../../../../gershgorin-circle-theorem.md) gives a bound and count for their whole component, rather than one [eigenvalue](../../../../../eigenvalue.md) per original disc. [Eigenvalue](../../../../../eigenvalue.md) branches coming from that component stay in its union, but may no longer be distinguished by individual discs. These statements describe the bounds through all merger thresholds as $\delta$ increases.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [4](../../4.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
