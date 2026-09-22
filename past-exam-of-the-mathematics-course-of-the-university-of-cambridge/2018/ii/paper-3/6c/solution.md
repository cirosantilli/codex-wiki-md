<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

For a radial function, the equation is

$$
n_t=\frac D r\frac{\partial}{\partial r}
\left(rn\frac{\partial n}{\partial r}\right).
$$

Therefore, assuming the population density and radial flux decay at infinity and are regular at the origin,

$$
\frac d{dt}\left(2\pi\int_0^\infty nr\,dr\right)
=2\pi D\left[rn n_r\right]_{0}^{\infty}=0.
$$

Thus $N$ is conserved; it is the total population obtained by integrating density over the plane. This is the global form of the equation's [conservation law](../../../../../conservation-law.md).

Set

$$
n(r,t)=\left(\frac N{Dt}\right)^{1/2}f(x),
\qquad
x=\frac r{(NDt)^{1/4}}.
$$

Then

$$
n_t=\left(\frac N D\right)^{1/2}t^{-3/2}
\left(-\frac12f-\frac14xf'\right),
$$

while the radial diffusion term has the same prefactor and equals

$$
D\nabla\cdot(n\nabla n)
=\left(\frac N D\right)^{1/2}t^{-3/2}
\frac1x\frac d{dx}(xff').
$$

Equating them and multiplying by $x$ gives

$$
\frac d{dx}\left(xff'+\frac14x^2f\right)=0,
$$

so the proposed ansatz is a [similarity solution](../../../../../similarity-solution.md).

Regularity at $x=0$ makes the constant of integration zero. Wherever $f>0$,

$$
f'=-\frac x4,
\qquad
f(x)=\frac{x_0^2-x^2}{8}
$$

for some $x_0>0$. The nonnegative weak solution continues as $f=0$ once this parabola reaches zero:

$$
\boxed{f(x)=\left[\frac{x_0^2-x^2}{8}\right]_+.}
$$

This is the [two-dimensional Barenblatt profile for quadratic porous-medium diffusion](../../../../../two-dimensional-barenblatt-profile-for-quadratic-porous-medium-diffusion.md); its degenerate diffusivity permits [compact support](../../../../../compact-support.md).

Indeed, conservation requires

$$
1=2\pi\int_0^\infty f(x)x\,dx
=\frac{\pi x_0^4}{16},
$$

so $x_0=(16/\pi)^{1/4}$ if desired. At time $t$ the populated disk has radius $x_0(NDt)^{1/4}$ and hence area

$$
\boxed{A(t)=\pi x_0^2(NDt)^{1/2}.}
$$

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
