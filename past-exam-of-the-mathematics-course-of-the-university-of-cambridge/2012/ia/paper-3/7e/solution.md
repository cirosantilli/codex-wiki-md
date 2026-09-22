<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Use the standard implicit assumption that $p$ is prime, so $\mathbb F_p$ is a [finite field](../../../../../finite-field.md). The matrices in question form $GL_2(\mathbb F_p)$, the [general linear group over a finite field](../../../../../general-linear-group-over-a-finite-field.md). Products stay in the set because [determinants](../../../../../determinant.md) multiply, the identity has determinant one, and

$$
\begin{pmatrix}a&b\\c&d\end{pmatrix}^{-1}
=(ad-bc)^{-1}\begin{pmatrix}d&-b\\-c&a\end{pmatrix}
$$

has entries in the [finite field](../../../../../finite-field.md) and nonzero [determinant](../../../../../determinant.md). Together with associativity this verifies the [group](../../../../../group-split.md) axioms. The multiplication of matrices with column [vectors](../../../../../vector.md) is a [group action](../../../../../group-action.md) because $I v=v$ and $(gh)v=g(hv)$.

Let $C=\langle g\rangle$ be the order-$p$ [cyclic subgroup](../../../../../cyclic-subgroup.md). By the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md), its [group orbits](../../../../../orbit-of-a-group-action.md) on $\mathbb F_p^2$ have size either one or $p$. If $f$ is the number of fixed [vectors](../../../../../vector.md), counting all $p^2$ vectors gives $f\equiv p^2\equiv0\pmod p$. Since the zero [vector](../../../../../vector.md) is fixed, $f\geq1$ and hence $f\geq p$. There is a nonzero fixed [vector](../../../../../vector.md) $v$.

Extend $v$ to a [basis](../../../../../basis.md) $(v,w)$. In this basis $g$ has matrix $\begin{pmatrix}1&b\\0&d\end{pmatrix}$. From $g^p=I$ we get $d^p=1$; in the prime [finite field](../../../../../finite-field.md), $d^p=d$, so $d=1$. Since $g$ has order $p>1$, it is not the identity, and $b\ne0$. Replace $w$ by $b^{-1}w$. Then $g(b^{-1}w)=v+b^{-1}w$, and in the new basis

$$
\boxed{g\sim\begin{pmatrix}1&1\\0&1\end{pmatrix}.}
$$

Thus all the [order-p matrices in GL2 over the prime field](../../../../../order-p-matrices-in-gl2-over-the-prime-field.md) form one [conjugacy class](../../../../../conjugacy-class.md). This proof also works at $p=2$. Primality is essential to the first assertion: for modulus four, $\operatorname{diag}(2,1)$ has nonzero determinant but no inverse, so the set defined using merely nonzero determinants would not be a [group](../../../../../group-split.md).

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
