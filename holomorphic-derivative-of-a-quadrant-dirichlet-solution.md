# Holomorphic derivative of a quadrant Dirichlet solution

↑ **Parent:** [Dirichlet Poisson integral in a quadrant](dirichlet-poisson-integral-in-a-quadrant.md)

For the bounded [Dirichlet Poisson integral in a quadrant](dirichlet-poisson-integral-in-a-quadrant.md), the [Wirtinger derivative](wirtinger-derivatives.md) is

$$
u_z(z)=\frac{2z}{\pi i}\int_0^\infty r\left[\frac{g_2(r)}{(r^2-z^2)^2}+\frac{g_1(r)}{(r^2+z^2)^2}\right]dr.
$$

This follows by differentiating the [Schwarz integral formula](schwarz-integral-formula.md) composed with $z^2$, remembering that for real boundary data $u_z$ is half the derivative of a [holomorphic function](holomorphic-function.md) whose [real part](real-part.md) is $u$. For complex boundary data, apply the construction to the real and imaginary parts separately and use linearity. If the data and their [derivatives](derivative.md) decay sufficiently, [integration by parts](integration-by-parts.md) gives

$$
u_z(z)=\frac z{\pi i}\left[\int_0^\infty\frac{g_2'(r)}{r^2-z^2}\,dr+\int_0^\infty\frac{g_1'(r)}{r^2+z^2}\,dr\right].
$$

The endpoint terms cancel exactly when $g_1(0)=g_2(0)$. Interior denominators do not vanish because $\operatorname{Im}z^2>0$.

## ↑ Ancestors (9)

1. [Dirichlet Poisson integral in a quadrant](dirichlet-poisson-integral-in-a-quadrant.md)
2. [Poisson integral](poisson-integral.md)
3. [Poisson kernel for the upper half-space](poisson-kernel-for-the-upper-half-space.md)
4. [Poisson equation](poisson-equation.md)
5. [Partial differential equation](partial-differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/3/solution.md)
