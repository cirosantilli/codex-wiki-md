<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $z=(x,y)$ and $\mu(dz)=\lambda(z)\,dz$. Treat the nonnegative plant weights as [independent](../../../../../independent-random-variables.md) marks conditional on the locations, with a [measurable](../../../../../measurability.md) mark law $K_z(dw)$ depending only on $z$. Its first and second moments are

$$
\int w\,K_z(dw)=m(z),\qquad\int w^2\,K_z(dw)=m(z)^2+v(z).
$$

This is the independent-marking interpretation appropriate for location-dependent weights.

The general results needed are the following. The [Independent marking theorem for Poisson point processes](../../../../../independent-marking-theorem-for-poisson-point-processes.md) says that such marks turn a [Poisson point process](../../../../../poisson-point-process.md) of intensity $\mu$ into a [Poisson point process](../../../../../poisson-point-process.md) on location-mark space with intensity $\nu(dz,dw)=\mu(dz)K_z(dw)$. The [Campbell first-moment formula](../../../../../campbell-first-moment-formula.md) says that for any nonnegative [measurable](../../../../../measurability.md) $g$, $\mathbb E\sum_{u\in\Pi}g(u)=\int g\,d\nu$, allowing infinite values. The second [Poisson factorial moment measure](../../../../../poisson-factorial-moment-measure.md) identity says that for nonnegative [measurable](../../../../../measurability.md) $h$,

$$
\mathbb E\sum_{u,u'\in\Pi,\ u\ne u'}h(u,u')=\iint h(u,u')\,\nu(du)\nu(du').
$$

These statements apply to sigma-finite intensities and therefore do not require finitely many plants in the entire field. We use these general results without proving them.

Define the total as the nonnegative sum $W=\sum_{(z,w)\in\Pi}w$, or equivalently as the increasing limit of its finite-intensity truncations. the [Campbell theorem](../../../../../campbell-s-theorem.md) gives

$$
\mathbb EW=\int_S\int_0^\infty w\,K_z(dw)\,\mu(dz)=\int_Sm(z)\lambda(z)\,dz=:M.
$$

Since $M<\infty$, the nonnegative [random variable](../../../../../random-variable-split.md) $W$ cannot be infinite on an event of positive [probability](../../../../../probability.md). Thus **$W$ is finite [almost surely](../../../../../almost-sure-convergence.md)**, even if the number of plants is infinite.

Separate the square into its diagonal and ordered distinct-pair terms. Nonnegativity allows the use of [Tonelli's theorem](../../../../../tonelli-theorem.md) and increasing limits, giving

$$
\begin{aligned}
\mathbb EW^2
&=\mathbb E\sum_{(z,w)\in\Pi}w^2+\mathbb E\sum_{(z,w)\ne(z',w')}ww'\\
&=\int_S\bigl(m(z)^2+v(z)\bigr)\lambda(z)\,dz+M^2.
\end{aligned}
$$

The assumed second [integral](../../../../../integral.md) is finite, so $W$ is [square-integrable](../../../../../square-integrable-function.md). Subtracting $(\mathbb EW)^2$ yields

$$
\boxed{\mathbb EW=\int_Sm\lambda\,dz,\qquad\operatorname{Var}W=\int_S(v+m^2)\lambda\,dz.}
$$

The term $v$ accounts for random weights at fixed locations; the term $m^2$ accounts for the [Poisson](../../../../../poisson-distribution.md) fluctuations in the locations and count. Nonnegativity is natural for weights. For signed marks, absolute first-moment integrability, rather than just a conditionally convergent [integral](../../../../../integral.md) of the signed [mean](../../../../../expected-value.md), would be needed for the ordinary sum.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
