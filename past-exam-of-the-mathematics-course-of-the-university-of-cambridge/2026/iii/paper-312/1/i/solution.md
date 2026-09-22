<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\phi=\bar\phi+\varphi$ and evaluate derivatives of $P$ on the homogeneous background

$$
\bar X=\frac{\bar\phi'^2}{2a^2}.
$$

The first- and second-order changes in $X$ are

$$
\delta_1X=\frac{\bar\phi'\varphi'}{a^2},
\qquad
\delta_2X=\frac{\varphi'^2-(\nabla\varphi)^2}{2a^2}.
$$

After using the background equation to remove the linear action, the quadratic action of the [P(X, phi) scalar field theory](../../../../../../p-x-phi-scalar-field-theory.md) is

$$
S_2=\frac12\int d\tau\,d^3x\left\lbrace
a^2A\varphi'^2-a^2P_X(\nabla\varphi)^2
+2a^2P_{X\phi}\bar\phi'\varphi\varphi'
+a^4P_{\phi\phi}\varphi^2\right\rbrace,
$$

where

$$
A=P_X+2\bar XP_{XX}.
$$

Varying gives

$$
(a^2A\varphi')'-a^2P_X\nabla^2\varphi
+\left[(a^2P_{X\phi}\bar\phi')'-a^4P_{\phi\phi}\right]\varphi=0.
$$

The [Sound speed of a P(X, phi) scalar perturbation](../../../../../../sound-speed-of-a-p-x-phi-scalar-perturbation.md) is

$$
\boxed{c_s^2=\frac{P_X}{P_X+2\bar XP_{XX}}=\frac{P_X}{A}}.
$$

At leading slow variation, take $H$, $c_s$, and the kinetic coefficients as nearly constant and neglect the effective mass and their logarithmic derivatives. The Fourier equation then becomes

$$
\varphi_k''+2\frac{a'}a\varphi_k'+c_s^2k^2\varphi_k=0.
$$

For $u_k=a\varphi_k$ and [de Sitter spacetime](../../../../../../de-sitter-spacetime.md) $a''/a=2/\tau^2$, this is

$$
u_k''+\left(c_s^2k^2-\frac2{\tau^2}\right)u_k=0.
$$

Two independent solutions are

$$
u_k^{\pm}=\left(1\pm\frac{i}{c_sk\tau}\right)e^{\pm ic_sk\tau}.
$$

The [Bunch-Davies vacuum](../../../../../../bunch-davies-vacuum.md) selects the positive-frequency behavior $e^{-ic_sk\tau}$ as $-c_sk\tau\to\infty$. Canonical normalization of $v=a\sqrt A\,\varphi$ gives the general amplitude; with the field normalization $P_X\simeq1$, so $A\simeq c_s^{-2}$, it reduces, up to an overall phase, to

$$
\boxed{\varphi_k(\tau)=
\frac{H}{\sqrt{2c_sk^3}}
(1+ic_sk\tau)e^{-ic_sk\tau}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
