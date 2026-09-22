<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

Linearity of the [integral](../../../../../integral.md) in each argument gives a [bilinear form](../../../../../bilinear-form.md), and $fg=gf$ gives [symmetry](../../../../../symmetry-physics.md). Also $(f,f)=\int_{-1}^1 f(x)^2dx\geq0$. If a [polynomial](../../../../../polynomial-split.md) $f$ is nonzero somewhere on this interval, [continuity](../../../../../continuous-function.md) makes $f^2$ strictly positive on a smaller interval, so the [integral](../../../../../integral.md) is positive. A [polynomial](../../../../../polynomial-split.md) vanishing on the whole interval is the zero [polynomial](../../../../../polynomial-split.md). Thus the form is [positive-definite](../../../../../positive-definite-bilinear-form.md) and is an [inner product](../../../../../inner-product.md).

Apply the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) to $1,x,x^2$. Odd [functions](../../../../../function-split.md) have zero [integral](../../../../../integral.md), so $x$ is already [orthogonal](../../../../../orthogonal-vectors.md) to $1$, and the third [orthogonal polynomial](../../../../../orthogonal-polynomial.md) is $x^2-1/3$. Their squared [norms](../../../../../norm.md) are

$$
 \|1\|^2=2,\qquad \|x\|^2=\frac23,\qquad
 \|x^2-1/3\|^2=\frac25-\frac49+\frac29=\frac8{45}.
$$

Therefore an **orthonormal basis** is

$$
 \boxed{\left\{\frac1{\sqrt2},\ \sqrt{\frac32}\,x,\ \sqrt{\frac58}\,(3x^2-1)\right\}.}
$$

These are the first three normalized [Legendre polynomials](../../../../../legendre-polynomial.md). Their distinct degrees also prove that they span the three-dimensional [vector space](../../../../../vector-space-split.md).

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
