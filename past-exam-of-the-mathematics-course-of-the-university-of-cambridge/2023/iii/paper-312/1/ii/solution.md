<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The first-order [in-in formalism](../../../../../../keldysh-formalism.md) formula at observation time $\tau_0$ is

$$
\langle O(\tau_0)\rangle_{\lambda}
=i\int_{-\infty(1-i\epsilon)}^{\tau_0}d\tau\,
\langle[H_{\rm int}(\tau),O_I(\tau_0)]\rangle.
$$

Fourier transforming the three derivatives gives

$$
H_{\rm int}(\tau)
=-i\lambda a^4
\int_{\mathbf p_1\cdots\mathbf p_4}
(2\pi)^3\delta^{(3)}(\mathbf p_1+\cdots+\mathbf p_4)
\,[\mathbf p_2\mathbin\cdot(\mathbf p_3\mathbin\times\mathbf p_4)]
\prod_{a=1}^4\phi_a(\mathbf p_a,\tau),
$$

where $\int_{\mathbf p}=\int d^3p/(2\pi)^3$. Because the four species are distinct, [Wick contraction](../../../../../../wick-contraction.md) pairs each vertex field with the external field of the same species and introduces no permutation factor. If

$$
\mathcal E=\mathbf k_2\mathbin\cdot(\mathbf k_3\mathbin\times\mathbf k_4),
\qquad k_T=k_1+k_2+k_3+k_4,
$$

then

$$
\langle H_{\rm int}(\tau)O(\tau_0)\rangle
=i\lambda a^4(\tau)(2\pi)^3\delta^{(3)}\!\left(\sum_a\mathbf k_a\right)
\mathcal E\prod_{a=1}^4f(k_a,\tau)f^*(k_a,\tau_0).
$$

Combining this with part i gives the requested [time integral](../../../../../../time-integral.md):

$$
\boxed{
\langle O(\tau_0)\rangle_{\lambda}
=2i\lambda(2\pi)^3\delta^{(3)}\!\left(\sum_a\mathbf k_a\right)\mathcal E
\int_{-\infty(1-i\epsilon)}^{\tau_0}d\tau\,a^4(\tau)
\operatorname{Re}\left[i\prod_{a=1}^4f(k_a,\tau)f^*(k_a,\tau_0)\right]}.
$$

The factor $\mathcal E$ is a [pseudoscalar](../../../../../../pseudoscalar.md), so the resulting [primordial trispectrum](../../../../../../primordial-trispectrum.md) is parity odd and purely imaginary in this momentum-space convention.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
