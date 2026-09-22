<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Landau-Ginzburg theory](../../../../../../landau-ginzburg-theory.md) for a scalar [order parameter](../../../../../../order-parameter.md) supplements a local symmetry-allowed potential with a [gradient](../../../../../../gradient.md) penalty. For a $\mathbb Z_2$ [symmetry](../../../../../../symmetry-physics.md) at zero field, a stable quartic model is

$$
F[\phi]=\int d^Dx\left[\frac K2|\nabla\phi|^2+\frac r2\phi^2+\frac u4\phi^4-h\phi\right],\qquad K,u>0,
$$

with $r=a(T-T_c)$ near a mean-field transition. Equilibrium fluctuations have weight $e^{-F/(k_BT)}$. In the [Landau approximation](../../../../../../landau-approximation.md), minimize the functional. A uniform stationary state obeys $r\phi+u\phi^3=h$. At zero field the minimum is $\phi=0$ for $r>0$ and $\phi=\pm\sqrt{-r/u}$ for $r<0$. The latter pair is [spontaneous symmetry breaking](../../../../../../spontaneous-symmetry-breaking.md) of the [discrete symmetry](../../../../../../discrete-symmetry.md).

The uniform [free-energy density](../../../../../../free-energy-density.md) at its minimum is zero above the transition and $-r^2/(4u)$ below, up to regular backgrounds. Differentiating the equation of state gives $\chi_+=1/r$ and $\chi_-=1/(2|r|)$. At $r=0$, $\phi=(h/u)^{1/3}$. Gaussian fluctuations around the minimum have inverse [covariance](../../../../../../covariance.md) $(Kq^2+r)/(k_BT)$ above and $(Kq^2+2|r|)/(k_BT)$ below. Their [correlation lengths](../../../../../../correlation-length.md) are $\xi_+=(K/r)^{1/2}$ and $\xi_-=(K/(2|r|))^{1/2}$. These results give the usual [mean-field critical exponents](../../../../../../mean-field-critical-exponent.md)

$$
\boxed{\alpha=0,\quad\beta_{\rm mag}=1/2,\quad\gamma=1,\quad\delta=3,\quad\nu=1/2,\quad\eta=0.}
$$

The [heat capacity](../../../../../../heat-capacity.md) has a finite jump rather than a power-law divergence. Negative quartic coefficient requires higher stabilizing terms and can produce a first-order transition; a vanishing quartic coefficient requires a tricritical analysis. Thus the assumed positivity of $u$ matters.

The [Ginzburg criterion](../../../../../../ginzburg-criterion.md) tests whether this saddle description is self-consistent. Below the transition compare fluctuations of the [order parameter](../../../../../../order-parameter.md) averaged over a [correlation volume](../../../../../../correlation-volume.md) with its squared mean-field value $\phi_0^2=|r|/u$. Modes with $q\lesssim\xi^{-1}$ dominate this coarse-grained fluctuation estimate:

$$
\langle(\delta\phi)^2\rangle_\xi\simeq k_BT\int_{q\lesssim\xi^{-1}}\frac{d^Dq}{(2\pi)^D}\frac1{Kq^2+2|r|}
=A_D\frac{k_BT}{K^{D/2}}|r|^{D/2-1},
$$

where the positive dimensionless $A_D$ depends on the averaging window and the factor of two used in $\xi$. Dividing by $\phi_0^2$ gives

$$
\boxed{\mathcal G(r)=A_D\frac{k_BT\,u}{K^{D/2}}|r|^{(D-4)/2}\ll1.}
$$

It is the fluctuation of a correlation-volume average, not the full cutoff-dominated microscopic [variance](../../../../../../variance-split.md), that should be compared with the mean-field [order parameter](../../../../../../order-parameter.md).

For $D<4$, $\mathcal G$ diverges as $r\to0$, so the asymptotic critical region is fluctuation dominated. Away from it, [mean-field theory](../../../../../../mean-field-theory.md) can still work when

$$
|r|\gg\left(A_Dk_BT\,u/K^{D/2}\right)^{2/(4-D)}.
$$

For $D>4$, the long-wavelength ratio tends to zero near criticality, consistently with Gaussian control and mean-field thermodynamic exponents. At $D=4$, quartic coupling is marginal; scale-dependent logarithms require a renormalization-group analysis rather than interpreting a constant bare ratio as a proof of no corrections. This identifies four as the [upper critical dimension](../../../../../../upper-critical-dimension.md) of the short-range scalar quartic model.

The [Landau-Ginzburg theory](../../../../../../landau-ginzburg-theory.md) is valuable because [symmetries](../../../../../../symmetry-physics.md) restrict a manageable list of local operators, the [gradient](../../../../../../gradient.md) term describes correlations and interfaces, and the [Ginzburg criterion](../../../../../../ginzburg-criterion.md) identifies when neglected fluctuations become decisive. Below the [upper critical dimension](../../../../../../upper-critical-dimension.md) an interacting [renormalization-group fixed point](../../../../../../renormalization-group-fixed-point.md), rather than the bare saddle, determines universal exponents. For continuous [order parameters](../../../../../../order-parameter.md) the manifold of ordered minima also has [Goldstone modes](../../../../../../goldstone-boson.md), and lower-critical-dimension fluctuations require separate attention. **Mean-field minimization supplies an approximation; the Ginzburg ratio decides whether its neglect of fluctuations is justified.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
