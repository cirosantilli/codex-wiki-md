<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At cubic order, the expansion of $P(X,\phi)$ produces the schematic operators

$$
\varphi'^3,quad
\varphi'(\nabla\varphi)^2,quad
\varphi\varphi'^2,quad
\varphi(\nabla\varphi)^2,quad
\varphi^2\varphi',quad
\varphi^3.
$$

The derivative self-interactions involving $P_{XX}$ and $P_{XXX}$ are generally largest when $c_s\ll1$, while coefficients containing explicit $\phi$ derivatives of a slowly varying $P$ are commonly slow-variation suppressed. The former therefore tend to dominate [primordial non-Gaussianity](../../../../../../primordial-non-gaussianity.md).

The terms contributing to $\varphi\varphi'^2$ are

$$
a^4P_{X\phi}\varphi\,\delta_2X
+\frac{a^4}{2}P_{XX\phi}\varphi(\delta_1X)^2.
$$

Thus

$$
S_3\supset\int d\tau\,d^3x\,a^2\lambda_0
\varphi\varphi'^2,
\qquad
\boxed{\lambda_0=\frac12(P_{X\phi}+2\bar XP_{XX\phi})}.
$$

Equivalently, if the complete time-dependent coefficient is called $\lambda$, then $\lambda(\tau)=a^2\lambda_0$.

Treat $\lambda_0$ as constant at leading slow variation. To cubic order the corresponding [interaction Hamiltonian](../../../../../../interaction-hamiltonian.md) is

$$
H_I=-a^2\lambda_0
\int_{\mathbf p_1\mathbf p_2\mathbf p_3}
(2\pi)^3\delta^{(3)}(\mathbf p_1+\mathbf p_2+\mathbf p_3)
\varphi_{\mathbf p_1}\varphi'_{\mathbf p_2}\varphi'_{\mathbf p_3}.
$$

For $q_i=c_sk_i$, the mode function above satisfies

$$
\varphi_k(0)=A_k,
\qquad
\varphi_k^{*\prime}(\tau)=A_kq_k^2\tau e^{iq_k\tau},
\qquad
A_k=\frac{H}{\sqrt{2c_sk^3}}.
$$

Writing $K=k_1+k_2+k_3$, the needed regulated integral is

$$
\int_{-\infty(1-i\epsilon)}^0
(1-iq_i\tau)e^{ic_sK\tau}\,d\tau
=-\frac{i}{c_s}\left(\frac1K+\frac{k_i}{K^2}\right).
$$

There are three choices for the undifferentiated leg and two contractions interchanging the differentiated legs. The stated [in-in formalism](../../../../../../keldysh-formalism.md) formula therefore gives

$$
\langle\varphi_{\mathbf k_1}\varphi_{\mathbf k_2}\varphi_{\mathbf k_3}\rangle
=(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)
B_\lambda(k_1,k_2,k_3),
$$

with

$$
\boxed{
B_\lambda
=\frac{\lambda_0H^4}{2(k_1k_2k_3)^3}
\sum_{\mathrm{cyc}}
k_j^2k_l^2
\left(\frac1K+\frac{k_i}{K^2}\right)}.
$$

The powers of $c_s$ cancel for this vertex with the normalization specified in part (i). Reversing the convention for the sign of $H_I$ reverses the displayed overall sign but not the momentum shape of the [primordial bispectrum](../../../../../../primordial-bispectrum.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
