# Gaussian diffusion of a smooth initial profile

↑ **Parent:** [Laplacian](laplacian.md)

For [diffusion](diffusion.md) with a constant [diffusion coefficient](diffusion-coefficient.md) $D>0$ and no sources, the model [flux](flux.md) is $J=-D\nabla u$. A [continuity equation](continuity-equation.md) gives $u_t=-\nabla\cdot J=D\Delta u$. This proportionality is a constitutive assumption about transport; the [continuity equation](continuity-equation.md) expresses conservation. If $D$ varies with position, it must remain inside the [divergence](divergence.md), giving $u_t=\nabla\cdot(D\nabla u)$ instead.[Volume II, §12–4, equations 12.19–12.22: diffusion flux and local conservation](the-feynman-lectures-on-physics-volume-ii-by-richard-feynman-and-others.md)

An exact constructed [heat equation](heat-equation.md) example on the whole plane uses dimensionless coordinates with $D=1$ and the smooth initial [Gaussian function](gaussian-function.md) $u(x,y,0)=e^{-r^2}$. Set $s=1+4t$. For $t\geq0$,

$$
u(x,y,t)=\frac1s e^{-r^2/s},\qquad r^2=x^2+y^2.
$$

Direct differentiation verifies both the initial condition and

$$
u_t=\Delta u=\frac{4(r^2-s)}{s^3}e^{-r^2/s}.
$$

The center decreases, while the region $r^2>s$ increases at that instant. The sign-change [circle](circle.md) expands with [radius](radius.md) $\sqrt{s}$. A fixed outer location can initially increase and later decrease as this [circle](circle.md) passes it.

<a id="image-an-exact-gaussian-function-spreads-under-the-heat-equation-while-its-spatial-integral-stays-fixed"></a>
![](laplacian-gaussian-diffusion-profiles.png)

**[Figure 8](#image-an-exact-gaussian-function-spreads-under-the-heat-equation-while-its-spatial-integral-stays-fixed). An exact Gaussian function spreads under the heat equation while its spatial integral stays fixed**. Original analytic model with $D=1$. Left: radial profiles at $t=0,1/4,1$, whose peaks are $1,1/2,1/5$. Right: $u_t=\Delta u$ at $t=1/4$; the sign changes at $r=\sqrt2$. These are model predictions, not experimental measurements. The conserved quantity uses the whole-plane area element $2\pi r\,dr$, rather than the unweighted area under a radial profile.

At time $t$, the peak is $1/s$, and the [radius](radius.md) where the profile is $1/e$ times its peak is $\sqrt{s}$. The width grows as the height falls. Integration in [polar coordinates](polar-coordinates.md) gives

$$
\int_{\mathbb R^2}u(x,y,t)\,dx\,dy=2\pi\int_0^\infty\frac r{s}e^{-r^2/s}\,dr=\pi.
$$

Thus a decreasing peak is compatible with a conserved spatial [integral](integral-split.md). Dividing $u$ by $\pi$ makes a [probability density function](probability-density-function.md) with coordinate [variances](variance-split.md) $s/2=1/2+2t$, connecting the same spreading to [Brownian motion](brownian-motion-split.md) with [diffusion coefficient](diffusion-coefficient.md) one. Equivalently the profile is evolved by the [Gaussian heat kernel](gaussian-heat-kernel.md) with time parameter $2t$, since that article uses generator $\tfrac12\Delta$.

## ↑ Ancestors (9)

1. [Laplacian](laplacian.md)
2. [Vector calculus](vector-calculus.md)
3. [Multivariable calculus](multivariable-calculus-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/20/b/solution.md)
