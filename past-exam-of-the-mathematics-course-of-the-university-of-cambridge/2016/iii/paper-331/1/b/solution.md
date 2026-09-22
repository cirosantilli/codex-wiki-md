<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A direct elimination of [pressure](../../../../../../pressure.md) gives the same result as taking a double [curl](../../../../../../curl.md) of the momentum equation. [Incompressibility](../../../../../../incompressible-flow.md) gives $\nabla^2p=\mathrm{Ra}\,\mathrm{Pr}\,\partial_z\theta$. Apply $\nabla^2$ to the vertical momentum equation and subtract this pressure derivative to obtain

$$
\boxed{\partial_t\nabla^2w=\mathrm{Ra}\,\mathrm{Pr}\,\nabla_h^2\theta+\mathrm{Pr}\nabla^4w,\qquad
\partial_t\theta=w+\nabla^2\theta.}
$$

Here $\nabla_h^2=\partial_x^2+\partial_y^2$ is the horizontal [Laplacian](../../../../../../laplacian.md). At $z=0,1$, impermeability gives $w=0$ and fixed temperature gives $\theta=0$. The [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md) gives $\partial_zu=\partial_zv=0$, since horizontal derivatives of the boundary value $w=0$ vanish. Differentiating [incompressibility](../../../../../../incompressible-flow.md) once in $z$ therefore gives

$$
\boxed{w=\partial_z^2w=\theta=0\quad\text{at }z=0,1.}
$$

For a horizontal [Fourier mode](../../../../../../fourier-mode.md) $X=e^{i(k_xx+k_yy)}$, $\nabla_h^2X=-\lambda^2X$ with real $\lambda=\sqrt{k_x^2+k_y^2}$. More generally the nonnegative spectrum of $-\nabla_h^2$ follows by [integration by parts](../../../../../../integration-by-parts.md) for periodic or square-integrable horizontal disturbances. Substituting the separated [normal mode](../../../../../../normal-mode.md) gives, with $D=d/dz$,

$$
\sigma(D^2-\lambda^2)W=-\mathrm{Ra}\,\mathrm{Pr}\lambda^2\Theta+\mathrm{Pr}(D^2-\lambda^2)^2W,\qquad
(D^2-\lambda^2-\sigma)\Theta=-W.
$$

The [boundary conditions](../../../../../../boundary-condition.md) admit a complete [Fourier sine series](../../../../../../fourier-sine-series.md) in $z$. For a nonzero horizontal [wavenumber](../../../../../../wavenumber.md), take $W=W_n\sin(n\pi z)$, $\Theta=\Theta_n\sin(n\pi z)$, and set $a_n^2=\lambda^2+n^2\pi^2$. The two amplitude equations are

$$
a_n^2(\sigma+\mathrm{Pr}a_n^2)W_n=\mathrm{Ra}\,\mathrm{Pr}\lambda^2\Theta_n,\qquad
(\sigma+a_n^2)\Theta_n=W_n.
$$

Thus **the [stress-free convection growth-rate polynomial](../../../../../../stress-free-convection-growth-rate-polynomial.md) is**

$$
\boxed{(\sigma+\mathrm{Pr}a_n^2)(\sigma+a_n^2)=\frac{\mathrm{Ra}\,\mathrm{Pr}\lambda^2}{a_n^2}.}
$$

Its [discriminant](../../../../../../discriminant.md) is $(\mathrm{Pr}-1)^2a_n^4+4\mathrm{Ra}\,\mathrm{Pr}\lambda^2/a_n^2$, so both [growth rates](../../../../../../growth-rate.md) are real for $\mathrm{Ra}>0$. For $\mathrm{Ra}<0$, its two coefficients after the leading term are positive: their sum gives $\sigma_1+\sigma_2=-(1+\mathrm{Pr})a_n^2<0$, and their product is $\mathrm{Pr}(a_n^4-\mathrm{Ra}\lambda^2/a_n^2)>0$. Real roots are both negative; nonreal roots have real part $-(1+\mathrm{Pr})a_n^2/2<0$. **Hence stable heating from above damps every mode.** Horizontally uniform thermal modes and uncoupled horizontal viscous modes are also purely damped; impermeability and [incompressibility](../../../../../../incompressible-flow.md) exclude a horizontally uniform nonzero $w$.

Because the unstable-side roots are real, the onset is stationary, an [exchange of stabilities in stress-free convection](../../../../../../exchange-of-stabilities-in-stress-free-convection.md). Setting $\sigma=0$ gives the [free-slip convection neutral curve](../../../../../../free-slip-convection-neutral-curve.md)

$$
\mathrm{Ra}_n(\lambda)=\frac{(\lambda^2+n^2\pi^2)^3}{\lambda^2}.
$$

With $x=\lambda^2$, its derivative has the sign of $2x-n^2\pi^2$. Its minimum is at $x=n^2\pi^2/2$, with value $27n^4\pi^4/4$. Minimizing also over $n\geq1$ gives **the critical values**

$$
\boxed{\lambda_c=\frac\pi{\sqrt2},\qquad\mathrm{Ra}_c=\frac{27\pi^4}{4}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
