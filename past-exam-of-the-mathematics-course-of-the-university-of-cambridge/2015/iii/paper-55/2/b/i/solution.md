<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a centred [Gaussian random field](../../../../../../../gaussian-random-field.md), [Wick theorem](../../../../../../../wick-s-theorem.md) expresses each even correlation function as a sum over all pairings of two-point functions; odd moments vanish. For example,

$$
\langle ABCD\rangle=\langle AB\rangle\langle CD\rangle+\langle AC\rangle\langle BD\rangle+\langle AD\rangle\langle BC\rangle.
$$

For six fields there are $5\cdot3\cdot1=15$ pairings. In a tree-level connected three-point calculation with one cubic vertex, each of the three external fields must contract with a different vertex field. This gives $3!=6$ connected [Wick contractions](../../../../../../../wick-contraction.md). Pairings connecting two external fields instead are disconnected tadpole contributions, omitted from the [primordial bispectrum](../../../../../../../primordial-bispectrum.md).

Put $\mathcal F=(1-c_s^2)\mathcal A/c_s^2$. Using $dt=a\,d\tau$ and $\dot\zeta=\zeta'/a$, the integrated [interaction Hamiltonian](../../../../../../../interaction-hamiltonian.md) becomes

$$
\int dt\,H_{\rm int}(t)=-\int d\tau\,d^3x\,\frac{a\epsilon\mathcal F}{H}\zeta'^3
=\int d\tau\,d^3x\,\frac{\epsilon\mathcal F}{H^2\tau}\zeta'^3.
$$

The unequal-time [Wick contraction](../../../../../../../wick-contraction.md) required by the displayed operator order is

$$
\boxed{\langle\zeta(\mathbf k,0)\zeta'(\mathbf p,\tau)\rangle
=(2\pi)^3\delta^{(3)}(\mathbf k+\mathbf p)\,u_k(0)u_p'{}^*(\tau).}
$$

The conjugate is essential: the equal-time power spectrum alone does not specify the erroneous unstarred replacement printed in the target expression. The [in-in bispectrum conjugation rule](../../../../../../../in-in-bispectrum-conjugation-rule.md) fixes the vacuum convergence and final sign.

Fourier transforming the vertex gives $(2\pi)^3\delta^{(3)}(\mathbf p_1+\mathbf p_2+\mathbf p_3)$ with three measures $d^3p_j/(2\pi)^3$. The six pairings supply the product of three external-vertex delta functions, each carrying $(2\pi)^3$. Integrating all three internal momenta leaves one overall $(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)$. Thus **the normalized connected contraction formula is**

$$
\boxed{\langle\zeta_{\mathbf k_1}\zeta_{\mathbf k_2}\zeta_{\mathbf k_3}\rangle_c
=(2\pi)^3\delta^{(3)}\!\left(\sum_i\mathbf k_i\right)
\operatorname{Re}\left[-12i\frac{\epsilon\mathcal F}{H^2}
\prod_i u_{k_i}(0)\int_{-\infty(1-i0)}^0\frac{d\tau}{\tau}\prod_i u_{k_i}'{}^*(\tau)\right].}
$$

This spells out what the printed permutations and delta functions must represent: all six permutations, full Fourier normalization, and conjugated vertex modes. Three cyclic permutations alone would miss a factor of two.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 55](../../../../paper-55-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
