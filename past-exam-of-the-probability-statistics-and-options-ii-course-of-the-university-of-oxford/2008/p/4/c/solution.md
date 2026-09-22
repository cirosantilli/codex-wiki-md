<h1 id="p/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At step $k$, choose a real shift $\mu_k$, factor $A_k-\mu_kI=Q_kR_k$, and set

$$
A_{k+1}=R_kQ_k+\mu_kI=Q_k^\mathsf TA_kQ_k.
$$

The last equality proves [orthogonal](../../../../../orthogonal-vectors.md) similarity at every step. Thus all iterates have the same [eigenvalues](../../../../../eigenvalue.md); if $A_k$ is symmetric, the last expression is symmetric, proving symmetry by [induction](../../../../../mathematical-induction.md).

For the specified [matrix](../../../../../matrix.md), let $e=(1,\ldots,1)^\mathsf T$. Then $A=I-2ee^\mathsf T/n$ and $e^\mathsf Te=n$, so $A^\mathsf T=A$ and $A^2=I$. It is a [Householder reflection](../../../../../householder-transformation.md), hence [orthogonal](../../../../../orthogonal-vectors.md). With the standard positive-diagonal QR convention, part (a) gives $Q=A$, $R=I$ at the first unshifted step, and therefore $A_1=RQ=A$. The same repeats forever: **the unshifted [algorithm](../../../../../algorithm-split.md) is stationary**.

If arbitrary diagonal signs in QR are allowed, $R=D$, $Q=AD$ for a sign [matrix](../../../../../matrix.md) $D$, and the next iterate is $DAD$. Its off-diagonal magnitudes are unchanged, so even then only sign changes occur, not progress toward a diagonal form. This explains the role of the usual convention in the literal stationary-iterate statement.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [P](../../../p.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
