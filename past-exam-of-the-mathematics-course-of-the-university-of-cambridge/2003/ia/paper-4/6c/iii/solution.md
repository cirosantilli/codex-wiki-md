<h1 id="6c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $p\equiv1\pmod4$, part (i) constructs a solution $a=q!$ to $a^2\equiv-1$. It is nonzero modulo $p$, so $a$ and $-a$ are distinct for odd $p$. Any other solution $x$ obeys

$$
(x-a)(x+a)=x^2-a^2\equiv0\pmod p.
$$

The [Euclid lemma](../../../../../../euclid-lemma.md) forces $x\equiv a$ or $-a$. Hence there are exactly two solutions. For $p\equiv3\pmod4$, a solution to $x^2\equiv-1$ would have $x^4\equiv1$, but part (ii) would imply $x^2\equiv1$, impossible because $p$ cannot divide two. Therefore

$$
\boxed{\#\{x\bmod p:x^2\equiv-1\}=\begin{cases}2,&p\equiv1\pmod4,\\0,&p\equiv3\pmod4.\end{cases}}
$$

These two cases exhaust all odd primes.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6C](../../6c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
