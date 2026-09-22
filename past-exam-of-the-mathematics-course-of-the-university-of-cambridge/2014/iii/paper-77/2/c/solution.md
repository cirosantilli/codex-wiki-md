<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking the curl of the [Brinkman equation](../../../../../../brinkman-equation.md) eliminates [pressure](../../../../../../pressure.md) and the constant matrix [velocity](../../../../../../velocity.md). With $\mathbf u=(\psi_y,-\psi_x)$ and [vorticity](../../../../../../vorticity.md) $-\nabla^2\psi$, the [Brinkman swimming sheet](../../../../../../brinkman-swimming-sheet.md) equation is

$$
\boxed{(\nabla^2-A^2)\nabla^2\psi=0.}
$$

The surface conditions are conditions on partial derivatives evaluated on the moving boundary:

$$
\boxed{\psi_y(x,\epsilon\sin\xi,t)=0,\qquad
\psi_x(x,\epsilon\sin\xi,t)=\epsilon\cos\xi.}
$$

At infinity, $\psi_y\to\mathcal U$ and $\psi_x\to0$. The derivative of $\psi$ along the surface also equals $\epsilon\cos\xi$, because $\psi_y=0$ there, so a convenient gauge has $\psi(x,\epsilon\sin\xi,t)=\epsilon\sin\xi$. Decaying perturbations and the [force-free](../../../../../../force-free.md) condition determine the swimming solution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
