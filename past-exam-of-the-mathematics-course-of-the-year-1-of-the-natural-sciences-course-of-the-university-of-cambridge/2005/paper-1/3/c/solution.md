<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The quoted pass probabilities on later attempts are conditional on reaching those attempts. If $K$ is the first successful attempt, then

$$
P(K=1)=\frac35,\quad P(K=2)=\frac25\frac45=\frac8{25},\quad P(K=3)=\frac25\frac15\frac78=\frac7{100}.
$$

They sum to $99/100$, so conditioning on success by the third attempt is essential. The [conditional mean of a bounded success time](../../../../../conditional-mean-of-a-bounded-success-time.md) is

$$
\boxed{\mathbb E[K\mid K\leq3]=\frac{1(3/5)+2(8/25)+3(7/100)}{99/100}=\frac{145}{99}\simeq1.465.}
$$

The remaining probability $1/100$ represents failing all three attempts and is excluded by this conditioning.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
