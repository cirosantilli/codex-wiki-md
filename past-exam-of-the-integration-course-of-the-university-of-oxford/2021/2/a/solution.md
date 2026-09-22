<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Near zero, $\sin x/x\to1$, so $|\sin x|/x^\alpha$ is comparable to $x^{1-\alpha}$. The [power integral test](../../../../improper-power-integral.md) shows that the integral near zero is finite exactly when $\alpha<2$.

For the tail, $|\sin x|\leq1$ proves integrability when $\alpha>1$. To prove necessity, take the disjoint [intervals](../../../../interval-mathematics.md)

$$
I_k=[2k\pi+\pi/6,\ 2k\pi+5\pi/6],\qquad k\geq1.
$$

On each, $\sin x\geq1/2$, and $x\leq2\pi(k+1)$. Therefore $\int_{I_k}|\sin x|x^{-\alpha}\,dx\geq c_\alpha(k+1)^{-\alpha}$ with $c_\alpha>0$. The [p-series](../../../../p-series.md) diverges when $\alpha\leq1$, proving that the absolute tail integral diverges in that range.

Combining the two conditions,

$$
\boxed{f_\alpha\text{ is Lebesgue integrable on }(0,\infty)\iff1<\alpha<2.}
$$

For $0<\alpha\leq1$, the tail [improper integral](../../../../improper-integral.md) converges conditionally by the [Dirichlet test for improper integrals](../../../../dirichlet-test-for-improper-integrals.md), but that does not give [Lebesgue integrability](../../../../integrability.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
