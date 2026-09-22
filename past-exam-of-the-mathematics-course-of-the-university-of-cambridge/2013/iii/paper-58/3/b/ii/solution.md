<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $w$ be the number of ones. The displayed output state assigns the outcome $(0,0)$ probability

$$
\boxed{\Pr(0,0)=\frac{(N-2w)^2}{N^2}.}
$$

For a constant string, $w=0$ or $N$, so this probability is one. For a balanced string, $w=N/2$, so it is zero. Under the promise, **$(0,0)$ certifies a constant string, and any other possible outcome certifies a balanced string.** A nonzero ordered-pair outcome must have $i<j$ and $\widehat x_i-\widehat x_j\ne0$, which also certifies $x_i\ne x_j$ without separately reading either bit. This is the fact used by [opposite-pair elimination for exact quantum balance testing](../../../../../../../opposite-pair-elimination-for-exact-quantum-balance-testing.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 58](../../../../paper-58-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
