<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Under $H_0$, [conditional independence](../../../../../conditional-independence.md) gives

$$
\mathbb E[(x_1-f(z_1))(y_1-g(z_1))\mid z_1]=0.
$$

Multiplication by the measurable sign $s(z_1)$ and the [law of total expectation](../../../../../law-of-total-expectation.md) prove the first identity.

Write

$$
a_i=\widehat f(z_i)-f(z_i),
\qquad
b_i=\widehat g(z_i)-g(z_i).
$$

Then

$$
\tau_N
=\frac1n\sum_i\epsilon_i\xi_i s(z_i)
-\frac1n\sum_i\epsilon_i b_i s(z_i)
-\frac1n\sum_i\xi_i a_i s(z_i)
+\frac1n\sum_i a_ib_i s(z_i).
$$

Conditional orthogonality under $H_0$ and the variance bounds in (ii) give

$$
\sqrt n\,n^{-1}\sum_i\epsilon_i b_i s(z_i)
=O_p(\sqrt{\operatorname{MSPE}_g})=o_p(1),
$$

and similarly for the term containing $\xi_i a_i$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) bounds the last term by

$$
\left(n^{-1}\sum_i a_i^2\right)^{1/2}
\left(n^{-1}\sum_i b_i^2\right)^{1/2},
$$

which is $o_p(n^{-1/2})$ by $n\operatorname{MSPE}_f\operatorname{MSPE}_g\to0$.

The leading summands $\epsilon_i\xi_i s(z_i)$ are independent, centered, and have variance $\operatorname{Var}(\epsilon_1\xi_1)$ because $s^2=1$. The [central limit theorem](../../../../../central-limit-theorem.md) and consistency of $\tau_D$ therefore give, by the [Slutsky theorem](../../../../../slutsky-theorem.md),

$$
T=\frac{\sqrt n\,\tau_N}{\tau_D}
\xrightarrow dN(0,1).
$$

This is the [generalized covariance measure statistic](../../../../../generalized-covariance-measure-statistic.md).

Without the null, condition first on $(x_1,z_1)$. Since

$$
\mathbb E[\mathbb E(y_1\mid x_1,z_1)-\mathbb E(y_1\mid z_1)\mid z_1]=0,
$$

the term involving $\mathbb E(x_1\mid z_1)$ vanishes, giving

$$
\mathbb E[(x_1-\mathbb E(x_1\mid z_1))
(y_1-\mathbb E(y_1\mid z_1))s(z_1)]
=\mathbb E[x_1\{\mathbb E(y_1\mid x_1,z_1)
-\mathbb E(y_1\mid z_1)\}s(z_1)].
$$

For the specified alternative, independence and $\mathbb Ex_1=0$ make the right side

$$
\mathbb E(x_1^2)\mathbb E[h(z_1)s(z_1)].
$$

The constant choice $s=1$ gives zero because $\mathbb Eh(z_1)=0$, so no first-order power is expected. Taking

$$
s(z)=\operatorname{sgn}h(z)
$$

instead gives $\mathbb E(x_1^2)\mathbb E|h(z_1)|>0$, producing asymptotic power.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
