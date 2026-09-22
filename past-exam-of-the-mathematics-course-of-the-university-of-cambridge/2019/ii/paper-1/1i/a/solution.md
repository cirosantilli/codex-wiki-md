<h1 id="1i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) says that if the positive integers $m_1,\ldots,m_r$ are pairwise [coprime](../../../../../../coprime-integers.md) and $M=\prod_i m_i$, then for arbitrary residue classes $a_i\pmod{m_i}$ there is a unique residue class $x\pmod M$ satisfying

$$
x\equiv a_i\pmod{m_i}
\qquad(1\leq i\leq r).
$$

Equivalently, reduction is a [ring isomorphism](../../../../../../ring-isomorphism.md)

$$
\mathbb Z/M\mathbb Z\longrightarrow
\prod_{i=1}^r\mathbb Z/m_i\mathbb Z.
$$

For existence, put $M_i=M/m_i$. Pairwise coprimality gives $\gcd(M_i,m_i)=1$, so [Bézout's identity](../../../../../../bezout-identity.md) supplies an integer $u_i$ with $u_iM_i\equiv1\pmod{m_i}$. Then

$$
x=\sum_{i=1}^r a_i u_iM_i
$$

has the required residues, because every term except the $i$th is divisible by $m_i$. If $x$ and $y$ are two solutions, each $m_i$ divides $x-y$. Pairwise coprimality then implies that their product $M$ divides $x-y$, proving uniqueness modulo $M$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1I](../../1i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
