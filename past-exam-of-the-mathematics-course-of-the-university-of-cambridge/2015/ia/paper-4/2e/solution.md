<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) says that for pairwise [coprime integers](../../../../../coprime-integers.md) $m_1,\ldots,m_r>0$, any prescribed residue modulo each $m_i$ is realized by exactly one residue class modulo $\prod_i m_i$. The [Fermat little theorem](../../../../../fermat-little-theorem.md) says that for a [prime number](../../../../../prime-number.md) $q$ and an [integer](../../../../../integer.md) $a$ not divisible by $q$, $a^{q-1}\equiv1\pmod q$; equivalently, $a^q\equiv a\pmod q$ for every [integer](../../../../../integer.md) $a$.

For the given [prime number](../../../../../prime-number.md), write $p=2k+1$. Its square is $p^2=1+4k(k+1)=1+8t$ for some [integer](../../../../../integer.md) $t$, since one of two consecutive [integers](../../../../../integer.md) is even. Therefore $p^4=(1+8t)^2\equiv1\pmod{16}$. The [Fermat little theorem](../../../../../fermat-little-theorem.md) applied modulo $3$ gives $p^2\equiv1\pmod3$, hence $p^4\equiv1\pmod3$; applied modulo $5$ it gives $p^4\equiv1\pmod5$. These applications are valid because $p>5$.

The three moduli $16,3,5$ are pairwise [coprime integers](../../../../../coprime-integers.md) and have product $240$. By the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md),

$$
\boxed{p^4\equiv1\pmod{240}.}
$$

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
