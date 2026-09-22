<h1 id="6/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $r=x-u^*$. If $u^*$ is a best approximation, then for every $v\in\mathcal U_n$ and real $t$, the competitor $u^*+tv$ satisfies

$$
\|r-tv\|^2-\|r\|^2=-2t\operatorname{Re}(r,v)+t^2\|v\|^2\ge0.
$$

The linear coefficient must be zero, since otherwise choosing sufficiently small $t$ of the appropriate sign makes this expression negative. Hence $\operatorname{Re}(r,v)=0$. In a real [inner product space](../../../../../../../inner-product-space.md) this is the desired orthogonality; in a complex [inner product space](../../../../../../../inner-product-space.md), apply the same argument to $iv$ to show that the imaginary part also vanishes. Thus $(r,v)=0$ for all $v\in\mathcal U_n$.

Conversely, suppose this orthogonality holds. Every competitor $u\in\mathcal U_n$ has $u-u^*\in\mathcal U_n$. The [Pythagorean identity](../../../../../../../pythagorean-theorem-in-an-inner-product-space.md) then gives

$$
\|x-u\|^2=\|r-(u-u^*)\|^2=\|r\|^2+\|u-u^*\|^2\ge\|r\|^2.
$$

Equality forces $u=u^*$. We have proved the characterization, as well as uniqueness:

$$
\boxed{u^*\text{ is best}\iff (x-u^*,v)=0\text{ for every }v\in\mathcal U_n.}
$$

This is the [orthogonal projection onto a finite-dimensional subspace](../../../../../../../orthogonal-projection-onto-a-finite-dimensional-subspace.md). Completeness of the ambient space is not needed. Existence follows, for example, by solving the invertible [Gram matrix](../../../../../../../gram-matrix.md) system in a [basis](../../../../../../../basis.md) of the finite-dimensional [linear subspace](../../../../../../../vector-subspace.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [6](../../../6.md)
4. [Paper 75](../../../../paper-75-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
