<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

The [dot product](../../../../../dot-product.md) and [Euclidean norm](../../../../../euclidean-norm.md) are $\mathbf x\cdot\mathbf y=\sum_i x_iy_i$ and $|\mathbf x|=\sqrt{\mathbf x\cdot\mathbf x}$. For every real $t$,

$$
0\leq|\mathbf x-t\mathbf y|^2=|\mathbf x|^2-2t\,\mathbf x\cdot\mathbf y+t^2|\mathbf y|^2.
$$

Its [quadratic discriminant](../../../../../quadratic-discriminant.md) is nonpositive, proving the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) $|\mathbf x\cdot\mathbf y|\leq|\mathbf x||\mathbf y|$. In the inequality asked for, equality holds exactly when $\mathbf x$ is a positive scalar multiple of $\mathbf y$, and

$$
\boxed{\theta=\arccos\frac{\mathbf x\cdot\mathbf y}{|\mathbf x||\mathbf y|}.}
$$

Using the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) and its contraction identity,

$$
(\mathbf a\times\mathbf b)\cdot(\mathbf b\times\mathbf c)
=\varepsilon_{ijk}a_jb_k\varepsilon_{i\ell m}b_\ell c_m
=(\mathbf a\cdot\mathbf b)(\mathbf b\cdot\mathbf c)-|\mathbf b|^2(\mathbf a\cdot\mathbf c).
$$

Put $T=\mathbf a\cdot(\mathbf b\times\mathbf c)$, the [scalar triple product](../../../../../scalar-triple-product.md). Cyclic symmetry gives $\mathbf m\cdot\mathbf a=\mathbf m\cdot\mathbf b=\mathbf m\cdot\mathbf c=T$, so each requested angle $\phi$ satisfies $\cos\phi=T/|\mathbf m|$. If every pairwise angle is $\theta$ and $t=\cos\theta$, the preceding identity gives

$$
|\mathbf m|^2=3(1-t^2)+6(t^2-t)=3(1-t)^2,
$$

and therefore **$|\mathbf m|=\sqrt3(1-\cos\theta)$**. This is $0$ when $\theta=0$; for a right-handed [orthonormal basis](../../../../../orthonormal-basis.md) and $\theta=\pi/2$, $\mathbf m=\mathbf a+\mathbf b+\mathbf c$ has norm $\sqrt3$.

The three [planes](../../../../../plane.md) have equations $\mathbf a\cdot\mathbf x=\mathbf a\cdot\mathbf p$, $\mathbf b\cdot\mathbf x=\mathbf b\cdot\mathbf q$, and $\mathbf c\cdot\mathbf x=\mathbf c\cdot\mathbf r$. They meet at one point exactly when $\Delta=\mathbf a\cdot(\mathbf b\times\mathbf c)\ne0$, meaning their normals are [linearly independent vectors](../../../../../linear-independence.md). The point is

$$
\boxed{\mathbf x=
\frac{(\mathbf a\cdot\mathbf p)(\mathbf b\times\mathbf c)+(\mathbf b\cdot\mathbf q)(\mathbf c\times\mathbf a)+(\mathbf c\cdot\mathbf r)(\mathbf a\times\mathbf b)}
{\mathbf a\cdot(\mathbf b\times\mathbf c)}.}
$$

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
