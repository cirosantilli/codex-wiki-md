<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X=x/\epsilon$, $a(X)=1/d(X)$, and seek

$$
u=u_0(x,t)+\epsilon u_1(x,X,t)+\cdots
$$

with periodic correctors. The leading cell equation makes $u_0$ independent of $X$. At the next order, continuity of microscopic heat flux gives

$$
a(X)(u_{0x}+u_{1X})=J(x,t).
$$

Averaging over one period and using $\langle u_{1X}\rangle=0$ yields

$$
u_{0x}=J\int_0^1d(X)dX=J\overline d.
$$

Thus the [periodic homogenization of a diffusion equation](../../../../../../periodic-homogenization-of-a-diffusion-equation.md) has effective diffusivity $1/\overline d$:

$$
\boxed{u_{0t}=\frac1{\overline d}u_{0xx}.}
$$

For the sawtooth profile, the two triangular areas give

$$
\overline d=\int_0^p\frac{2X}{p}dX
+\int_p^1\frac{2(1-X)}{1-p}dX=p+(1-p)=1.
$$

The homogenized problem is therefore the unit-diffusivity [heat equation](../../../../../../heat-equation.md). Its half-line step solution is

$$
\boxed{u(x,t)=T_0\operatorname{erfc}\left(\frac{x}{2\sqrt t}\right)
=T_0\left[1-\operatorname{erf}\left(\frac{x}{2\sqrt t}\right)\right].}
$$

It has the required initial and boundary limits, and direct differentiation verifies $u_t=u_{xx}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
