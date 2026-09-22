<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $W$ is proper, $T$ is a nonzero [linear functional](../../../../../linear-functional.md). Choose $e\in X$ with $Te=1$, by rescaling any [vector](../../../../../vector.md) outside its [kernel](../../../../../kernel-of-a-linear-map-split.md). For every $x\in X$,

$$
x=\underbrace{(x-(Tx)e)}_{\in W}+(Tx)e.
$$

If $ae\in W$, applying $T$ gives $a=0$. Consequently this is a [direct sum](../../../../../direct-sum.md), and the [quotient vector space](../../../../../quotient-vector-space.md) $X/W$ has [dimension](../../../../../dimension-vector-space.md) one. This computes the [codimension of a vector subspace](../../../../../codimension-of-a-vector-subspace.md):

$$
\boxed{X=W\oplus\langle e\rangle,\qquad\operatorname{codim}_XW=1.}
$$

To prove boundedness without assuming [completeness](../../../../../completeness.md), use the [linear functional with closed kernel](../../../../../linear-functional-with-closed-kernel.md) criterion directly. Since $W$ is a [closed set](../../../../../closed-set.md) and $e\notin W$, the distance

$$
d=\inf_{w\in W}\|e-w\|_X
$$

is positive. If $Tx\ne0$, then $e-x/(Tx)\in W$, so

$$
d\leq\left\|\frac{x}{Tx}\right\|_X=\frac{\|x\|_X}{|Tx|}.
$$

For $Tx=0$ the resulting estimate is immediate. Therefore

$$
\boxed{|Tx|\leq d^{-1}\|x\|_X\quad(x\in X),\qquad T\in X^*.}
$$

Here $X^*$ denotes the [continuous dual space](../../../../../continuous-dual-space-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis I course of the University of Oxford](../../../../split.md)
6. [Functional analysis I course of the University of Oxford](../../../../../functional-analysis-i-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
