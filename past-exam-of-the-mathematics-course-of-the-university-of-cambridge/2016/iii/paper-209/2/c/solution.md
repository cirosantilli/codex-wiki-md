<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $u$. Put $m=\varphi(u)$ and form the centered real vectors

$$
Y_j=\begin{pmatrix}\cos(uX_j)-\operatorname{Re}m\\ \sin(uX_j)-\operatorname{Im}m\end{pmatrix}.
$$

They are bounded [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md), so the [multivariate central limit theorem](../../../../../../multivariate-central-limit-theorem.md) applies to $n^{-1/2}\sum_jY_j=(\operatorname{Re}\mathcal C_n(u),\operatorname{Im}\mathcal C_n(u))^T$.

To identify its limiting [covariance matrix](../../../../../../covariance-matrix.md), put $Z=e^{iuX_1}-m$. Its [complex covariance](../../../../../../complex-covariance.md) and [pseudo-covariance](../../../../../../pseudo-covariance.md) are respectively

$$
V=\mathbb E|Z|^2=1-|m|^2,\qquad
P=\mathbb E Z^2=\varphi(2u)-m^2.
$$

For $Z=A+iB$, $|Z|^2=A^2+B^2$ and $Z^2=A^2-B^2+2iAB$. Thus

$$
\boxed{\Sigma(u)=\frac12\begin{pmatrix}V+\operatorname{Re}P&\operatorname{Im}P\\
\operatorname{Im}P&V-\operatorname{Re}P\end{pmatrix}.}
$$

The two conditions on $\Gamma(u)$ identify exactly this real [covariance matrix](../../../../../../covariance-matrix.md): the second is $\operatorname{Cov}_{\mathbb C}(\Gamma(u),\overline{\Gamma(u)})=\mathbb E\Gamma(u)^2$, with a conjugate in its second argument. A centered [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) is determined by its [covariance matrix](../../../../../../covariance-matrix.md), including when that matrix is singular. Therefore

$$
\boxed{(\operatorname{Re}\mathcal C_n(u),\operatorname{Im}\mathcal C_n(u))
\xrightarrow{d}(\operatorname{Re}\Gamma(u),\operatorname{Im}\Gamma(u)).}
$$

This proves [convergence in distribution](../../../../../../convergence-in-distribution.md) at each fixed $u$; it does not assert convergence of the entire [empirical characteristic process](../../../../../../empirical-characteristic-process.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
