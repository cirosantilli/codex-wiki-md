<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The uniform stationarity equation and local stability condition are

$$
rM+uM^3+vM^5=h,\qquad V''(M)=r+3uM^2+5vM^4>0.
$$

For $u>0$, $h=0$, and small negative $r$, the stable nonzero solution satisfies $M^2=-r/u+O(r^2)$. Thus the [order parameter](../../../../../../order-parameter.md) vanishes continuously as $r\uparrow0$. The equilibrium [Landau free energy](../../../../../../landau-free-energy.md) has leading singular contribution $f_{\min}=-r^2/(4u)$ below the transition and zero above it. Its first thermal derivative is continuous, while its second derivative has a finite jump: the [mean-field approximation](../../../../../../mean-field-approximation.md) predicts a [continuous phase transition](../../../../../../continuous-phase-transition.md) with no [latent heat](../../../../../../latent-heat.md). The [magnetic susceptibility](../../../../../../magnetic-susceptibility.md) follows by differentiating the stationarity equation:

$$
\chi=\frac{\partial M}{\partial h}=\frac{1}{r+3uM^2+5vM^4}.
$$

It diverges on approaching the ordinary [thermodynamic critical point](../../../../../../thermodynamic-critical-point.md), and the quadratic [Landau scalar correlation length](../../../../../../landau-scalar-correlation-length.md) behaves as $\xi\sim\sqrt{\kappa/|r|}$, with a different amplitude on the two sides.

For $u<0$, a nonzero stationary point at $h=0$ has $r+uM^2+vM^4=0$. Substitution into $V(M)-V(0)$ gives $-uM^4/4-vM^6/3$. Setting this to zero yields

$$
\boxed{M_{\mathrm{coex}}^2=-\frac{3u}{4v},\qquad r_{\mathrm{coex}}=\frac{3u^2}{16v}.}
$$

The finite jump of $M$ makes this a [first-order phase transition](../../../../../../first-order-phase-transition.md). For a thermal path $r=r(T)$ with $r'(T)\ne0$ and the other coefficients fixed, $\partial f_{\min}/\partial T=r'(T)M^2/2$ jumps, giving an entropy discontinuity and nonzero [latent heat](../../../../../../latent-heat.md). The [Landau free energy](../../../../../../landau-free-energy.md) itself remains continuous. The disordered minimum loses stability at $r=0$; the two nonzero stationary solutions merge at $r=u^2/(4v)$. These [spinodal points](../../../../../../spinodal-point.md) bound [metastability](../../../../../../metastability.md), but neither replaces the equilibrium [phase coexistence](../../../../../../phase-coexistence.md) condition.

Writing $r=a t$ with $a>0$ near an ordinary [thermodynamic critical point](../../../../../../thermodynamic-critical-point.md), the zero-field equation gives $M\sim(-t)^{1/2}$. At $r=0$, small $h$ obeys $h=uM^3+O(M^5)$, hence $M\sim\operatorname{sgn}(h)|h|^{1/3}$. The ordinary [mean-field critical exponents](../../../../../../mean-field-critical-exponent.md) are therefore **$\beta=1/2$ and $\delta=3$**. These are [Landau theory](../../../../../../landau-theory.md) predictions, not dimension-independent values for an interacting theory below its [upper critical dimension](../../../../../../upper-critical-dimension.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
