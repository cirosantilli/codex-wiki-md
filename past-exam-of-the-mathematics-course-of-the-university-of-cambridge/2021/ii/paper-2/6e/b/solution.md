<h1 id="6e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate $\langle f(n)\rangle=\sum_{n\geq0}f_np_n$ and substitute the three master equations. Reindexing every gain term by its source state gives one contribution per possible transition:

$$
\begin{aligned}
\frac d{dt}\langle f(n)\rangle
={}&b\sum_{n=0}^\infty(f_{n+1}-f_n)p_n\\
&-d\sum_{n=2}^\infty(f_n-f_{n-2})np_n
-D(f_1-f_0)p_1.
\end{aligned}
$$

This is the [generator identity for a continuous-time Markov chain](../../../../../../markov-jump-process-generator.md) applied to the test function $f$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6E](../../6e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
