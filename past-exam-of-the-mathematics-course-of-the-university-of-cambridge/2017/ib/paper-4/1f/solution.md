<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

For a [basis](../../../../../basis.md) $v_1,\ldots,v_d$ of the [real vector space](../../../../../real-vector-space.md) $V$, the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) constructs an [orthonormal basis](../../../../../orthonormal-basis.md) successively:

$$
w_j=v_j-\sum_{i<j}\langle v_j,e_i\rangle e_i,\qquad e_j=\frac{w_j}{\sqrt{\langle w_j,w_j\rangle}}.
$$

The [inner product](../../../../../inner-product.md) makes $w_j$ [orthogonal](../../../../../orthogonal-vectors.md) to all earlier $e_i$. Moreover $w_j\ne0$, since otherwise $v_j$ would be a [linear combination](../../../../../linear-combination.md) of its predecessors, contrary to [linear independence](../../../../../linear-independence.md). Induction gives $\operatorname{span}(e_1,\ldots,e_j)=\operatorname{span}(v_1,\ldots,v_j)$. Starting with a [basis](../../../../../basis.md) of a [linear subspace](../../../../../vector-subspace.md) $U$ and extending it to a [basis](../../../../../basis.md) of $V$ gives the same construction with the first $r=\dim U$ vectors spanning $U$.

The [orthogonal complement](../../../../../orthogonal-complement.md) is $U^\perp=\{v\in V:\langle v,u\rangle=0\text{ for every }u\in U\}$. For every $v\in V$, set $u=\sum_{i=1}^r\langle v,e_i\rangle e_i$. Then $u\in U$ and $v-u\in U^\perp$. If $w\in U\cap U^\perp$, then $\langle w,w\rangle=0$, so $w=0$ by definiteness of the [inner product](../../../../../inner-product.md). Thus the [direct sum](../../../../../direct-sum.md) is

$$
\boxed{V=U\oplus U^\perp}.
$$

This also covers $U=0$ and $U=V$.

For the [polynomial](../../../../../polynomial-split.md) space, the form is immediately a [symmetric bilinear form](../../../../../symmetric-bilinear-form.md), and $(f,f)=f(1)^2+f(2)^2+f(3)^2\geq0$. A nonzero [polynomial](../../../../../polynomial-split.md) of [degree of a polynomial](../../../../../degree-of-a-polynomial.md) at most two cannot have three distinct [roots of a polynomial](../../../../../root-of-a-polynomial.md), so this form is an [inner product](../../../../../inner-product.md) for $n=1,2$. For $n\geq3$, the nonzero [polynomial](../../../../../polynomial-split.md) $(x-1)(x-2)(x-3)$ has $(f,f)=0$. Therefore, among the stipulated positive [integers](../../../../../integer.md),

$$
\boxed{n\in\{1,2\}}.
$$

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
