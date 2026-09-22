<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $F(\tau)=\sum_{M\mid N}c(M)E_2(M\tau)$ and $C=\sum_{M\mid N}c(M)/M$. For $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma_0(N)$, each divisor $M$ of $N$ also divides the lower-left entry $c$. Thus

$$
\gamma_M=\begin{pmatrix}a&Mb\\c/M&d\end{pmatrix}\in SL_2(\mathbb Z),\qquad M\gamma\tau=\gamma_M(M\tau).
$$

The full transformation of the [Eisenstein series of weight two](../../../../../../eisenstein-series-of-weight-two.md) consequently gives

$$
E_2(M\gamma\tau)=(c\tau+d)^2E_2(M\tau)+\frac{6c(c\tau+d)}{M\pi i}.
$$

Summing with the prescribed coefficients proves

$$
F(\gamma\tau)=(c\tau+d)^2F(\tau)+\frac{6c(c\tau+d)}{\pi i}C.
$$

If $C=0$, this is exactly the desired weight-two law. Conversely, test it at $\gamma=\begin{pmatrix}1&0\\N&1\end{pmatrix}\in\Gamma_0(N)$. Its anomaly factor $6N(N\tau+1)/(\pi i)$ is nonzero throughout the [upper half-plane](../../../../../../upper-half-plane-complex-analysis.md); if $F$ is modular it forces $C=0$. This proves [cancellation of weight-two Eisenstein anomalies](../../../../../../cancellation-of-weight-two-eisenstein-anomalies.md):

$$
\boxed{\sum_{M\mid N}c(M)E_2(M\tau)\text{ is modular of weight }2\text{ on }\Gamma_0(N)\iff\sum_{M\mid N}\frac{c(M)}M=0.}
$$

Equivalently the inverse-height terms cancel in $\sum c(M)E_2^*(M\tau)$, leaving precisely the holomorphic function $F$. Eliminating $c(1)$ shows that all such combinations are spanned by $E_2(\tau)-ME_2(M\tau)$ for $M>1$ dividing $N$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
