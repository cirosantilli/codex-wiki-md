<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [Gaussian critical exponents](../../../../../gaussian-critical-exponent.md), use dimensionless statistical-action conventions, with the [Boltzmann factor](../../../../../boltzmann-factor.md) $e^{-H}$. If $H$ is an energy, apply the following to $H/(k_BT)$ and absorb that smooth factor into the couplings. Choose the [Fourier transform](../../../../../fourier-transform.md) convention

$$
\phi(x)=\int_p e^{ip\cdot x}\widetilde\phi(p),\qquad
\int_p=\int_{|p|<\Lambda}\frac{d^Dp}{(2\pi)^D},\qquad\Lambda\sim a^{-1}.
$$

Reality gives $\widetilde\phi(-p)=\widetilde\phi(p)^*$. The Fourier-space [statistical Hamiltonian](../../../../../statistical-hamiltonian.md) is

$$
\boxed{H=\frac12\int_p(\kappa^{-1}p^2+m^2)
\widetilde\phi(p)\widetilde\phi(-p)
-\int_p\widetilde J(-p)\widetilde\phi(p).}
$$

The source term is not multiplied by one half. Completing the [Gaussian functional integral](../../../../../gaussian-functional-integral.md) gives $\langle\widetilde\phi(p)\rangle=\widetilde J(p)/(\kappa^{-1}p^2+m^2)$ and the connected Fourier-space [two-point correlation function](../../../../../two-point-correlation-function.md)

$$
\widetilde G(p)=\frac1{\kappa^{-1}p^2+m^2}
=\frac\kappa{p^2+\kappa m^2}.
$$

Assume $m^2>0$ for the stable massive [Gaussian field theory](../../../../../gaussian-field-theory.md). In the continuum long-distance theory, the real-space [correlation function](../../../../../correlation-function.md) is the Green kernel of $-\kappa^{-1}\nabla^2+m^2$. Away from its source, a radial ansatz $G(R)\sim R^{-(D-1)/2}e^{-R/\xi}$ gives, at large $R$, $m^2-\kappa^{-1}\xi^{-2}=0$. Equivalently the propagator pole is at $p^2=-\kappa m^2$. Thus **the exponential [correlation length](../../../../../correlation-length.md) is**

$$
\boxed{\xi=\frac1{m\sqrt\kappa}.}
$$

At $m=0$ the [correlation length](../../../../../correlation-length.md) diverges. A sharp momentum regulator itself introduces artificial oscillatory long-distance tails; this length describes the physical continuum pole or a local/smoothly regulated model on distances large compared with $a$.

For a [momentum-shell renormalization group](../../../../../momentum-shell-renormalization-group.md) step with $b>1$, split the [Fourier modes](../../../../../fourier-mode.md) into retained modes $|p|<\Lambda/b$ and eliminated modes $\Lambda/b<|p|<\Lambda$. Define $\widetilde\phi_B(p)$ as the retained field. Integrating the eliminated modes is exact for a [Gaussian field theory](../../../../../gaussian-field-theory.md); a uniform source acts only on the zero mode, so this integration produces a field-independent free-energy term. Rescale $q=bp$ and set $\widetilde\phi_B(p)=\widetilde Z\widetilde\phi'(q)$. The retained quadratic action becomes

$$
\frac12b^{-D}\widetilde Z^2\int_q
(\kappa^{-1}b^{-2}q^2+m^2)\widetilde\phi'(q)\widetilde\phi'(-q).
$$

Keeping the gradient coefficient fixed requires $b^{-D-2}\widetilde Z^2=1$. For $J=h$, the source term is $-h\widetilde\phi_B(0)$, so **the complete Gaussian rescaling is**

