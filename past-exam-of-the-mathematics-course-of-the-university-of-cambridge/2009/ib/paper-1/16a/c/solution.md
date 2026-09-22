<h1 id="16a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At instantaneous height $z$, the [image charge](../../../../../../image-charge.md) is a distance $2z$ below the real charge, giving force $m\ddot z=-K/z^2$ with $K=q^2/(16\pi\varepsilon_0)$. Multiplying by $\dot z$ and using rest at $z=d$ gives

$$
\frac m2\dot z^2=K\left(\frac1z-\frac1d\right).
$$

The induced-conductor potential energy is $-K/z$, not the full energy of a pair of independently movable charges. On the falling branch, integrate the reciprocal speed:

$$
t_{\rm hit}=\sqrt{\frac m{2K}}\int_0^d\sqrt{\frac{zd}{d-z}}\,dz=\sqrt{\frac{md^3}{2K}}\int_0^1\sqrt{\frac{s}{1-s}}\,ds=\frac\pi2\sqrt{\frac{md^3}{2K}}.
$$

The last [integral](../../../../../../integral.md) is $\pi/2$ by $s=\sin^2\theta$. Hence the [fall time of a charge toward a grounded plane](../../../../../../fall-time-of-a-charge-toward-a-grounded-plane.md) in the electrostatic Newtonian model is

$$
\boxed{t_{\rm hit}=\frac{\pi\sqrt{2\pi\varepsilon_0md^3}}{|q|}.}
$$

For $q=0$ there is no force and the particle remains at rest.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16A](../../16a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
