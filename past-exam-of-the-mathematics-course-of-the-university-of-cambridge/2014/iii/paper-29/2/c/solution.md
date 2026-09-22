<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Scale the disk to the [unit disc](../../../../../../unit-disc.md), so that the starting point is $a=1/r\in(0,1)$. Use the [Möbius transformation](../../../../../../mobius-transformation.md)

$$
\psi_a(w)=\frac{w-a}{1-aw},
$$

which maps the disk onto itself, sends $a$ to $0$, and sends $1$ to $1$. By [conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md), the exit image is the circular exit of a [Brownian motion](../../../../../../brownian-motion-split.md) starting at $0$. [Rotational invariance of planar Brownian motion](../../../../../../rotational-invariance-of-planar-brownian-motion.md) makes that exit uniform in angle.

The endpoints of the right semicircle satisfy

$$
\psi_a(i)=\frac{-2a+i(1-a^2)}{1+a^2}=e^{i\varphi},\qquad
\psi_a(-i)=e^{-i\varphi},\qquad
\varphi=\frac\pi2+2\arctan a.
$$

Its image is the arc through $1$ between these points, of angular length $2\varphi$. Thus the [Möbius calculation of circular Brownian exit](../../../../../../mobius-calculation-of-circular-brownian-exit.md) gives

$$
\mathbb P_1(E_+)=\frac{2\varphi}{2\pi}=\frac12+\frac2\pi\arctan(1/r).
$$

Since $E_+$ and $E_-$ partition the exit almost surely, part (b) yields

$$
\boxed{\mathbb P_1(T(r)<S)=\frac4\pi\arctan(1/r)
=\frac2\pi\arctan\!\left(\frac{2r}{r^2-1}\right).}
$$

The last equality uses $2\arctan(1/r)\in(0,\pi/2)$, so the double-angle tangent identity uses the stated principal branch. As a check, the boundary angle derivative of $\psi_a$ is $(1-a^2)/|e^{i\theta}-a|^2$; integrating this circular exit density over the right semicircle gives exactly the integral supplied in the question.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
