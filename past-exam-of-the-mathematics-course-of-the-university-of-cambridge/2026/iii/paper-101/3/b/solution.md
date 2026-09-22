<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $K=\operatorname{Frac}R$, let

$$
f(T)=T^d+a_{d-1}T^{d-1}+\cdots+a_0
$$

be the [minimal polynomial of an algebraic element](../../../../../../minimal-polynomial-of-an-algebraic-element.md) $y$ over $K$, and let $B$ be the integral closure of $R$ in a finite normal extension containing all roots of $f$. Since $y$ is integral over $R$ and $R$ is [integrally closed domain](../../../../../../integrally-closed-domain.md), every $a_i$ belongs to $R$.

Write $y=\sum_jp_jz_j$ with $p_j\in\mathfrak p$ and $z_j\in A$. Every $K$-embedding into the normal extension fixes the $p_j$ and sends each $z_j$ to an element integral over $R$. Thus every conjugate of $y$ lies in the extended ideal $\mathfrak pB$. Each nonleading coefficient of $f$ is, up to sign, an [elementary symmetric polynomial](../../../../../../elementary-symmetric-polynomial.md) in those conjugates, so it lies in $\mathfrak pB\cap R$.

For an [integral extension](../../../../../../integral-extension.md), extension followed by contraction preserves a prime ideal:

$$
\mathfrak pB\cap R=\mathfrak p.
$$

Indeed, the determinant trick gives $r^m\in\mathfrak p$ for $r\in\mathfrak pB\cap R$, and primality then gives $r\in\mathfrak p$. Hence $a_i\in\mathfrak p$ for every $i<d$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
