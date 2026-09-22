<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

The [Wilson theorem](../../../../../wilson-s-theorem.md) says that $(p-1)!\equiv-1\pmod p$ for a [prime number](../../../../../prime-number.md) $p$. Thus $18\cdot17!\equiv-1\pmod{19}$, and since $18\equiv-1$, we get $17!\equiv1$. The [Fermat little theorem](../../../../../fermat-little-theorem.md) says $b^{p-1}\equiv1\pmod p$ when $p$ does not divide $b$. Applying it to $3$ gives $3^{18}\equiv1$, so $3^{16}$ is the inverse of $9$ modulo $19$. Since $9\cdot17=153\equiv1$, the required residue is

$$
\boxed{a=17.}
$$

This is the unique representative in $\{1,\ldots,19\}$.

For the simultaneous [integer congruences](../../../../../integer-congruence.md), the modulus-$2$ condition is already implied by $x\equiv3\pmod4$. Write $x=3+4k$; the modulus-$3$ condition becomes $k\equiv1\pmod3$, hence $x=7+12t$. The modulus-$5$ condition then gives $2+2t\equiv4$, or $t\equiv1\pmod5$. Therefore

$$
\boxed{x=19+60j,\qquad j\in\mathbb Z.}
$$

Every such integer satisfies all four [integer congruences](../../../../../integer-congruence.md); reversing the substitutions shows that there are no others. The uniqueness modulo $60$ also follows from the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) applied to the coprime moduli $3,4,5$.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
