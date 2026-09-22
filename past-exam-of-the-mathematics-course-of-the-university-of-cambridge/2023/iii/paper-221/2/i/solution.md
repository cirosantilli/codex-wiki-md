<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [no unmeasured confounding assumption](../../../../../../conditional-exchangeability.md) is the conditional exchangeability statement

$$
(Y(0),Y(1))\perp A\mid X.
$$

Also assume [consistency of potential outcomes](../../../../../../consistency-in-causal-inference.md), no interference between units, and [positivity in causal inference](../../../../../../positivity-assumption.md), in particular $\mathbb P(A=0\mid X)>0$ on the covariate support of treated units. Then

$$
\begin{aligned}
\mathbb E[Y(0)\mid A=1]
&=\mathbb E\{\mathbb E[Y(0)\mid X,A=1]\mid A=1\}\\
&=\mathbb E\{\mathbb E[Y(0)\mid X,A=0]\mid A=1\}\\
&=\mathbb E\{\mu(X)\mid A=1\}.
\end{aligned}
$$

The first treated potential outcome equals the observed treated mean by consistency. Moreover,

$$
\mathbb E\{\mu(X)\mid A=1\}
=\frac{\mathbb E[A\mu(X)]}{\mathbb P(A=1)}
=\frac{\mathbb E[\pi(X)\mu(X)]}{\mathbb E[\pi(X)]}.
$$

Subtracting proves the displayed identification formula for the [average treatment effect on the treated](../../../../../../average-treatment-effect-on-the-treated.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
