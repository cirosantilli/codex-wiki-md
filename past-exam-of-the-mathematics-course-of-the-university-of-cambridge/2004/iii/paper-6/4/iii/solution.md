<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $F$ be the [convex hull](../../../../../../convex-hull.md) of all terms of the sequence, meaning the set of their finite [convex combinations](../../../../../../convex-combination.md). Suppose $B(0,\epsilon)\cap F=\varnothing$. Part (ii) then gives a [continuous linear functional](../../../../../../continuous-linear-functional.md) $S$ with $Sf\geq1$ for every $f\in F$. In particular $Sf_n\geq1$ for every $n$, contradicting $Sf_n\to0$. Therefore the ball meets $F$.

A point of that intersection is a finite combination $\sum_{k=1}^m\alpha_kf_{n_k}$ with nonnegative coefficients summing to one. Set $N=\max_k n_k$, combine repeated indices and insert zero coefficients for omitted indices. This gives

$$
\boxed{\lambda_j\geq0,\quad\sum_{j=1}^N\lambda_j=1,\qquad
\left\|\sum_{j=1}^N\lambda_j f_j\right\|<\epsilon.}
$$

Thus **zero lies in the [norm](../../../../../../norm.md) closure of the convex hull**. The same argument applies to every tail of the sequence and, by choosing errors tending to zero, also gives the usual [Mazur lemma](../../../../../../mazur-s-lemma.md). Completeness of $V$ is not required for this conclusion.

The hypothesis needed is precisely convergence to zero against every [continuous linear functional](../../../../../../continuous-linear-functional.md), namely [weak convergence](../../../../../../weak-convergence.md). The PDF says only “continuous” for the testing maps. If that is interpreted as including arbitrary nonlinear continuous maps, the constant map $T\equiv1$ makes the hypothesis impossible. The proof above establishes the substantive conclusion under the intended, weaker linear-testing hypothesis, and therefore also the implication under the literal stronger wording.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
