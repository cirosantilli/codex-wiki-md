<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $X^x$ solve

$$
dX_s=b(X_s)\,ds+\sqrt{a(X_s)}\,dB_s,
\qquad X_0=x.
$$

The [Feynman-Kac formula](../../../../../../feynman-kac-formula.md) is

$$
u(t,x)=\mathbb E_x\left[
f(X_t)\exp\left(\int_0^tV(X_r)\,dr\right)\right].
$$

Fix $t$ and apply the two-variable [Itô formula](../../../../../../ito-s-lemma.md) to $F(s,y)=u(t-s,y)$ and the semimartingale vector $(s,X_s)$. Multiplying by

$$
R_s=\exp\left(\int_0^sV(X_r)\,dr\right)
$$

and using the [Itô product rule](../../../../../../ito-product-rule.md), the drift of $R_sF(s,X_s)$ is

$$
R_s(-\partial_tu+Lu+Vu)(t-s,X_s)\,ds=0.
$$

The remaining stochastic integral is a true martingale because the coefficients and derivatives are bounded. Taking expectations at $s=0$ and $s=t$ gives the formula.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
