<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $f\in C(\mathbb T)$, define $E_j(f)=\inf_{T\in\mathcal T_j}\|f-T\|_\infty$, where $\mathcal T_j$ is the space of degree-at-most-$j$ [trigonometric polynomials](../../../../../../trigonometric-polynomial.md). The first [inverse theorem for trigonometric approximation](../../../../../../inverse-theorem-for-trigonometric-approximation.md) states that a universal constant $C$ satisfies

$$
\boxed{\omega(f,1/n)\le\frac Cn\sum_{j=0}^n E_j(f),\qquad n\ge1.}
$$

For perspective, take best approximants at dyadic degrees and telescope their differences. Each difference between consecutive approximants has [supremum norm](../../../../../../supremum-norm.md) at most twice the earlier error, and the [Bernstein inequality for trigonometric polynomials](../../../../../../bernstein-inequality-for-trigonometric-polynomials.md) multiplies that bound by its degree when differentiating. The resulting dyadic sum is bounded by the displayed sum because $E_j$ decreases with $j$; the remaining approximation error is also bounded by an average of earlier errors.

Now suppose $E_j(f)\le K j^{-\alpha}$ for large $j$, absorbing finitely many earlier terms into a constant. If $0<\alpha<1$, comparison with an [integral](../../../../../../integral.md) gives $\sum_{j=1}^n j^{-\alpha}=O(n^{1-\alpha})$. If $\alpha=1$, the same comparison gives $\sum_{j=1}^n j^{-1}=O(1+\ln n)$. Substitution proves **the requested two rates**:

$$
\boxed{\omega(f,1/n)=
\begin{cases}
O(n^{-\alpha}),&0<\alpha<1,\\
O(\ln n/n),&\alpha=1\quad(n\ge2).
\end{cases}}
$$

The logarithm is the endpoint contribution of the harmonic sum and cannot generally be removed, as the following [Weierstrass function](../../../../../../weierstrass-function.md) shows.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
