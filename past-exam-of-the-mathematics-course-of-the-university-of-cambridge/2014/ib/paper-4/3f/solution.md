<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

A [contraction mapping](../../../../../contraction-mapping.md) $T$ on a [metric space](../../../../../metric-space.md) satisfies $d(Tx,Ty)\leq qd(x,y)$ for all $x,y$, with one constant $0\leq q<1$. The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) says that on a nonempty [complete metric space](../../../../../complete-metric-space.md) such a map has a unique [fixed point](../../../../../fixed-point.md); successive iterates from any starting point converge to it. More precisely, if $x_n=T^nx_0$, then $d(x_n,x_*)\leq q^nd(x_1,x_0)/(1-q)$.

The [Volterra integration operator](../../../../../volterra-operator.md) maps [continuous functions](../../../../../continuous-function.md) to [continuous functions](../../../../../continuous-function.md). In the [uniform norm](../../../../../supremum-norm.md),

$$
 \|Af-Ag\|_\infty\leq\|f-g\|_\infty.
$$

This constant cannot be decreased: for $f=1$ and $g=0$, $Af(x)=x$, and both [uniform norms](../../../../../supremum-norm.md) are one. Hence **$A$ is not a contraction**.

Changing the order of [integration](../../../../../integral.md) over the triangular region gives

$$
 A^2f(x)=\int_0^x\int_0^t f(s)\,ds\,dt
 =\int_0^x(x-s)f(s)\,ds.
$$

Thus

$$
 \|A^2f-A^2g\|_\infty\leq\sup_{0\leq x\leq1}\frac{x^2}{2}\|f-g\|_\infty
 =\frac12\|f-g\|_\infty.
$$

**$A^2$ is a contraction, with sharp constant $1/2$.** This is an example of an [iterated contraction](../../../../../iterated-contraction.md).

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
