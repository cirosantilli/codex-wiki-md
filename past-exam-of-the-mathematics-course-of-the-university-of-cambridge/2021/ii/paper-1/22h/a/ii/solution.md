<h1 id="22h/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Conversely, suppose

$$
\|x_n\|\leq C
$$

and define

$$
a_i=\lim_{n\to\infty}\langle x_n,e_i\rangle.
$$

For every $N$, [Bessel inequality](../../../../../../../bessel-s-inequality.md) and passage to the limit give

$$
\sum_{i=1}^N|a_i|^2
=\lim_{n\to\infty}
\sum_{i=1}^N|\langle x_n,e_i\rangle|^2
\leq C^2.
$$

Hence $\sum_i|a_i|^2\leq C^2$. The partial sums $\sum_{i=1}^Na_ie_i$ are therefore Cauchy; completeness of the [Hilbert space](../../../../../../../hilbert-space-split.md) gives an element

$$
x_\infty=\sum_{i=1}^{\infty}a_ie_i,
\qquad
\|x_\infty\|\leq C.
$$

Let $P_Nh=\sum_{i=1}^N\langle h,e_i\rangle e_i$. For fixed $N$, coordinate convergence gives

$$
\langle x_n-x_\infty,P_Nh\rangle\longrightarrow0.
$$

The [Hilbertian basis](../../../../../../../hilbertian-basis.md) property gives $P_Nh\to h$, and

$$
|\langle x_n-x_\infty,h-P_Nh\rangle|
\leq(\|x_n\|+\|x_\infty\|)\|h-P_Nh\|
\leq2C\|h-P_Nh\|.
$$

First choose $N$ large and then $n$ large. This proves

$$
\langle x_n,h\rangle\longrightarrow\langle x_\infty,h\rangle
$$

for every $h\in H$, so $x_n\rightharpoonup x_\infty$. This establishes the [coordinate criterion for weak convergence in a separable Hilbert space](../../../../../../../coordinate-criterion-for-weak-convergence-in-a-separable-hilbert-space.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [22H](../../../22h.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
