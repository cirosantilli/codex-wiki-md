<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $P_j$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto $V_j$. The dilation property and the [orthonormal basis](../../../../../../orthonormal-basis.md) property give the [orthonormal basis](../../../../../../orthonormal-basis.md) $\varphi_{j,k}(x)=2^{j/2}\varphi(2^jx-k)$ of $V_j$. The periodized nonnegative function

$$
F(u)=\sum_{k\in\mathbb Z}|\varphi(u-k)|^2
$$

has period one and $\int_0^1F=\|\varphi\|_2^2=1$, by [Tonelli theorem](../../../../../../tonelli-theorem.md). For a function $g\in L^2(\mathbb R)$ with [compact support](../../../../../../compact-support.md) contained in a bounded interval $I$, [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the [Parseval identity](../../../../../../parseval-identity.md) give

$$
\|P_jg\|_2^2=\sum_k|\langle g,\varphi_{j,k}\rangle|^2
\leq \|g\|_2^2\int_I2^jF(2^jx)\,dx
=\|g\|_2^2\int_{2^jI}F(u)\,du\longrightarrow0
$$

as $j\to-\infty$. The last step uses absolute continuity of the integral of a locally $L^1$ function, since the interval's length tends to zero. If $f\in\bigcap_jV_j$, then

$$
|\langle f,g\rangle|=|\langle f,P_jg\rangle|\leq\|f\|_2\|P_jg\|_2\longrightarrow0.
$$

Functions with [compact support](../../../../../../compact-support.md) are dense in $L^2$, so $f=0$. Consequently

$$
\boxed{\bigcap_{j\in\mathbb Z}V_j=\{0\}.}
$$

This proof needs neither the density axiom nor any [compact support](../../../../../../compact-support.md) assumption on the [scaling function](../../../../../../scaling-function.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
