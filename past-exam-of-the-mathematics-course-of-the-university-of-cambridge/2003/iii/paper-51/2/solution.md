<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [stress-energy tensor](../../../../../stress-energy-tensor.md) generates [translations](../../../../../translation-geometry.md). One may improve it by adding a [divergence](../../../../../divergence.md) without changing the [translation](../../../../../translation-geometry.md) charges under suitable [boundary conditions](../../../../../boundary-condition.md), and choose it symmetric in a relativistic theory. If $\Theta^{\mu\nu}$ is symmetric and conserved, a spacetime vector field $\omega$ defines the current $j^\mu=\Theta^{\mu\nu}\omega_\nu$. For a [Conformal Killing vector field](../../../../../conformal-killing-vector-field.md),

$$
\partial_\mu j^\mu=\Theta^{\mu\nu}\partial_\mu\omega_\nu
=\frac{\partial\cdot\omega}{d}\Theta^\mu{}_{\mu}.
$$

Thus a traceless conserved [stress-energy tensor](../../../../../stress-energy-tensor.md) produces all the conformal charges. The [dilation](../../../../../uniform-dilation.md) current is $x_\nu\Theta^{\mu\nu}$, and the special [conformal currents](../../../../../conformal-current.md) are $(2x_\lambda x_\nu-x^2\eta_{\lambda\nu})\Theta^{\mu\nu}$. A [trace](../../../../../matrix-trace.md) that is merely the [divergence](../../../../../divergence.md) of a [virial current](../../../../../virial-current.md) gives [scale invariance](../../../../../scale-invariance.md); conformal invariance requires the additional improvement that removes the [trace](../../../../../matrix-trace.md). These statements distinguish an actual traceless tensor from a [trace](../../../../../matrix-trace.md) discarded without justification.

For a free massless [scalar field](../../../../../scalar-field.md), the [canonical stress-energy tensor](../../../../../canonical-stress-energy-tensor.md) has [trace](../../../../../matrix-trace.md) $(1-d/2)(\partial\phi)^2$. For $d>1$, the [improved stress-energy tensor of a free massless scalar](../../../../../improved-stress-energy-tensor-of-a-free-massless-scalar.md) is

$$
\Theta_{\mu\nu}=\partial_\mu\phi\partial_\nu\phi-\frac12\eta_{\mu\nu}(\partial\phi)^2
+\frac{d-2}{4(d-1)}(\eta_{\mu\nu}\Box-\partial_\mu\partial_\nu)\phi^2.
$$

Its improvement is identically conserved. On $\Box\phi=0$, the identity $\Box\phi^2=2(\partial\phi)^2$ shows that its [trace](../../../../../matrix-trace.md) vanishes. In $d=2$, no improvement is needed: the [canonical stress-energy tensor](../../../../../canonical-stress-energy-tensor.md) is already traceless. In Lorentzian null coordinates, conservation and tracelessness imply that its two surviving components depend separately on $x^+$ and $x^-$. After Euclidean continuation, these become the [holomorphic stress-energy tensor](../../../../../holomorphic-stress-energy-tensor.md) $T(z)$ and its antiholomorphic counterpart $\bar T(\bar z)$, with

$$
\bar\partial T=0,\qquad \partial\bar T=0.
$$

Local conformal changes are arbitrary holomorphic and antiholomorphic coordinate changes, not just the three global [Möbius transformation](../../../../../mobius-transformation.md) generators in either sector.

To make the free-field quantum normalization explicit, rescale the field to $\varphi=\sqrt{4\pi}\phi$, so that its plane contraction is $\varphi(z,\bar z)\varphi(w,\bar w)\sim-\log|z-w|^2$. Define $J=i\partial\varphi$, so $J(z)J(w)\sim(z-w)^{-2}$. [Normal ordering](../../../../../normal-ordering.md) gives

$$
T(z)=\frac12:J(z)^2:=-\frac12:(\partial\varphi)^2:.
$$

A single [Wick contraction](../../../../../wick-contraction.md) shows that $J$ is a weight-one [primary operator](../../../../../primary-field.md). The two double contractions in $T(z)T(w)$ produce $\frac12(z-w)^{-4}$; single contractions, followed by Taylor expansion at $w$, produce $2T(w)/(z-w)^2+\partial T(w)/(z-w)$. Thus the [operator product expansion](../../../../../operator-product-expansion.md) is

$$
\boxed{T(z)T(w)\sim\frac{1/2}{(z-w)^4}+\frac{2T(w)}{(z-w)^2}+\frac{\partial T(w)}{z-w}},\qquad \boxed{c=1}.
$$

The same holds independently for $\bar T$, with $\bar c=1$. The undifferentiated noncompact scalar has a logarithmic contraction and a zero-mode subtlety; its derivative current has the ordinary primary transformation law.

The [holomorphic stress-energy tensor](../../../../../holomorphic-stress-energy-tensor.md) implements infinitesimal [conformal transformations](../../../../../conformal-map.md) through contour charges $Q_v=\frac1{2\pi i}\oint dz\,v(z)T(z)$. A primary field $\mathcal O$ of weight $h$ obeys

$$
T(z)\mathcal O(w)\sim\frac{h\mathcal O(w)}{(z-w)^2}+\frac{\partial\mathcal O(w)}{z-w},\qquad
[Q_v,\mathcal O]=(v\partial+h v')\mathcal O.
$$

For example the free-field vertex operator $:\!e^{i\alpha\varphi}\!:$ has holomorphic weight $h=\alpha^2/2$, as follows by contracting $\partial\varphi$ with the exponential twice. In correlators the contour may encircle each insertion, giving the conformal [Ward identity](../../../../../ward-identity.md) $\langle T(z)\prod_i\mathcal O_i(z_i)\rangle=\sum_i[h_i/(z-z_i)^2+\partial_{z_i}/(z-z_i)]\langle\prod_i\mathcal O_i(z_i)\rangle$. This also yields the [global conformal Ward identities for chiral correlators](../../../../../global-conformal-ward-identities-for-chiral-correlators.md).

Writing $T(z)=\sum_nL_nz^{-n-2}$ and integrating the stress-tensor [operator product expansion](../../../../../operator-product-expansion.md) gives the [Virasoro algebra](../../../../../virasoro-algebra.md)

$$
\boxed{[L_m,L_n]=(m-n)L_{m+n}+\frac{c}{12}(m^3-m)\delta_{m+n,0}}.
$$

Its [central charge](../../../../../central-charge.md) is the quantum correction to the classical conformal algebra; the correction vanishes on $L_{-1},L_0,L_1$. Equivalently, in the pullback convention a finite holomorphic change $z\mapsto f(z)$ sends $T$ to $(f')^2T(f)+\frac c{12}\{f,z\}$, where $\{f,z\}=f'''/f'-\frac32(f''/f')^2$ is the [Schwarzian derivative](../../../../../schwarzian-derivative.md). This anomalous term vanishes for [Möbius transformations](../../../../../mobius-transformation.md). On a curved background the related [trace](../../../../../matrix-trace.md) anomaly is proportional to its curvature; it does not destroy the flat-space conformal symmetry of this massless theory.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
