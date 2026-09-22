<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With one marked input, after $r$ distinct failed guesses it is uniformly distributed among the $N-r$ untested inputs. Therefore the conditional chance of success on the next guess is $1/(N-r)$. One further failure raises it by

$$
\boxed{\frac1{N-r-1}-\frac1{N-r}=\frac1{(N-r-1)(N-r)},\quad 0\le r\le N-2,}
$$

or by a multiplicative factor $(N-r)/(N-r-1)$. There is a different unconditional statement: the marked position is uniform, so $\mathbb P(K=k)=1/N$ and $\mathbb P(K\le k)=k/N$. Thus each additional distinct guess increases cumulative success by $1/N$, even though the conditional next-guess probability increases after each failure. These distinguish the two possible meanings of a probability boost.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
