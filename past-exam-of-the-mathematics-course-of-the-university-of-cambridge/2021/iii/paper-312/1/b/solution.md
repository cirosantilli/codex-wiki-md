<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $dt=a\,d\tau$ and $\dot\phi=a^{-1}\phi'$, the interaction is

$$
S_{\rm int}=\frac\lambda{3!}\int d\tau\,d^3x\,a^2\phi'^2\phi,
\qquad
H_{\rm int}=-\frac\lambda{3!}\int d^3x\,a^2\phi'^2\phi
$$

to first order in $\lambda$. The tree-level [in-in formalism](../../../../../../keldysh-formalism.md) gives

$$
\langle\phi_{\mathbf k_1}\phi_{\mathbf k_2}\phi_{\mathbf k_3}\rangle
=2\operatorname{Im}\int_{-\infty(1-i\epsilon)}^0d\tau\,
\langle0|\phi_{\mathbf k_1}(0)\phi_{\mathbf k_2}(0)
\phi_{\mathbf k_3}(0)H_{\rm int}(\tau)|0\rangle.
$$

There are two [Wick contractions](../../../../../../wick-contraction.md) for each choice of the undifferentiated field at the vertex. With $K=k_1+k_2+k_3$, the stated [Bunch-Davies vacuum](../../../../../../bunch-davies-vacuum.md) mode obeys

$$
f_k(0)=\frac{H}{\sqrt{2k^3}},
\qquad
f_k^{*\prime}(\tau)=\frac{Hk^2\tau}{\sqrt{2k^3}}e^{ik\tau}.
$$

The two powers of $\tau$ from the differentiated modes cancel $a^2=1/(H^2\tau^2)$, and the remaining integral is

$$
\int_{-\infty(1-i\epsilon)}^0
(1-ik_i\tau)e^{iK\tau}\,d\tau
=-i\frac{K+k_i}{K^2}.
$$

Removing the momentum-conserving delta function, the [bispectrum from a time-derivative cubic scalar interaction](../../../../../../bispectrum-from-a-time-derivative-cubic-scalar-interaction.md) is therefore

$$
\boxed{
B(k_1,k_2,k_3)=
\frac{\lambda H^4}{12k_1^3k_2^3k_3^3K^2}
\left[
k_2^2k_3^2(K+k_1)+k_3^2k_1^2(K+k_2)
+k_1^2k_2^2(K+k_3)
\right]}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
