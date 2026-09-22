<h1 id="31e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $a=b=0$, take the [Logarithmic first integral of the Lotka-Volterra equations](../../../../../../logarithmic-first-integral-of-the-lotka-volterra-equations.md)

$$
\boxed{V(x,y)=r(x-\log x-1)+y-\log y-1.}
$$

Along a trajectory,

$$
\begin{aligned}
\dot V
&=r\left(1-\frac1x\right)x(1-y)
+\left(1-\frac1y\right)ry(x-1)\\
&=r(x-1)(1-y)+r(y-1)(x-1)=0.
\end{aligned}
$$

Thus $V$ is a [first integral](../../../../../../first-integral.md). The scalar function $h(s)=s-\log s-1$ is nonnegative for $s>0$, vanishes only at $s=1$, and tends to infinity as $s\downarrow0$ or $s\to\infty$. Moreover,

$$
\nabla^2V=
\begin{pmatrix}r/x^2&0\\0&1/y^2\end{pmatrix}
$$

is positive definite, so $V$ is [strictly convex](../../../../../../strictly-convex-function.md). It follows that $(1,1)$ is its unique critical point and every level set $V=c>0$ is a compact smooth simple closed curve in the [positive quadrant](../../../../../../positive-quadrant.md). The vector field is nonzero on such a level curve, so uniqueness of solutions makes each connected level curve one [periodic orbit](../../../../../../periodic-orbit.md). The zero level consists of the fixed point $(1,1)$. **Hence every trajectory in $\Lambda$ is either periodic or the fixed point $(1,1)$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31E](../../31e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
