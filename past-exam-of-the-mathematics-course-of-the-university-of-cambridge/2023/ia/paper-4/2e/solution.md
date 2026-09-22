<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) says that for pairwise coprime positive integers $m_i$, the map

$$
\mathbb Z/(m_1\cdots m_r)\mathbb Z
\longrightarrow\prod_i\mathbb Z/m_i\mathbb Z
$$

is a bijection. For two [moduli](../../../../../modulus.md), choose $u,v$ with $um+vn=1$; then

$$
x=b,um+a,vn
$$

has residues $a$ modulo $m$ and $b$ modulo $n$. Uniqueness follows because the difference of two solutions is divisible by both coprime [moduli](../../../../../modulus.md), hence by their product. Induction proves the general case.

The two given congruences are compatible modulo $\gcd(6,8)=2$, and checking modulo $\operatorname{lcm}(6,8)=24$ gives

$$
x\equiv10\pmod{24}.
$$

Write $d=2^r3^sm$ with $(m,6)=1$. Use the Chinese remainder theorem to choose

$$
a\equiv0\pmod{2^r},\qquad 2a\equiv1\pmod{3^sm},
$$



$$
3b\equiv1\pmod{2^r},\qquad b\equiv0\pmod{3^sm}.
$$

Then $4a^2+9b^2\equiv1$ modulo each of the pairwise coprime factors $2^r$, $3^s$, and $m$, hence modulo $d$.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
