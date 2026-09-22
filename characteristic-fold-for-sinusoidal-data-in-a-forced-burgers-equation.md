# Characteristic fold for sinusoidal data in a forced Burgers equation

↑ **Parent:** [Method of characteristics](method-of-characteristics.md)

For the [partial differential equation](partial-differential-equation-split.md) $u_x+u u_y=x$ with initial profile $u(0,\eta)=1+\sin\eta$, the [method of characteristics](method-of-characteristics.md) gives the parametrized surface

$$
u=1+\sin\eta+\frac{x^2}{2},\qquad y=\eta+x(1+\sin\eta)+\frac{x^3}{6}.
$$

The projection to the $(x,y)$ plane has [Jacobian determinant](jacobian-determinant.md) $1+x\cos\eta$. It is positive for $|x|<1$, so the [inverse function theorem](inverse-function-theorem.md) makes the surface a unique local solution graph there. For $\eta\ge0$, strict monotonicity and divergence to infinity give a global inverse onto $y\ge x+x^3/6$ at each such $x$.

The [derivative](derivative.md) $u_y=\cos\eta/(1+x\cos\eta)$ becomes singular when that projection first degenerates, although $u$ itself stays finite. At $x=1$ the degenerate labels are odd multiples of $\pi$, and at $x=-1$ they are even multiples. At either boundary the limiting map remains strictly increasing, with isolated zero [derivatives](derivative.md), so fixed image values determine convergent labels. Consequently the gradient diverges at fixed $y=(2k+1)\pi+7/6$ as $x\uparrow1$, and at fixed $y=2k\pi-7/6$ as $x\downarrow-1$, using $k\ge0$ and $k\ge1$, respectively, to stay in the half-line initial domain. At these first singularities $y_{\eta\eta}=0$ and $y_{\eta\eta\eta}\ne0$; this is the onset of loss of invertibility, rather than an ordinary nondegenerate fold at the initial singular time.

## ↑ Ancestors (8)

1. [Method of characteristics](method-of-characteristics.md)
2. [Characteristic curve](characteristic-curve.md)
3. [Transport equation](transport-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2004/8/solution.md)
