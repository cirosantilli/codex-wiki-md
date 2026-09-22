<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

We construct a [cube root of a matrix](../../../../../cube-root-of-a-matrix.md) on each [Jordan block](../../../../../jordan-block.md). Since $A$ is an [invertible matrix](../../../../../invertible-matrix.md) over the [complex numbers](../../../../../complex-number.md), its [Jordan normal form](../../../../../jordan-normal-form.md) is

$$
A=PJP^{-1},\qquad J=\bigoplus_{r=1}^{\ell}J_{m_r}(\lambda_r),\qquad \lambda_r\ne0.
$$

Consider one block $J_m(\lambda)=\lambda I+N$, where $N=J_m(0)$ is a [Nilpotent Jordan block](../../../../../nilpotent-jordan-block.md) and $N^m=0$. Choose a complex [cube root](../../../../../cube-root.md) $\beta$ of $\lambda$, so $\beta^3=\lambda$.

We need a [polynomial](../../../../../polynomial-split.md) $q(z)$ with [constant term](../../../../../constant-term.md) one satisfying

$$
q(z)^3\equiv1+z\pmod{z^m}.
$$

This can be constructed using only [polynomial multiplication](../../../../../polynomial-multiplication.md). Write $q(z)=1+\sum_{j=1}^{m-1}c_jz^j$. Once $c_1,\ldots,c_{j-1}$ have been chosen, the [coefficient](../../../../../coefficient.md) of $z^j$ in $q(z)^3$ is $3c_j$ plus an expression depending only on those earlier [coefficients](../../../../../coefficient.md). Choose $c_j$ to make this [coefficient](../../../../../coefficient.md) one at $j=1$ and zero at $2\leq j<m$. Division by three is possible over the [complex numbers](../../../../../complex-number.md), so the recursion always succeeds. Its first [coefficients](../../../../../coefficient.md) are

$$
c_1=\frac13,\qquad c_2=-\frac19,\qquad c_3=\frac5{81}.
$$

This is the [truncated binomial cube root of the identity plus a nilpotent matrix](../../../../../truncated-binomial-cube-root-of-the-identity-plus-a-nilpotent-matrix.md); equivalently $c_j=\binom{1/3}{j}$, where the generalized [binomial coefficient](../../../../../binomial-coefficient-split.md) is $\alpha(\alpha-1)\cdots(\alpha-j+1)/j!$ and the empty product is one.

Substitute $z=N/\lambda$. The [polynomial remainder](../../../../../remainder-of-polynomial-division.md) is a multiple of $N^m$, hence zero. It follows that

$$
C_m(\lambda)=\beta q(N/\lambda)
\quad\Longrightarrow\quad
C_m(\lambda)^3=\lambda(I+N/\lambda)=J_m(\lambda).
$$

For $m=1$, take $q=1$, so the same construction covers single-entry blocks. Assemble the [block diagonal matrix](../../../../../block-diagonal-matrix.md) $C=\bigoplus_r C_{m_r}(\lambda_r)$. Taking [matrix powers](../../../../../matrix-power.md) respects these blocks, and conjugating back gives

$$
\boxed{B=PCP^{-1},\qquad B^3=PC^3P^{-1}=PJP^{-1}=A.}
$$

Thus every [invertible matrix](../../../../../invertible-matrix.md) over the [complex numbers](../../../../../complex-number.md) has at least one [cube root of a matrix](../../../../../cube-root-of-a-matrix.md). The construction uses only finitely many [matrix powers](../../../../../matrix-power.md).

## ↑ Ancestors (13)

1. [i](../i.md)
2. [c](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
