<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

The substitution removes the zero-order term: $u_x=e^{-x^2}(v_x-2xv)$ and $u_y=e^{-x^2}v_y$, so the [partial differential equation](../../../../../partial-differential-equation-split.md) becomes $v_x+xv_y=1$. Its [method of characteristics](../../../../../method-of-characteristics.md) gives

$$
\frac{dy}{dx}=x,\qquad \frac{dv}{dx}=1.
$$

The invariant is $\eta=y-x^2/2$. Therefore $v=x+F(\eta)$. The initial line $x=0$ is noncharacteristic, and the boundary data give $F(\eta)=\eta e^{-\eta^2}$. Hence

$$
\boxed{u(x,y)=e^{-x^2}\left[x+\left(y-\frac{x^2}{2}\right)e^{-(y-x^2/2)^2}\right].}
$$

Each characteristic meets the data line once, ensuring uniqueness among differentiable solutions, and substituting the result verifies both the equation and the data.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
