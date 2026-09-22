<h1 id="17b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the pole as $(x_0,y_0)$ with $x_0,y_0>0$. The [method of images](../../../../../../method-of-images.md) uses three reflected poles with signs $-, -, +$. Thus

$$
G(x,y)=\frac1{2\pi}\left[\log|(x,y)-(x_0,y_0)|-\log|(x,y)-(-x_0,y_0)|-\log|(x,y)-(x_0,-y_0)|+\log|(x,y)-(-x_0,-y_0)|\right].
$$

The logarithms cancel in pairs on each axis. Only the original pole is in the interior, so this is the required [Dirichlet Green function in a quadrant](../../../../../../dirichlet-green-function-in-a-quadrant.md).

On the horizontal boundary $(t,0)$ the outward normal is $-\mathbf e_y$. Differentiating the four logarithms gives

$$
\begin{aligned}
\partial_nG(t,0)&=\frac{y_0}{\pi}\left(\frac1{(t-x_0)^2+y_0^2}-\frac1{(t+x_0)^2+y_0^2}\right)\\
&=\frac{4x_0y_0t}{\pi[(t-x_0)^2+y_0^2][(t+x_0)^2+y_0^2]}.
\end{aligned}
$$

Multiply by the horizontal [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) $e^{-t^2}$ and integrate to obtain

$$
F(x_0,y_0)=\frac{4x_0y_0}{\pi}\int_0^\infty\frac{te^{-t^2}}{[(t-x_0)^2+y_0^2][(t+x_0)^2+y_0^2]}\,dt.
$$

By exchanging the axes, the vertical boundary contributes $F(y_0,x_0)$. The representation in part (a) consequently gives

$$
\boxed{\phi(x_0,y_0)=F(x_0,y_0)+F(y_0,x_0).}
$$

For the unbounded-domain condition, the same expression is the [Poisson integral](../../../../../../poisson-integral.md) after the conformal [change of variables](../../../../../../change-of-variables-formula.md) $w=(x+iy)^2$ to the upper half-plane, with real-axis data $e^{-|s|}$. This continuous boundary function tends to zero at both ends. Its [Poisson integral](../../../../../../poisson-integral.md) tends to zero as $|w|\to\infty$: split the data into a compact part, whose kernel integral tends to zero, and a tail uniformly smaller than any prescribed positive number. Hence the constructed function has the required decay, and its two boundary traces agree at the corner. The [maximum principle for harmonic functions](../../../../../../maximum-principle-for-harmonic-functions.md) on expanding quarter-discs proves uniqueness among decaying solutions. The corner value is obtained by continuity as $1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17B](../../17b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