$$
\boxed{\widetilde Z=b^{(D+2)/2},\qquad
\kappa'^{-1}=\kappa^{-1},\qquad m'=bm,\qquad
h'=b^{(D+2)/2}h.}
$$

The corresponding real-space field obeys $\phi_B(x)=b^{(2-D)/2}\phi'(x/b)$; confusing that real-space factor with $\widetilde Z$ would change the source exponent incorrectly.

Let $F$ be [free energy](../../../../../thermodynamic-free-energy.md) per original volume, with $t$ proportional to $m^2$. Rescaled volume is $V'=V/b^D$, so the [Gaussian free-energy scaling relation](../../../../../gaussian-free-energy-scaling-relation.md) is

$$
\boxed{F(t,h)=F_{\mathrm{shell}}(t)+b^{-D}F(b^2t,b^{(D+2)/2}h).}
$$

A field-normalisation Jacobian can be included in the field-independent shell term. For any finite step on positive-mass modes, that background is analytic near $t=0$. Subtract regular backgrounds and choose $b=t^{-1/2}$ on the massive side. The usual homogeneous singular scaling then gives

$$
\boxed{F_S(t,h)=t^{D/2}f\!\left(\frac h{t^{(D+2)/4}}\right),\qquad
\alpha=2-\frac D2,\qquad\Delta=\frac{D+2}{4}.}
$$

These are [Gaussian critical exponents](../../../../../gaussian-critical-exponent.md) for the stipulated Gaussian approximation. A useful check is its source-dependent contribution $-h^2/(2m^2)$: $D/2-2\Delta=-1$ gives precisely that power of $t$.

There is a qualification to a strictly pure-power singular [free energy](../../../../../thermodynamic-free-energy.md). The [Gaussian free-energy logarithm at effective dimension two](../../../../../gaussian-free-energy-logarithm-at-effective-dimension-two.md) in $D=2$ contains $t\log t$ after subtracting analytic terms. Thus the displayed exponent assignments remain the formal power indices, but at $D=2$ the advertised homogeneous expression needs this additive logarithmic term. A purely quadratic theory also cannot stabilise the ordered $t<0$ phase or the zero-mass zero mode at nonzero $h$; the scaling calculation is taken from $t>0$, and an ordered-phase continuation requires stabilising interactions.

At a uniaxial [Lifshitz point](../../../../../lifshitz-point.md), the quadratic kernel instead is

$$
K(p)=\kappa^{-1}p_\perp^2+\mu^{-1}p_\parallel^4+m^2,
\qquad\kappa,\mu>0.
$$

The vanishing coefficient of $p_\parallel^2$ is an additional tuning that distinguishes this [Lifshitz point](../../../../../lifshitz-point.md) from an ordinary critical point. Use a factorised cutoff, retain $|p_\perp|<\Lambda_\perp/b$ and $|p_\parallel|<\Lambda_\parallel/c$, and integrate its complement. A rectangular or cylindrical retained region is suitable; its precise boundary is not an exponent. This is a [uniaxial Lifshitz Gaussian renormalization](../../../../../uniaxial-lifshitz-gaussian-renormalization.md) step.

Set $q_\perp=bp_\perp$, $q_\parallel=cp_\parallel$, and $\widetilde\phi_B=\widetilde Z\widetilde\phi'$. The momentum measure acquires $b^{-(D-1)}c^{-1}$. Keeping both kinetic coefficients fixed requires

$$
b^{-(D-1)}c^{-1}\widetilde Z^2b^{-2}=1,
\qquad
b^{-(D-1)}c^{-1}\widetilde Z^2c^{-4}=1.
$$

Therefore **the anisotropic blocking and source factors are**

$$
\boxed{c=b^{1/2},\qquad
\widetilde Z=b^{(2D+3)/4},\qquad
m'=bm,\qquad h'=b^{(2D+3)/4}h.}
$$

The [anisotropic effective dimension](../../../../../anisotropic-effective-dimension.md) is $d_{\mathrm{eff}}=D-1+1/2=D-1/2$: one parallel coordinate contributes half the scaling weight of a perpendicular coordinate. The rescaled-volume factor is $b^{-d_{\mathrm{eff}}}$, so

$$
F(t,h)=F_{\mathrm{shell}}(t)+b^{-(D-1/2)}F(b^2t,b^{(2D+3)/4}h).
$$

Choosing $b=t^{-1/2}$ gives **the requested Lifshitz Gaussian exponents**:

$$
\boxed{\alpha=2-\frac{D-1/2}{2}=\frac94-\frac D2,
\qquad \Delta=\frac{2D+3}{8}.}
$$

Again $(D-1/2)/2-2\Delta=-1$, checking the uniform-source susceptibility. The associated length powers are $\xi_\perp\sim t^{-1/2}$ and $\xi_\parallel\sim t^{-1/4}$. A Gaussian determinant has the analogous logarithmic exception if its effective dimension equals 2. Interactions can alter these exponents; dimensional rescaling here solves the specified Gaussian model.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
