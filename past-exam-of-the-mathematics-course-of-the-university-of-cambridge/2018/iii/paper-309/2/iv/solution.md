<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The index order in $M_\mu{}^\nu x^\mu$ fixes the rotation sign. With the entries specified in the paper, the [integral curves of a vector field](../../../../../../integral-curve-of-a-vector-field.md) satisfy

$$
\frac{dx^1}{d\lambda}=A^1+x^2,\qquad
\frac{dx^2}{d\lambda}=A^2-x^1,\qquad
\frac{dx^j}{d\lambda}=A^j\quad(j\ge3).
$$

Shift to $u=x^1-A^2$, $v=x^2+A^1$. Then $\dot u=v$, $\dot v=-u$, so $u^2+v^2$ is constant. If $x(0)=x_0$, put $u_0=x_0^1-A^2$ and $v_0=x_0^2+A^1$. Solving this linear [ordinary differential equation](../../../../../../ordinary-differential-equation.md) gives the full [local flow](../../../../../../local-flow.md):

$$
\boxed{\begin{aligned}
x^1(\lambda)&=A^2+u_0\cos\lambda+v_0\sin\lambda,\\
x^2(\lambda)&=-A^1+v_0\cos\lambda-u_0\sin\lambda,\\
x^j(\lambda)&=x_0^j+A^j\lambda\quad(j\ge3).
\end{aligned}}
$$

The planar motion is a circle centred at $(A^2,-A^1)$, traversed clockwise as $\lambda$ increases. A nonzero vector $(A^3,\ldots,A^n)$ produces a [helical orbit of a Euclidean Killing vector](../../../../../../helical-orbit-of-a-euclidean-killing-vector.md); zero drift gives a circle. At zero radius the curves are straight lines in the remaining directions, or stationary points if that drift also vanishes. These formulas are defined for every real $\lambda$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
