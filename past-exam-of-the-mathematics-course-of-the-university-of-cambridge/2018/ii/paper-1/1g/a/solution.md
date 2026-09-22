<h1 id="1g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For pairwise [coprime integers](../../../../../../coprime-integers.md) $m_1,\ldots,m_r$, put $M=\prod_i m_i$. The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) states that reduction gives an isomorphism

$$
\mathbb Z/M\mathbb Z\longrightarrow\prod_{i=1}^r\mathbb Z/m_i\mathbb Z.
$$

Equivalently, every system $x\equiv a_i\pmod {m_i}$ has one solution modulo $M$.

For existence, let $M_i=M/m_i$. Since $\gcd(M_i,m_i)=1$, choose $u_i$ with $u_iM_i\equiv1\pmod {m_i}$. Then

$$
x=\sum_{i=1}^r a_i u_iM_i
$$

has every required residue: modulo $m_j$, all terms except the $j$th vanish and the remaining term is $a_j$. For uniqueness, if $x$ and $y$ have the same residues, every $m_i$ divides $x-y$. Pairwise coprimality then makes $M$ divide $x-y$. **Thus the simultaneous solution exists and is unique modulo $M$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1G](../../1g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
