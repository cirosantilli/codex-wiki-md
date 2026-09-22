<h1 id="9e/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Urn $r$ has $n-r$ blue balls among $n-1$ balls. Averaging over the uniformly chosen urn,

$$
\mathbb P(\text{first blue})
=\frac1n\sum_{r=1}^n\frac{n-r}{n-1}
=\boxed{\frac12}.
$$

The probability that both removed balls are blue is

$$
\begin{aligned}
\mathbb P(B_1\cap B_2)
&=\frac1n\sum_{r=1}^n
\frac{(n-r)(n-r-1)}{(n-1)(n-2)}\\
&=\frac13.
\end{aligned}
$$

Therefore

$$
\boxed{
\mathbb P(B_2\mid B_1)
=\frac{\mathbb P(B_1\cap B_2)}{\mathbb P(B_1)}
=\frac23}.
$$

The first blue draw makes urns with more blue balls more likely, which explains why the conditional probability exceeds one half.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [9E](../../../9e.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
