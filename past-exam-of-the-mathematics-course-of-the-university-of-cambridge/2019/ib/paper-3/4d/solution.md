<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

The [Möbius transformation](../../../../../mobius-transformation.md)

$$
w=i\frac{1-z}{1+z}
$$

maps the [unit disc](../../../../../unit-disc.md) conformally onto the upper half-plane. On the upper semicircle of its boundary, $w$ approaches the positive real axis; on the lower semicircle it approaches the negative real axis. If $0<\arg w<\pi$, the harmonic function

$$
\phi(w)=\phi_0\left(1-\frac{2\arg w}{\pi}\right)
$$

has the required boundary limits.

For $z=x+iy$,

$$
w=\frac{2y+i(1-x^2-y^2)}{(1+x)^2+y^2}.
$$

Since the imaginary part is positive inside the disc,

$$
\frac\pi2-\arg w
=\arctan\frac{\operatorname{Re}w}{\operatorname{Im}w}
=\arctan\frac{2y}{1-x^2-y^2}.
$$

Therefore the solution of the [Dirichlet problem](../../../../../dirichlet-problem.md) is

$$
\boxed{\phi(x,y)=\frac{2\phi_0}{\pi}
\arctan\!\left(\frac{2y}{1-x^2-y^2}\right)},
\qquad x^2+y^2<1.
$$

The exceptional boundary endpoints are precisely the jump points of the prescribed data.

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
