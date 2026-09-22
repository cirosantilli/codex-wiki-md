<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

On the part with $1\leq z\leq2$, write

$$
\mathbf r(\rho,\phi)
=\left(\rho\cos\phi,\rho\sin\phi,
\sqrt{\rho^2-1}\right),
\qquad
\sqrt2\leq\rho\leq\sqrt5.
$$

This is the upper portion of a [hyperboloid of one sheet](../../../../../one-sheet-hyperboloid.md). Choosing the [outward orientation](../../../../../orientation-of-a-surface.md), whose normal points radially away from the $z$-axis, the [vector area element](../../../../../vector-area-element.md) is

$$
\begin{aligned}
d\mathbf S
&=(\mathbf r_\phi\times\mathbf r_\rho)\,d\rho\,d\phi\\
&=\boxed{\left(
\frac{\rho^2\cos\phi}{\sqrt{\rho^2-1}},
\frac{\rho^2\sin\phi}{\sqrt{\rho^2-1}},
-\rho\right)d\rho\,d\phi}.
\end{aligned}
$$

Its radial component is positive and its vertical component is negative. Reversing the normal reverses all the fluxes below.

For

$$
\mathbf A=(-yz^2,xz^2,0),
$$

the [curl](../../../../../curl.md) is

$$
\nabla\times\mathbf A=(-2xz,-2yz,2z^2).
$$

On the surface, $z^2=\rho^2-1$, and therefore

$$
(\nabla\times\mathbf A)\cdot d\mathbf S
=-2\rho(2\rho^2-1)\,d\rho\,d\phi.
$$

Direct integration gives

$$
\begin{aligned}
\int_S\nabla\times\mathbf A\cdot d\mathbf S
&=-2\int_0^{2\pi}\int_{\sqrt2}^{\sqrt5}
\rho(2\rho^2-1)\,d\rho\,d\phi\\
&=-2\pi[\rho^4-\rho^2]_{\sqrt2}^{\sqrt5}\\
&=\boxed{-36\pi}.
\end{aligned}
$$

To verify this with the [Stokes theorem](../../../../../stokes-theorem.md), note that on a circle of fixed $\rho,z$,

$$
\mathbf A=z^2\rho\,\mathbf e_\phi,
\qquad
d\mathbf r=\rho\mathbf e_\phi\,d\phi.
$$

The induced [boundary orientation](../../../../../boundary-orientation.md) runs in the negative $\phi$ direction on the top circle and the positive $\phi$ direction on the bottom circle. Hence

$$
\oint_{\partial S}\mathbf A\cdot d\mathbf r
=2\pi(1^2)(\sqrt2)^2
-2\pi(2^2)(\sqrt5)^2
=4\pi-40\pi
=-36\pi.
$$

For $S'$, Stokes' theorem again reduces the flux to its two boundary circles. The outward orientation gives positive $\phi$ direction at $z=-1$, where $\rho^2=2$, and negative $\phi$ direction at $z=\sqrt2$, where $\rho^2=3$. Thus

$$
\boxed{
\int_{S'}\nabla\times\mathbf A\cdot d\mathbf S
=2\pi(1)(2)-2\pi(2)(3)
=-8\pi}.
$$

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
