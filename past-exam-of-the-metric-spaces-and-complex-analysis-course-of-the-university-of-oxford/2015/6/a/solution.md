<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $z\overline z=|z|^2$ and $\overline Bz+B\overline z=2\operatorname{Re}(\overline Bz)$. When $A\ne0$, [completing the square](../../../../completing-the-square.md) gives

$$
A|z|^2+\overline Bz+B\overline z+C=A\left|z+\frac BA\right|^2+C-\frac{|B|^2}{A}.
$$

Thus, with $\Delta=|B|^2-AC$,

$$
\boxed{\left|z+\frac BA\right|^2=\frac{\Delta}{A^2}\quad(A\ne0).}
$$

If $\Delta>0$, this is a [circle](../../../../circle.md) with centre $-B/A$ and [radius](../../../../radius.md) $\sqrt\Delta/|A|$. If $\Delta=0$, it is the single point $-B/A$, sometimes called a degenerate [circle](../../../../circle.md) of [radius](../../../../radius.md) zero. If $\Delta<0$, it is the [empty set](../../../../empty-set.md), because a squared [complex modulus](../../../../complex-modulus.md) cannot be negative.

When $A=0$ and $B\ne0$, write $B=u+iv$ and $z=x+iy$. The remaining equation is

$$
\boxed{ux+vy=-\frac C2,\qquad (u,v)\ne(0,0),}
$$

which is a [straight line](../../../../straight-line.md) with [normal vector](../../../../normal-vector.md) $(u,v)$. It passes through zero exactly when $C=0$. Finally, when $A=B=0$, the equation has no solutions if $C\ne0$ and every [complex number](../../../../complex-number.md) is a solution if $C=0$.

The complete [classification of a real complex-circle equation](../../../../classification-of-a-real-complex-circle-equation.md) therefore includes two degeneracies in addition to ordinary [circles](../../../../circle.md), [straight lines](../../../../straight-line.md) and the [empty set](../../../../empty-set.md):

$$
\boxed{\begin{array}{c|c}
\text{condition}&\text{locus}\\\hline
A\ne0,\ \Delta>0&\text{circle}\ (-B/A,\sqrt\Delta/|A|)\\
A\ne0,\ \Delta=0&\{-B/A\}\\
A\ne0,\ \Delta<0&\varnothing\\
A=0,\ B\ne0&\text{line }2\operatorname{Re}(\overline Bz)+C=0\\
A=B=0,\ C\ne0&\varnothing\\
A=B=C=0&\mathbb C
\end{array}}
$$

For the three advertised alternatives to be exhaustive, one must exclude the identically zero equation and either exclude or explicitly allow [radius](../../../../radius.md)-zero [circles](../../../../circle.md). This is a qualification of the unrestricted coefficients, not a reason to discard the genuine [circle](../../../../circle.md) and [straight line](../../../../straight-line.md) cases used next.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
