<h1 id="11i/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Suppose first that $b$ is not primitive modulo $p^2$. Since it is primitive modulo $p$, its order modulo $p^2$ is then $p-1$, so

$$
b^{p-1}\equiv1\pmod{p^2}.
$$

Because $p-1$ divides $p^2-1$, the composite number $p^2$ satisfies

$$
b^{p^2-1}\equiv1\pmod{p^2};
$$

it is a [Fermat pseudoprime](../../../../../../../fermat-pseudoprime.md) to base $b$ and is divisible by $p^2$. Thus (iii) fails.

Conversely, suppose $b$ is primitive modulo $p^2$ and a base-$b$ pseudoprime $N$ is divisible by $p^a$ with $a\geq2$. By part (i),

$$
\operatorname{ord}_{p^a}(b)=p^{a-1}(p-1).
$$

The pseudoprime congruence forces this order to divide $N-1$, so in particular $p\mid N-1$. But $p\mid N$, a contradiction. Hence no such pseudoprime exists. This proves (i)$\Leftrightarrow$(iii), and all three statements are equivalent.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [11I](../../../11i.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
