<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At $t=1$, the diagonal entries of $U-L$ are $2$, while every off-diagonal $(i,j)$ entry is

$$
-a_{ij}=-2\cos\left(\frac{\pi}{m_{ij}}\right).
$$

Hence $U-L$ is exactly the [Coxeter Gram matrix](../../../../../../coxeter-gram-matrix.md) $G(W)$, and part c gives

$$
\det(I-C)=\det G(W).
$$

For a [Finite Coxeter group](../../../../../../finite-coxeter-group.md) the Gram matrix is [positive definite](../../../../../../positive-definite-matrix.md), and for a [Hyperbolic Coxeter group](../../../../../../hyperbolic-coxeter-group.md) it is nondegenerate with Lorentzian signature. In either case $\det(I-C)\ne0$, so $1$ is not an [eigenvalue](../../../../../../eigenvalue.md) of $C$ and the [Coxeter element](../../../../../../coxeter-element.md) fixes no nonzero vector.

For an [Affine Coxeter group](../../../../../../affine-coxeter-group.md), the Gram form has a nonzero [radical](../../../../../../radical-of-a-bilinear-form.md). If $0\ne v\in\operatorname{rad}G(W)$, then $\langle v,e_i\rangle=0$ for every $i$, and every generating reflection satisfies

$$
\sigma(x_i)v=v-\langle v,e_i\rangle e_i=v.
$$

Their product $\sigma(c)$ therefore fixes $v$. Thus every affine Coxeter element has a nonzero fixed vector.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
