<h1 id="16a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

As the real charge descends to height $z(t)$, its instantaneous [image charge](../../../../../../image-charge.md) is at $-z(t)$. The force is therefore

$$
m\ddot z=-\frac{q^2}{4\pi\varepsilon_0(2z)^2},\qquad \ddot z=-\frac{\kappa}{z^2},\qquad \kappa=\frac{q^2}{16\pi\varepsilon_0m}.
$$

The image is not kept at its initial position. Multiplying by $\dot z$ and using $z(0)=d$, $\dot z(0)=0$ gives

$$
\frac12\dot z^2=\kappa\left(\frac1z-\frac1d\right),\qquad \dot z<0.
$$

For the [falling charge above a grounded conducting plane](../../../../../../falling-charge-above-a-grounded-conducting-plane.md), the arrival time is

$$
T=\frac1{\sqrt{2\kappa}}\int_0^d\frac{dz}{\sqrt{1/z-1/d}}.
$$

Put $z=d\sin^2\theta$; the integral becomes $2d^{3/2}\int_0^{\pi/2}\sin^2\theta\,d\theta=\pi d^{3/2}/2$. Hence

$$
\boxed{T=\frac{\pi d^{3/2}}{2\sqrt{2\kappa}}=\frac\pi{|q|}\sqrt{2\pi\varepsilon_0md^3}.}
$$

This is the finite arrival time in the specified ideal force model, for $q\ne0$. The field-force derivation also avoids incorrectly using the full real-image pair interaction energy: the conductor's effective energy is $-q^2/(16\pi\varepsilon_0z)$, with the factor one-half appropriate to induced charge.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [16A](../../16a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
