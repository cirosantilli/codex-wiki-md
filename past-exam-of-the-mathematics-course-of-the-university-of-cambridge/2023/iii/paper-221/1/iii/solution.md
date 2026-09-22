<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write

$$
m(x_1,x_2,x_3)=\mathbb E[X_4\mid x_1,x_2,x_3].
$$

Since $X_1$ has no parents, its total effect has no [backdoor path](../../../../../../backdoor-path.md), and

$$
\tau_1
=\mathbb E[X_4\mid X_1=1]
-\mathbb E[X_4\mid X_1=0].
$$

For $X_2$, $X_3$ intercepts every directed path to $X_4$. Conditional on $X_1$, there is no unblocked backdoor path from $X_2$ to $X_3$, and $(X_1,X_2)$ blocks every backdoor path from $X_3$ to $X_4$. The [conditional front-door adjustment](../../../../../../conditional-front-door-adjustment.md) therefore gives

$$
\mu_2(x)=
\sum_{x_1,x_3}p(x_1)p(x_3\mid x_1,x)
\sum_{x_2'}m(x_1,x_2',x_3)p(x_2'\mid x_1),
$$

and

$$
\tau_2=\mu_2(1)-\mu_2(0).
$$

Part ii shows that the inner sum, after also averaging $X_4$, does not actually depend on $x_1$.

For $X_3$, $(X_1,X_2)$ is a sufficient [backdoor adjustment set](../../../../../../backdoor-adjustment-set.md). Hence

$$
\mu_3(x)=
\sum_{x_1,x_2}m(x_1,x_2,x)
p(x_2\mid x_1)p(x_1),
\qquad
\tau_3=\mu_3(1)-\mu_3(0).
$$

These three formulas identify the requested [average treatment effects](../../../../../../average-treatment-effect.md) from the observed joint distribution.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
