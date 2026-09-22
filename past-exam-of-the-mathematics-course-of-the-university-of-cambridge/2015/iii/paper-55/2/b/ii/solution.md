<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use exactly the stipulated unit-sound-speed mode functions for this integral. Their late-time values are real and $u_k'{}^*(\tau)=Hk^2\tau e^{ik\tau}/\sqrt{4\epsilon k^3}$. Consequently

$$
\prod_i u_{k_i}(0)u_{k_i}'{}^*(\tau)
=\frac{H^6}{64\epsilon^3k_1k_2k_3}\tau^3e^{iK\tau},\qquad K=k_1+k_2+k_3>0.
$$

The vacuum contour lies above the negative real time axis, so $e^{iK\tau}$ decays at its past endpoint. With $s=iK+0^+$, repeated differentiation of $\int_{-\infty}^0e^{s\tau}d\tau=1/s$ gives

$$
\boxed{\int_{-\infty(1-i0)}^0\tau^2e^{iK\tau}d\tau=\frac{2}{(iK)^3}=\frac{2i}{K^3}.}
$$

Substitution gives **the bispectrum with consistent operator ordering and the stated Hamiltonian**:

$$
\boxed{B_\zeta(k_1,k_2,k_3)=\frac{3H^4}{8\epsilon^2}\frac{\mathcal F}{k_1k_2k_3K^3},}
$$



$$
\boxed{\langle\zeta_{\mathbf k_1}\zeta_{\mathbf k_2}\zeta_{\mathbf k_3}\rangle_c
=\frac{+3H^4\pi^3}{\epsilon^2}\frac{1-c_s^2}{c_s^2}\mathcal A
\frac{\delta^{(3)}(\sum_i\mathbf k_i)}{k_1k_2k_3K^3}.}
$$

The sign is positive in front of $\mathcal A$, contrary to the target's negative sign. The printed negative result is obtained algebraically if one uses the unstarred derivatives, $e^{-iK\tau}$, and the conjugate past contour, which gives $-2i/K^3$, while retaining $-2i$ outside. That combination is not the stated vacuum contour or the stated external-before-vertex contraction. A consistently conjugated representation must also conjugate the external prefactor and has the positive result above. The [unit-speed cubic time-derivative bispectrum](../../../../../../../unit-speed-cubic-time-derivative-bispectrum.md) records these conventions explicitly.

The approximation treats $H$, $\epsilon$ and the interaction coefficients as constant, uses the [de Sitter approximation](../../../../../../../de-sitter-approximation.md), retains only the stipulated vertex at tree level, and takes $k_i|\tau_{\rm final}|\to0$ after doing the convergent early-time integral. The $i0$ prescription must be kept while imposing the past boundary condition; an arbitrary early-time cutoff leaves spurious oscillatory boundary terms. For a physical noncanonical quadratic action with $c_s\ne1$, the mode functions also change to $H(1+ic_sk\tau)e^{-ic_sk\tau}/\sqrt{4\epsilon c_sk^3}$. They were not supplied here; the displayed calculation is conditional on the paper's specified modes, rather than a full self-consistent noncanonical power-spectrum calculation.

With the stipulated power spectrum $P_\zeta(k)=H^2/(4\epsilon k^3)$, an [equilateral bispectrum configuration](../../../../../../../equilateral-bispectrum-configuration.md) gives $B(k,k,k)/P(k)^2=2\mathcal F/9$. For the local-style normalization evaluated only at that triangle, $B(k,k,k)=(18/5)f_{\rm NL}^{\rm effective}P(k)^2$, this means

$$
\boxed{f_{\rm NL}^{\rm effective}(k,k,k)=\frac5{81}\mathcal F.}
$$

This is a normalization convention for an equilateral amplitude, not a claim that the shape is local. In a [squeezed bispectrum configuration](../../../../../../../squeezed-bispectrum-configuration.md), the ratio to the long-short power product is suppressed by $(k_L/k_S)^2$. Small sound speed or large higher-kinetic derivatives can make $|\mathcal F|$ large enough for potentially observable [primordial non-Gaussianity](../../../../../../../primordial-non-gaussianity.md), whereas $c_s\to1$ with finite $\mathcal A$ suppresses this vertex. Detectability is conditional on amplitudes, the other cubic interactions, and perturbative control; it cannot be asserted from the given constants alone.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
