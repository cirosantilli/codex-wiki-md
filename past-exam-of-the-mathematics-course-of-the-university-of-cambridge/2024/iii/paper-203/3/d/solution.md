<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because $\widetilde F$ solves the differential equation from part (c), the [Itô formula](../../../../../../ito-s-lemma.md) makes $\widetilde F(V_t)$ a [local martingale](../../../../../../local-martingale.md) before $\tau$. The defining [improper integral](../../../../../../improper-integral.md) converges at both endpoints: its integrand is asymptotic to $(-u)^{1-d}$ near zero and to $|u|^{d-3}$ at minus infinity. Since $1<d<2$, both exponents are integrable. Hence

$$
0\leq\widetilde F(v)\leq I:=\int_{-\infty}^0\frac{du}{(-u)^{d-1}(1-u)^{4-2d}}<\infty,
$$

so the stopped local martingale is a bounded martingale.

If $\tau_x<\tau_y$, then $V_t\to0$ and $\widetilde F(V_t)\to0$. If $\tau_y<\tau_x$, then $V_t\to-\infty$ and $\widetilde F(V_t)\to I$. The hitting times cannot coincide because $X_t-Y_t$ stays positive. The [optional sampling theorem for a supermartingale](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) and [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md) therefore give

$$
\widetilde F(v)=I\,\mathbb P(\tau_y<\tau_x)=I F(v).
$$

Consequently

$$
F(v)=c\widetilde F(v),
\qquad
c=I^{-1}>0,
$$

which is the [Two-sided SLE boundary swallowing probability](../../../../../../two-sided-sle-boundary-swallowing-probability.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
