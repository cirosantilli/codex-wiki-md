<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The smallest integer is

$$
k=2.
$$

Indeed, reduction modulo $p$ cannot work: the map $x\mapsto x^p$ is the identity on $\mathbb F_p^\times$, although not every element of $\mathbb Z_p^\times$ is a $p$th power.

For odd $p$, the [p-adic unit group](../../../../../../p-adic-unit.md) decomposes as

$$
\mathbb Z_p^\times\cong\mu_{p-1}\times(1+p\mathbb Z_p).
$$

Raising to the $p$th power is an automorphism on $\mu_{p-1}$. On the principal units, the [p-adic logarithm](../../../../../../p-adic-logarithm.md) identifies it with multiplication by $p$ on $p\mathbb Z_p$, so

$$
(1+p\mathbb Z_p)^p=1+p^2\mathbb Z_p.
$$

Hence whether a unit is a $p$th power is determined exactly by its residue modulo $p^2$. Equivalently,

$$
\alpha\in(\mathbb Z_p^\times)^p
\quad\Longleftrightarrow\quad
\alpha\bmod p^2\in((\mathbb Z/p^2\mathbb Z)^\times)^p.
$$

This is the [pth-power criterion for p-adic units](../../../../../../pth-power-criterion-for-p-adic-units.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
