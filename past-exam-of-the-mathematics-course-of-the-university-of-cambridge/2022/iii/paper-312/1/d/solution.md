<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In conformal time the interaction Hamiltonian is

$$
H_I(\eta)=-\frac{\lambda}{4!}\int d^3x\,a^4(\eta)\varphi^4(\eta,\mathbf x).
$$

The first-order [in-in formalism](../../../../../../keldysh-formalism.md) formula and [Wick theorem](../../../../../../wick-s-theorem.md) give the connected [primordial trispectrum](../../../../../../primordial-trispectrum.md)

$$
\begin{aligned}
\langle\varphi_{\mathbf k_1}\varphi_{\mathbf k_2}
\varphi_{\mathbf k_3}\varphi_{\mathbf k_4}\rangle_c
={}&2\lambda(2\pi)^3\delta^{(3)}\!\left(\sum_a\mathbf k_a\right)\\
&\times\operatorname{Im}\left[
\prod_{a=1}^4f_{k_a}^*(\tau)
\int_{-\infty(1-i\epsilon)}^\tau d\eta\,
a^4(\eta)\prod_{a=1}^4f_{k_a}(\eta)
\right].
\end{aligned}
$$

The factor $4!$ from the [Wick contractions](../../../../../../wick-contraction.md) cancels the vertex factor. Writing $K=k_1+k_2+k_3+k_4$, the powers of $\eta$ cancel because $a^4\prod_af_{k_a}$ is constant apart from its phase, and the [i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md) gives

$$
\int_{-\infty(1-i\epsilon)}^\tau e^{-icK\eta}\,d\eta
=\frac{i}{cK}e^{-icK\tau}.
$$

Consequently

$$
\boxed{
\langle\varphi_{\mathbf k_1}\varphi_{\mathbf k_2}
\varphi_{\mathbf k_3}\varphi_{\mathbf k_4}\rangle_c
=(2\pi)^3\delta^{(3)}\!\left(\sum_a\mathbf k_a\right)
\frac{\lambda H^4\tau^4}{8c^5K\,k_1k_2k_3k_4}}.
$$

The full four-point function also contains the three disconnected products of the free two-point function found in part c.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
