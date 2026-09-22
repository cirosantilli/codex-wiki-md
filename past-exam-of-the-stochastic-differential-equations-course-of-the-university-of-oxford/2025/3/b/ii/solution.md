<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The stopped representation from part (a)(ii) and the [Itô isometry](../../../../../ito-isometry.md) give the exact second-moment identity

$$
\boxed{\mathbb E[M_{t\wedge T}^2]
=1+\mathbb E\int_0^{t\wedge T}\frac{e^{2X_s}}{(1+X_s^2)^2}\,ds.}
$$

The cross term with the initial value is zero because the stopped [stochastic integral](../../../../../stochastic-integral.md) has zero mean. This is the useful finite-time computation; evaluating the remaining occupation integral explicitly is unnecessary for proving integrability of $T$.

For $|x|\leq L$,

$$
\frac{e^{2x}}{(1+x^2)^2}\geq c_L,
\qquad c_L=\frac{e^{-2L}}{(1+L^2)^2}>0.
$$

Combining the second-moment identity with part (i) yields

$$
1+c_L\mathbb E[t\wedge T]\leq\mathbb E[M_{t\wedge T}^2]\leq e^{2L}.
$$

Let $t\to\infty$ and use [monotone convergence](../../../../../monotone-convergence-theorem.md):

$$
\boxed{\mathbb ET\leq e^{2L}(1+L^2)^2(e^{2L}-1)<\infty.}
$$

In particular $T<\infty$ [almost surely](../../../../../almost-sure-convergence.md), a conclusion obtained without assuming finite exit in the stopping argument.

One can also evaluate the limiting second moment exactly. At exit $M_T$ is either $e^{-L}$ or $e^L$, so

$$
M_T^2=(e^L+e^{-L})M_T-1.
$$

By [bounded convergence theorem](../../../../../bounded-convergence-theorem.md) and part (i), $\mathbb EM_T=1$. Therefore

$$
\boxed{\lim_{t\to\infty}\mathbb E[M_{t\wedge T}^2]
=\mathbb EM_T^2=e^L+e^{-L}-1.}
$$

The same bound also holds at every finite time, by applying $(y-e^{-L})(y-e^L)\leq0$ to $y=M_{t\wedge T}$ and taking [expected values](../../../../../expected-value-split.md). It improves the preceding bound to $\mathbb ET\leq c_L^{-1}(e^L+e^{-L}-2)$ if desired.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
