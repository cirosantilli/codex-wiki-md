<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Uniform composition and adiabatic convection give $T\propto\rho^{2/3}$ for a monatomic perfect gas. Hence near the centre

$$
T=T_c\left(1-\frac23\lambda r^2+O(r^4)\right).
$$

The luminosity equation is

$$
\frac{dL_r}{dr}=4\pi r^2\rho\epsilon
\propto r^2\rho^2T^\eta.
$$

Since $\rho^2T^\eta\propto1-(2+2\eta/3)\lambda r^2$, integration gives

$$
\boxed{
L_r\propto r^3\left[
1-\frac35\left(2+\frac{2\eta}{3}\right)\lambda r^2
\right]}.
$$

Similarly,

$$
m_r\propto r^3\left(1-\frac35\lambda r^2\right),
\qquad
P\propto\rho T
=P_c\left(1-\frac53\lambda r^2\right).
$$

The [radiative temperature gradient](../../../../../../radiative-temperature-gradient.md) is

$$
\nabla_{\rm rad}
=\frac{3\kappa L_rP}{16\pi a_{\rm rad}cGm_rT^4}.
$$

Expanding $\kappa=\kappa_0\rho^aT^{-b}$ and all the preceding factors gives

$$
\boxed{
\nabla_{\rm rad}=\nabla_{{\rm rad},c}(1-Ar^2+O(r^4))},
$$

where

$$
\boxed{
A=\lambda\left(
a-\frac{2b}{3}+\frac{2\eta-2}{5}
\right)}.
$$

The [Schwarzschild criterion](../../../../../../schwarzschild-criterion.md) requires

$$
\boxed{\nabla_{{\rm rad},c}>\nabla_{\rm ad}=\frac25}
$$

for the centre to be convectively unstable. If $A>0$, the radiative gradient decreases outward and can cross $2/5$, producing a finite [convective core](../../../../../../convective-core.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
