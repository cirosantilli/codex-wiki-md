<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

With polar unit vectors $\mathbf e_r=(\cos\theta,\sin\theta,0)$ and $\mathbf e_\theta=(-\sin\theta,\cos\theta,0)$, the second term is $\Gamma\mathbf e_\theta/(2\pi r)$. It is tangent to circles, independent of $z$, and has zero [divergence](../../../../../divergence.md) and zero [vorticity](../../../../../vorticity.md) away from the axis. Its singular axis carries a [line vortex](../../../../../line-vortex.md); adding the constant [velocity field](../../../../../velocity-field.md) gives a [uniform flow](../../../../../uniform-flow.md) plus that [line vortex](../../../../../line-vortex.md).

The counterclockwise [circulation](../../../../../circulation-physics.md) around a positively oriented loop is $\oint\mathbf u\cdot d\mathbf r$. For a radius-$R$ circle, the [uniform flow](../../../../../uniform-flow.md) contributes zero and the [line vortex](../../../../../line-vortex.md) contributes

$$
\oint_{C_R}\frac\Gamma{2\pi R}\mathbf e_\theta\cdot R\mathbf e_\theta\,d\theta=\Gamma.
$$

Any loop winding once around the axis has the same [circulation](../../../../../circulation-physics.md), by [Stokes theorem](../../../../../stokes-theorem.md) in the nonsingular intervening region.

On $C_R$, $\mathbf n=\mathbf e_r$, $\mathbf u\cdot\mathbf n=U\cos\theta$, and $dl=R\,d\theta$. Thus

$$
\oint_{C_R}(\mathbf u\cdot\mathbf n)\mathbf u\,dl=RU^2\mathbf e_x\int_0^{2\pi}\cos\theta\,d\theta+\frac{U\Gamma}{2\pi}\int_0^{2\pi}\cos\theta\,\mathbf e_\theta\,d\theta=\boxed{\frac12\boldsymbol\Gamma\mathbin\times\mathbf U}.
$$

In fact this equality holds for every $R>0$ for the stated field, since the remaining vector [integral](../../../../../integral.md) is $(0,\pi,0)$.

This is the advective part of the [momentum flux](../../../../../momentum-flux.md). To obtain the force, include [pressure](../../../../../pressure.md). For steady [irrotational flow](../../../../../irrotational-flow.md), the [Bernoulli equation](../../../../../bernoulli-equation.md) gives

$$
p=p_\infty-\frac\rho2(|\mathbf u|^2-U^2)=p_\infty+\frac{\rho U\Gamma\sin\theta}{2\pi R}-\frac{\rho\Gamma^2}{8\pi^2R^2}.
$$

The constant terms integrate to zero against $\mathbf n$; the remaining [pressure](../../../../../pressure.md) contribution is $\oint p\mathbf n\,dl=\rho\boldsymbol\Gamma\times\mathbf U/2$. The total outward [momentum flux](../../../../../momentum-flux.md) plus [pressure](../../../../../pressure.md) term is therefore $\rho\boldsymbol\Gamma\times\mathbf U$, the force of the obstacle on the fluid. The opposite force, of fluid on the obstacle per unit span, is

$$
\boxed{\mathbf F=\rho\mathbf U\times\boldsymbol\Gamma.}
$$

This is the [Kutta–Joukowski theorem](../../../../../kutta-joukowski-theorem.md), with positive $\Gamma$ defined counterclockwise: positive $U$ and $\Gamma$ give force in the negative $y$ direction. For an actual two-dimensional [aerofoil](../../../../../airfoil.md), faster-decaying far-field terms do not change this limit. **The displayed advective integral supplies half the lift; pressure supplies the other half.**

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
