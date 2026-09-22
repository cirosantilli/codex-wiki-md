<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $r=x-u^*$. If $u^*$ is a [best approximation](../../../../../../best-approximation-in-a-normed-space.md) in the finite-dimensional [linear subspace](../../../../../../vector-subspace.md), then for every $v$ in it and every real $t$,

$$
0\le\|r-tv\|^2-\|r\|^2=-2t\operatorname{Re}(r,v)+t^2\|v\|^2.
$$

A nonzero real linear [coefficient](../../../../../../coefficient.md) would make this negative for sufficiently small $t$ of the appropriate sign. Hence $\operatorname{Re}(r,v)=0$. In a complex [inner product space](../../../../../../inner-product-space.md), apply the argument to $iv$ too; the imaginary part also vanishes. Thus $(x-u^*,v)=0$ for every $v$ in the subspace.

Conversely, if that orthogonality holds, every other candidate has the form $u^*+v$, and the [Pythagorean theorem](../../../../../../pythagorean-theorem.md) in the [inner product](../../../../../../inner-product.md) norm gives

$$
\|x-u^*-v\|^2=\|x-u^*\|^2+\|v\|^2\ge\|x-u^*\|^2.
$$

Equality requires $v=0$. Therefore

$$
\boxed{u^*\text{ is the unique best approximant}\ \Longleftrightarrow\ x-u^*\perp\mathcal U_n.}
$$

The next part constructs this [orthogonal projection](../../../../../../orthogonal-projection.md) explicitly. No completeness of the whole [inner product space](../../../../../../inner-product-space.md) is required for projection onto a finite-dimensional subspace.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../1.md)
3. [7](../../7.md)
4. [Paper 61](../../../paper-61-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
