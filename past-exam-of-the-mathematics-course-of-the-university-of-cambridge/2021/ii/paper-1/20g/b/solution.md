<h1 id="20g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
\beta=\frac{\alpha+\alpha^2}{2}.
$$

Using $\alpha^3=5\alpha-8$, multiplication by $\beta$ on the ordered basis $(1,\alpha,\beta)$ is determined by

$$
\beta\cdot1=\beta,
\qquad
\beta\alpha=-4+2\alpha+\beta,
\qquad
\beta^2=-4-\alpha+3\beta.
$$

Its matrix, with these coordinate vectors as columns, is

$$
M_\beta=
\begin{pmatrix}
0&-4&-4\\
0&2&-1\\
1&1&3
\end{pmatrix}.
$$

The [characteristic polynomial](../../../../../../characteristic-polynomial.md) is

$$
\det(TI-M_\beta)=T^3-5T^2+11T-12.
$$

By the [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem.md), this monic integer polynomial annihilates $\beta$, so $\beta$ is an [algebraic integer](../../../../../../algebraic-integer.md).

Let

$$
A=\mathbb Z\langle1,\alpha,\beta\rangle.
$$

The element $\alpha$ is also integral because it satisfies the monic polynomial $f$. Hence $A\subseteq\mathcal O_K$. Since

$$
\alpha^2=2\beta-\alpha,
$$

the lattice $\mathbb Z[\alpha]$ has index two in $A$. The given power-basis discriminant is

$$
\Delta(1,\alpha,\alpha^2)=-4\cdot307,
$$

so the [discriminant-index formula for an integral lattice](../../../../../../discriminant-index-formula-for-an-integral-lattice.md) gives

$$
\Delta(1,\alpha,\beta)
=\frac{-4\cdot307}{2^2}
=-307.
$$

If $m=[\mathcal O_K:A]$, then

$$
-307=m^2d_K.
$$

Because $307$ is prime, the square $m^2$ can divide $307$ only when $m=1$. Thus

$$
\boxed{\mathcal O_K=A
=\mathbb Z\langle1,\alpha,\beta\rangle},
$$

so $(1,\alpha,\beta)$ is an [integral basis of the cubic field of discriminant minus 307](../../../../../../integral-basis-of-the-cubic-field-of-discriminant-minus-307.md).

Finally, the relation $\beta^2=-4-\alpha+3\beta$ gives

$$
\alpha=-4+3\beta-\beta^2.
$$

**Consequently $\mathcal O_K=\mathbb Z[\beta]$, which will allow direct use of Dedekind's theorem.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20G](../../20g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
