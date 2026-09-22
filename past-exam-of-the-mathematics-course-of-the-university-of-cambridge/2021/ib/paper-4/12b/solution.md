<h1 id="12b/solution">Solution</h1>

↑ **Parent:** [12B](../12b.md)

The [Laplace transform](../../../../../laplace-transform.md) of a function on $t\geq0$ is

$$
\widehat f(s)=\mathcal L\{f\}(s)
=\int_0^\infty e^{-st}f(t)\,dt,
$$

for values of $s$ for which the [integral](../../../../../integral.md) converges. [Integration by parts](../../../../../integration-by-parts.md) gives the [Laplace transform of a derivative](../../../../../laplace-transform-of-a-derivative.md)

$$
\boxed{\mathcal L\{f'\}(s)=s\widehat f(s)-f(0)}.
$$

Write $\widehat N_i(s)=\mathcal L\{N_i\}(s)$. Transforming the first two equations and using the initial data gives

$$
\widehat N_1(s)=\frac{N}{s+\lambda_1},
\qquad
\widehat N_2(s)
=\frac{N\lambda_1}{(s+\lambda_1)(s+\lambda_2)}.
$$

The third equation then gives

$$
(s+\lambda_3)\widehat N_3(s)-n
=\lambda_2\widehat N_2(s),
$$

and hence

$$
\widehat N_3(s)
=\frac n{s+\lambda_3}
+\frac{N\lambda_1\lambda_2}
{(s+\lambda_1)(s+\lambda_2)(s+\lambda_3)}.
$$

A [partial fraction decomposition](../../../../../partial-fraction-decomposition.md) therefore yields the [sequential radioactive decay](../../../../../sequential-radioactive-decay.md) formula

$$
\boxed{
\begin{aligned}
N_3(t)={}&ne^{-\lambda_3t}\\
&+N\lambda_1\lambda_2\left[
\frac{e^{-\lambda_1t}}{(\lambda_2-\lambda_1)(\lambda_3-\lambda_1)}
+\frac{e^{-\lambda_2t}}{(\lambda_1-\lambda_2)(\lambda_3-\lambda_2)}
+\frac{e^{-\lambda_3t}}{(\lambda_1-\lambda_3)(\lambda_2-\lambda_3)}
\right].
\end{aligned}
}
$$

Now let $\lambda_1=\lambda_2=\lambda$ and put $\Delta=\lambda_3-\lambda>0$. The transformed contribution originating from the initial $N_1$ population becomes

$$
\frac{N\lambda^2}{(s+\lambda)^2(s+\lambda_3)}.
$$

Equivalently, solve the middle equation first to obtain

$$
N_2(t)=N\lambda t e^{-\lambda t},
$$

and use an [integrating factor](../../../../../integrating-factor.md) in the final equation:

$$
N_3(t)=ne^{-\lambda_3t}
+N\lambda^2e^{-\lambda_3t}\int_0^t u e^{\Delta u}\,du.
$$

Evaluating the elementary integral gives

$$
\boxed{
N_3(t)
=ne^{-\lambda_3t}
+\frac{N\lambda^2}{(\lambda_3-\lambda)^2}
\left[
e^{-\lambda t}\bigl((\lambda_3-\lambda)t-1\bigr)
+e^{-\lambda_3t}
\right]
}.
$$

## ↑ Ancestors (10)

1. [12B](../12b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
