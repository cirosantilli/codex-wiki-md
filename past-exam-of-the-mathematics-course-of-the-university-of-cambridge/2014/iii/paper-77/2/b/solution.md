<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Scale time by $\omega^{-1}$, length by $k^{-1}$, [velocity](../../../../../../velocity.md) by $\omega/k$, [pressure](../../../../../../pressure.md) by $\mu\omega$, and [streamfunction](../../../../../../stream-function.md) by $\omega/k^2$. Write $A=\alpha/k$, $\xi=x-t$, and drop stars from dimensionless coordinates. The surface is $y=\epsilon\sin\xi$ and its material [velocity](../../../../../../velocity.md) in the sheet frame is $(0,-\epsilon\cos\xi)$. The [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) is therefore

$$
\mathbf u(x,\epsilon\sin\xi,t)=(0,-\epsilon\cos\xi),\qquad
\mathbf u\longrightarrow\mathcal U\mathbf e_x\quad(y\to+\infty),\qquad
\mathcal U=kU/\omega.
$$

The stationary matrix identifies a preferred frame. In the sheet frame it translates with $\mathcal U\mathbf e_x$, so [matrix-relative Brinkman velocity](../../../../../../matrix-relative-brinkman-velocity.md) gives the consistent equations

$$
\boxed{-\nabla p+\nabla^2\mathbf u=A^2(\mathbf u-\mathcal U\mathbf e_x),\qquad
\nabla\cdot\mathbf u=0.}
$$

Equivalently one may keep the printed right-hand side $A^2\mathbf u$ after defining $\widetilde p=p-A^2\mathcal U x$; then the far-field [pressure](../../../../../../pressure.md) has the gradient needed to balance that term. Using the printed equation with a uniform far-field flow and no such adjustment is inconsistent. The distinction first matters at second order, since the first-order swimming speed is zero. We solve the upper half-space; the lower half-space is its reflected counterpart.

## ↑ Ancestors (11)

1. [B](../b.md)
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
