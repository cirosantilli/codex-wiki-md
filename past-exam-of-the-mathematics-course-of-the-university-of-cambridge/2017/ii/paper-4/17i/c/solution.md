<h1 id="17i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [cyclotomic polynomial](../../../../../../cyclotomic-polynomial.md) $\Phi_7=1+X+\cdots+X^6$ is irreducible: replacing $X$ by $X+1$ gives an [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md) at seven. Hence the extension has degree six, and

$$
\boxed{G=(\mathbb Z/7\mathbb Z)^\times\cong C_6,\qquad\sigma_a(\eta)=\eta^a.}
$$

There is one subgroup of each order $1,2,3,6$, and therefore precisely four intermediate fields. The trivial subgroup fixes $\mathbb Q(\eta)$; the whole group fixes $\mathbb Q$. The order-two subgroup $\{1,6\}$ is [complex conjugation](../../../../../../complex-conjugation.md) and fixes $\mathbb Q(\eta+\eta^{-1})$, of degree three: $\eta$ satisfies $X^2-(\eta+\eta^{-1})X+1$ and is not real.

The order-three subgroup $\{1,2,4\}$ fixes $u=\eta+\eta^2+\eta^4$. Its other conjugate is $v=\eta^3+\eta^5+\eta^6$. Expanding products and using $\sum_{j=1}^6\eta^j=-1$ gives $u+v=-1$ and $uv=2$. Thus $u^2+u+2=0$, and this [fixed field](../../../../../../fixed-field.md) is $\mathbb Q(u)=\mathbb Q(\sqrt{-7})$, of degree two. These generators have the required degrees and are fixed by the indicated subgroups, so the [Galois correspondence](../../../../../../galois-correspondence.md) proves they are the full fixed fields.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17I](../../17i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
