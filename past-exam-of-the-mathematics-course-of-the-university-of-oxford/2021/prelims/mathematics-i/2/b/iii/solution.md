<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

Use the [linear map](../../../../../../../linear-map.md)

$$
\Phi:V_{n-1}\times V_{n-1}\longrightarrow V_{2n-1},\qquad
\Phi(a,b)=ap+bq.
$$

It is well defined because $\deg(ap),\deg(bq)\leq2n-1$, and it is a [linear map](../../../../../../../linear-map.md) by [distributivity](../../../../../../../distributive-property.md) of [polynomial multiplication](../../../../../../../polynomial-multiplication.md). If $\Phi(a,b)=0$ for a nonzero pair, [ii](../ii.md) would give a common [root of a polynomial](../../../../../../../root-of-a-polynomial.md) of $p$ and $q$. The hypothesis therefore implies $\ker\Phi=\{(0,0)\}$, so $\Phi$ is [injective](../../../../../../../injective-function.md).

By [i](../i.md), the domain and codomain both have [dimension](../../../../../../../dimension-vector-space.md) $2n$: a [basis](../../../../../../../basis.md) of the domain is $(x^j,0),(0,x^j)$ for $0\leq j<n$, and a [basis](../../../../../../../basis.md) of the codomain is $1,x,\ldots,x^{2n-1}$. The stated finite-dimensional result makes $\Phi$ [surjective](../../../../../../../surjective-function.md). In particular $1$ has a preimage, proving the [degree bound in polynomial Bézout's identity](../../../../../../../degree-bound-in-polynomial-bezout-s-identity.md):

$$
\boxed{\exists\,u,v\in V_{n-1}\quad up+vq=1.}
$$

Indeed, [injectivity](../../../../../../../injective-function.md) also proves uniqueness of this pair under the stated [degree of a polynomial](../../../../../../../degree-of-a-polynomial.md) bounds.

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [b](../../b.md)
3. [2](../../../2.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
