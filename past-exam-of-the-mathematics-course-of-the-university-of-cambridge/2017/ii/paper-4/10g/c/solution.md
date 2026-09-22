<h1 id="10g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Both forms have [discriminant of a binary quadratic form](../../../../../../discriminant-of-a-binary-quadratic-form.md) $-60$. The [reduction algorithm for a positive definite binary quadratic form](../../../../../../reduction-algorithm-for-a-positive-definite-binary-quadratic-form.md) gives $|b|\leq a\leq c$ and $a\leq\sqrt{60/3}<5$ for a reduced positive definite representative. Enumerating $a=1,2,3,4$ gives

$$
[1,0,15],\quad[2,2,8],\quad[3,0,5],\quad[4,2,4].
$$

The second and fourth forms are imprimitive and represent only even [integers](../../../../../../integer.md). Every odd [prime](../../../../../../prime-number.md) represented by a form of [discriminant of a binary quadratic form](../../../../../../discriminant-of-a-binary-quadratic-form.md) $-60$ must therefore be represented by $f$ or $g$.

For a [prime](../../../../../../prime-number.md) $p\nmid30$, [quadratic reciprocity](../../../../../../quadratic-reciprocity.md) gives

$$
\left(\frac{-60}{p}\right)=\left(\frac{-3}{p}\right)\left(\frac5p\right)
=\left(\frac p3\right)\left(\frac p5\right).
$$

Every [prime](../../../../../../prime-number.md) $p\equiv1\pmod{15}$ has this symbol equal to one and hence is represented by one of the two primitive forms, by part (b). But an odd [prime](../../../../../../prime-number.md) represented by $g$ and different from three is $2\pmod3$, so these [primes](../../../../../../prime-number.md) must be represented by $f$. Similarly, [primes](../../../../../../prime-number.md) $p\equiv2\pmod{15}$ have both symbols equal to $-1$, and are represented by $g$, since a [prime](../../../../../../prime-number.md) represented by $f$ is $1\pmod3$. Both [residue classes](../../../../../../residue-class.md) are [coprime](../../../../../../coprime-integers.md) to 15, so [Dirichlet theorem on primes in arithmetic progressions](../../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md) proves **each form represents infinitely many [primes](../../../../../../prime-number.md)**.

The same modulo-three distinction excludes every [prime](../../../../../../prime-number.md) other than three from being represented by both. The form $f$ does not represent three; $g$ represents three and five but neither is represented by $f$, and two is represented by neither. Therefore **there are no [primes](../../../../../../prime-number.md) represented by both forms**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10G](../../10g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
