<h1 id="a/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [Itô's formula](../../../../../ito-s-lemma.md) to $M_t=e^{N_t-\langle N\rangle_t/2}$. The quadratic-variation correction cancels the finite-variation term:

$$
dM_t=M_t\,dN_t,\qquad M_0=1.
$$

Localization of the integrand proves that $M$ is a nonnegative continuous [local martingale](../../../../../local-martingale.md).

For completeness, [Conditional Fatou lemma](../../../../../conditional-fatou-lemma.md) says that for nonnegative [random variables](../../../../../random-variable-split.md) $Y_n$,

$$
\mathbb E(\liminf Y_n\mid\mathcal F_s)
\leq\liminf\mathbb E(Y_n\mid\mathcal F_s).
$$

Choose a [localizing sequence](../../../../../localizing-sequence.md) $\tau_n\uparrow\infty$ such that each stopped $M$ is a [martingale](../../../../../martingale-split.md). Fatou first gives $\mathbb EM_t\leq1$. For $s<t$, its conditional form then gives

$$
\mathbb E(M_t\mid\mathcal F_s)
\leq\liminf_n M_{s\wedge\tau_n}=M_s.
$$

Thus **$M$ is a [supermartingale](../../../../../supermartingale.md)**.

A sufficient condition for it to be a true [martingale](../../../../../martingale-split.md) on $[0,T]$ is [Novikov's condition](../../../../../novikov-s-condition.md)

$$
\boxed{\mathbb E\exp(\tfrac12\langle N\rangle_T)<\infty.}
$$

Under this condition the [stochastic exponential](../../../../../doleans-dade-exponential.md) is a uniformly integrable [martingale](../../../../../martingale-split.md) on that finite interval. Requiring it for every finite $T$ gives the [martingale](../../../../../martingale-split.md) property at all finite times; it does not automatically give [uniform integrability](../../../../../uniform-integrability.md) as $t\to\infty$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
