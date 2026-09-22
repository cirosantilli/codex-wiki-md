<h1 id="30k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $S_1$ is [Gaussian](../../../../../../multivariate-normal-distribution.md), the terminal wealth $W_1$ is normal. For [constant absolute risk aversion utility](../../../../../../constant-absolute-risk-aversion-utility.md)

$$
U(x)=-e^{-\gamma x},
$$

the [moment-generating function](../../../../../../moment-generating-function.md) of a normal variable gives

$$
\mathbb E[U(W_1)]
=-\exp\left\{-\gamma\mathbb EW_1
+\frac{\gamma^2}{2}\operatorname{Var}(W_1)\right\}.
$$

Maximizing this expected utility is equivalent to maximizing

$$
\theta^Tb-\frac{\gamma}{2}\theta^TV\theta,
$$

after dropping a constant. The unique first-order condition is

$$
b-\gamma V\theta=0,
$$

and strict concavity gives

$$
\theta=\frac1\gamma V^{-1}b=\frac1\gamma\theta_m.
$$

It agrees with part (a) exactly when

$$
\boxed{
\gamma=\frac1\lambda
=\frac{\bigl(\mu-(1+r)S_0\bigr)^TV^{-1}
\bigl(\mu-(1+r)S_0\bigr)}
{w_1-(1+r)w_0}.
}
$$

For the usual risk-averse convention $\gamma>0$, the asserted correspondence assumes $w_1>(1+r)w_0$; under that natural target-return condition the choice is unique.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
