<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

Substitute $C=t^\alpha F(\xi)$, $\xi=rt^{-\beta}$. The derivatives give

$$
t^{\alpha-1}(\alpha F-\beta\xi F')
=Dt^{\alpha-2\beta}\left(F''+\frac2\xi F'\right).
$$

For a nontrivial spreading [similarity solution](../../../../../similarity-solution.md), equality at all times requires $\boxed{\beta=1/2}$. The conserved total number of molecules is

$$
N=4\pi\int_0^\infty C(r,t)r^2\,dr
=4\pi t^{\alpha+3\beta}\int_0^\infty F(\xi)\xi^2\,d\xi.
$$

A finite nonzero constant $N$ therefore requires $\alpha+3\beta=0$, giving $\boxed{\alpha=-3/2}$. In one dimension the same diffusion length exponent is $1/2$, but conservation gives amplitude exponent $-1/2$; generally it is $-d/2$ in dimension $d$.

The profile equation is consequently

$$
\boxed{D\left(F''+\frac2\xi F'\right)+\frac12\xi F'+\frac32F=0.}
$$

Multiplication by $\xi^2$ puts it in the integrated form $[D\xi^2F'+\xi^3F/2]'=0$. For the regular localized [Gaussian heat kernel](../../../../../gaussian-heat-kernel.md) profile, the constant is zero at the origin, so $DF'+\xi F/2=0$. Integrating gives

$$
\boxed{F(\xi)=A e^{-\xi^2/(4D)},\qquad
C(r,t)=\frac{N}{(4\pi Dt)^{3/2}}e^{-r^2/(4Dt)}.}
$$

The second expression chooses the optional normalization $A=N/(4\pi D)^{3/2}$. Its mass is $N$, and its width tends to zero with $t^{1/2}$ while its mass stays fixed, so it approaches $N$ times a [Dirac delta distribution](../../../../../dirac-delta-function.md) at the origin as $t\downarrow0$.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
