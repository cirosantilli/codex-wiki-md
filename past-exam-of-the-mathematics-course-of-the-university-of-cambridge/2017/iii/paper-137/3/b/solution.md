<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $D=(2\pi i)^{-1}d/dz=q\,d/dq$ and use the [Serre derivative](../../../../../../serre-derivative.md) $D_kf=Df-(k/12)E_2f$. Translation invariance of $f$ and the [Eisenstein series of weight two](../../../../../../eisenstein-series-of-weight-two.md) gives $D_kf(z+1)=D_kf(z)$.

Differentiate the weight-$k$ transformation $f(-1/z)=z^kf(z)$. The [chain rule](../../../../../../chain-rule.md) yields

$$
Df(-1/z)=z^{k+2}Df(z)+\frac{k}{2\pi i}z^{k+1}f(z).
$$

The assumed transformation of the [Eisenstein series of weight two](../../../../../../eisenstein-series-of-weight-two.md) gives

$$
\frac{k}{12}E_2(-1/z)f(-1/z)
=\frac{k}{12}z^{k+2}E_2(z)f(z)+\frac{k}{2\pi i}z^{k+1}f(z).
$$

Subtracting cancels the extra term. Hence $D_kf(-1/z)=z^{k+2}D_kf(z)$. Since $S$ and $T=\begin{pmatrix}1&1\\0&1\end{pmatrix}$ generate the [modular group](../../../../../../modular-group.md), these two transformations prove the weight-$k+2$ law for all its elements. Holomorphy on the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) follows from the formula.

For the [Fourier expansion of a modular form](../../../../../../fourier-expansion-of-a-modular-form.md) $f=\sum_{n\geq0}a_nq^n$, differentiation gives $Df=\sum_{n\geq1}na_nq^n$. The product of the convergent series for $E_2$ and $f$ likewise has no negative powers. Thus $D_kf$ is [holomorphic at a cusp](../../../../../../holomorphic-at-a-cusp.md) at infinity, and therefore at every cusp of the [modular group](../../../../../../modular-group.md). Its constant coefficient is $-ka_0/12$. Since $k>0$, it vanishes exactly when $a_0=0$. Consequently

$$
\boxed{D_kf\in M_{k+2}(\Gamma(1)),\qquad
D_kf\in S_{k+2}(\Gamma(1))\iff f\in S_k(\Gamma(1)).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
