<h1 id="5e/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let

$$
l=\operatorname{ord}_p(10).
$$

By Fermat's little theorem, $l\mid p-1$. If the digit count $L$ is a multiple of $l$, then $10^L\equiv1\pmod p$. The [cyclic decimal divisibility](../../../../../../cyclic-decimal-divisibility.md) relation gives

$$
c_j(n)\equiv10^jn\pmod{10^L-1},
$$

and hence also modulo $p$. Since $p>7$ is coprime to $10$, every $10^j$ is a unit modulo $p$. Therefore

$$
p\mid c_j(n)\quad\Longleftrightarrow\quad p\mid n
$$

for every $j$. Since $c_0(n)=n$, this proves the required equivalence.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
