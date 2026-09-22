<h1 id="20h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Measure vertices by their [Hamming distance](../../../../../../hamming-distance.md) from the target and let $h_k$ be the expected hitting time when that distance is $k$. We already know $h_1=2^n-1$. From distance one, one of the $n$ coordinate flips reaches the target and the other $n-1$ flips move to distance two. [First-step analysis](../../../../../../first-step-analysis.md) therefore gives

$$
h_1=1+\frac1n h_0+\frac{n-1}{n}h_2,
\qquad h_0=0.
$$

For $n\geq2$,

$$
\boxed{h_2=\frac{n}{n-1}(h_1-1)
=\frac{n(2^n-2)}{n-1}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
