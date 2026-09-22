<h1 id="12/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the forward-moving object to have been waiting at the meeting [position](../../../../../position.md), the last move must be a reverse move. The preceding $F-1$ choices must then contain exactly $n$ forward moves and $F-n-1$ reverse moves. Choosing their order gives

$$
\boxed{p_n^{\rm specialMeet}=\binom{F-1}{n}p^nq^{F-n},\qquad 0\leq n\leq F-1.}
$$

At $n=F$ the [probability](../../../../../probability.md) is **zero**, since the reverse-moving object was already at that unwrapped [position](../../../../../position.md) initially. At $n=0$ the displayed formula is $q^F$, consistent with the forward object waiting at its initial [position](../../../../../position.md) throughout. Equivalently, use the binomial convention $\binom{F-1}{F}=0$ to include this endpoint in the same formula without a negative power of $q$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
