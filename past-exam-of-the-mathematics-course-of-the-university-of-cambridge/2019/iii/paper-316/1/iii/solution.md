<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $u=e^2$ and use the torque balance from part (ii) to eliminate the [resonant argument](../../../../../../resonant-argument.md). The resonant contribution is

$$
\dot u_{\rm res}=2e\dot e_{\rm res}=-2qCe^q\sin\phi
=\frac{2qA}{a^2(p+q)}(1+3u).
$$

Adding the [Poynting–Robertson drag](../../../../../../poynting-robertson-drag.md) contribution gives the [dissipative resonant eccentricity equilibrium](../../../../../../dissipative-resonant-eccentricity-equilibrium.md) equation

$$
\dot u=\frac A{a^2}\left[\frac{2q}{p+q}-\frac{5p-q}{p+q}u\right]
=-\frac{u-B}{\tau},
$$

where

$$
\boxed{B=\frac{2q}{5p-q},\qquad \tau=\frac{a^2(p+q)}{A(5p-q)}.}
$$

For $5p>q$, integrating with $u(0)=e_0^2$ gives

$$
\boxed{e(t)=\sqrt{B+(e_0^2-B)e^{-t/\tau}}.}
$$

Here $a$ is the fixed resonant [semi-major axis](../../../../../../semi-major-axis.md) and the expression describes averaged evolution, neglecting the small [resonant-argument libration](../../../../../../resonant-argument-libration.md). The physical bound-orbit interpretation also requires $B<1$; a quantitatively controlled second-order calculation needs $B\ll1$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
