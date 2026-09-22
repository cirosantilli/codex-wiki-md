<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In a [two-dimensional conformal field theory](../../../../../two-dimensional-conformal-field-theory.md), a [quasi-primary operator](../../../../../quasi-primary-operator.md) of [conformal weights](../../../../../conformal-weight.md) $(h,\widetilde h)$ obeys

$$
\mathcal O'(z',\bar z')=\left(\frac{dz'}{dz}\right)^{-h}\left(\frac{d\bar z'}{d\bar z}\right)^{-\widetilde h}\mathcal O(z,\bar z)
$$

for global conformal, or Möbius, transformations. A [primary operator](../../../../../primary-field.md) obeys this law for every locally invertible holomorphic and antiholomorphic conformal coordinate change. Quasi-primary is therefore weaker: the stress tensor at nonzero [central charge](../../../../../central-charge.md) is quasi-primary, but its Schwarzian transformation term prevents it from being primary under a general map.

A [primary state](../../../../../primary-state.md) is a simultaneous eigenstate of $L_0,\widetilde L_0$ with eigenvalues $h,\widetilde h$, satisfying

$$
\boxed{L_n|\mathcal O\rangle=\widetilde L_n|\mathcal O\rangle=0\qquad(n>0).}
$$

A quasi-primary state need only satisfy the corresponding $n=1$ conditions. Negative modes of the [Virasoro algebra](../../../../../virasoro-algebra.md) generate descendants.

In [radial quantization](../../../../../radial-quantization.md), a local operator at the origin prepares a state on a surrounding circle; logarithmic radius is Euclidean time. The [state–operator correspondence](../../../../../state-operator-correspondence.md) is $|\mathcal O\rangle=\mathcal O(0)|0\rangle$. Acting with a [Virasoro generator](../../../../../virasoro-generator.md) means inserting its stress-tensor contour around that operator. For a [primary operator](../../../../../primary-field.md), the [operator product expansion](../../../../../operator-product-expansion.md) is

$$
T(z)\mathcal O(0)\sim\frac{h\mathcal O(0)}{z^2}+\frac{\partial\mathcal O(0)}{z}.
$$

Multiplication by $z^{n+1}$ and the contour residue give $L_0|\mathcal O\rangle=h|\mathcal O\rangle$, $L_{-1}|\mathcal O\rangle=|\partial\mathcal O\rangle$, and $L_n|\mathcal O\rangle=0$ for $n>0$. Conversely the contour modes are the coefficients of the singular expansion; vanishing positive modes removes every pole of order three and higher. The remaining double and simple poles generate precisely the primary transformation law. The antiholomorphic argument is identical. This proves the [state-operator correspondence for Virasoro primaries](../../../../../state-operator-correspondence-for-virasoro-primaries.md) in both directions.

An [integrated string vertex operator](../../../../../integrated-string-vertex-operator.md) is integrated with $d^2z$. The measure transforms with weights $(-1,-1)$, so conformal invariance requires its matter operator to have weights $(1,1)$. In [old covariant string quantization](../../../../../old-covariant-string-quantization.md) the same requirement is $L_{n>0}=\widetilde L_{n>0}=0$ and $L_0=\widetilde L_0=1$. The ghost-dressed unintegrated vertex $c\bar c\,V$ has total weights $(0,0)$. Physical states are identified modulo [null string states](../../../../../null-string-state.md), or more systematically by [BRST cohomology](../../../../../brst-cohomology.md); raw counting of all [primary operators](../../../../../primary-field.md) includes gauge redundancy.

For a free embedding boson the holomorphic stress tensor is $T=-:\partial X\cdot\partial X:/\alpha'$. Contracting it with $:e^{ik\cdot X}:$ gives weight $\alpha'k^2/4$; every holomorphic oscillator of level $r$ adds $r$ to that weight. Thus

$$
h=N+\frac{\alpha'k^2}{4},\qquad\widetilde h=\widetilde N+\frac{\alpha'k^2}{4}.
$$

With Lorentzian target signature, $M^2=-k^2$, so the [closed-bosonic-string mass shell from primary weights](../../../../../closed-bosonic-string-mass-shell-from-primary-weights.md) is

$$
\boxed{N=\widetilde N,\qquad M^2=\frac4{\alpha'}(N-1).}
$$

The ground state is tachyonic, level one is massless, and higher levels are massive. The primary conditions also constrain the polarization tensors; the two zero-mode conditions fix the mass and level matching.

For the commuting [beta-gamma system](../../../../../beta-gamma-system.md), write $r=z-w$. The displayed exchange leaves the arguments attached to their respective fields. Exchanging the arguments instead gives

$$
\beta(z)\gamma(w)\sim-\frac1r,\qquad\gamma(z)\beta(w)\sim+\frac1r.
$$

This [radial-ordering sign in commuting beta-gamma contractions](../../../../../radial-ordering-sign-in-commuting-beta-gamma-contractions.md) must be kept when differentiating. Expanding the total derivative in the proposed stress tensor gives

$$
T=(1-\lambda):\partial\beta\,\gamma:-\lambda:\beta\,\partial\gamma:.
$$

The contraction $\gamma(z)\beta(w)\sim1/r$ and its derivative $\partial\gamma(z)\beta(w)\sim-1/r^2$ give

$$
T(z)\beta(w)\sim(1-\lambda)\frac{\partial\beta(z)}r+\lambda\frac{\beta(z)}{r^2}
=\frac{\lambda\beta(w)}{r^2}+\frac{\partial\beta(w)}r.
$$

Similarly $\partial\beta(z)\gamma(w)\sim1/r^2$ and $\beta(z)\gamma(w)\sim-1/r$ give

$$
T(z)\gamma(w)\sim(1-\lambda)\frac{\gamma(z)}{r^2}+\lambda\frac{\partial\gamma(z)}r
=\frac{(1-\lambda)\gamma(w)}{r^2}+\frac{\partial\gamma(w)}r.
$$

There are no higher poles. Both fields are holomorphic and $\bar T=0$, so

$$
\boxed{(h_\beta,\widetilde h_\beta)=(\lambda,0),\qquad(h_\gamma,\widetilde h_\gamma)=(1-\lambda,0).}
$$

To compute the [central charge](../../../../../central-charge.md), put $A=:\partial\beta\,\gamma:$ and $B=:\beta\,\partial\gamma:$. Only double [Wick contractions](../../../../../wick-contraction.md) can give the fourth-order pole in $TT$. Their coefficients are

$$
A(z)A(w)\sim\frac1{r^4},\qquad B(z)B(w)\sim\frac1{r^4},\qquad
A(z)B(w)\sim\frac2{r^4},\qquad B(z)A(w)\sim\frac2{r^4},
$$

where only the double-contraction terms are shown. For example, the mixed contraction uses $\partial\beta(z)\partial\gamma(w)\sim2/r^3$ and $\gamma(z)\beta(w)\sim1/r$. All Wick pairings have bosonic signs. Therefore the fourth-order coefficient is

$$
(1-\lambda)^2+\lambda^2-4\lambda(1-\lambda)=6\lambda^2-6\lambda+1.
$$

The stress-tensor [operator product expansion](../../../../../operator-product-expansion.md) has fourth-order coefficient $c/2$, yielding

$$
\boxed{c=12\lambda^2-12\lambda+2,\qquad\bar c=0.}
$$

This is the [stress tensor of a commuting beta-gamma system](../../../../../stress-tensor-of-a-commuting-beta-gamma-system.md) calculation. Single contractions supply the usual $2T/r^2+\partial T/r$ terms, with the potential third-order terms canceling.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
