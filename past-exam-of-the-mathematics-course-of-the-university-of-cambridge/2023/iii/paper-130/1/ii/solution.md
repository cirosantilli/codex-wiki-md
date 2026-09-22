<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the given coloring use $k$ colors, and choose $N$ from the [Extended Hales-Jewett theorem](../../../../../../extended-hales-jewett-theorem.md) for alphabet $\{0,1\}$ and dimension $n$. Color a word $w\in\{0,1\}^N$ by the color of the [positive integer](../../../../../../positive-integer.md)

$$
\Phi(w)=1+\sum_{j=1}^N 2^{j-1}w_j.
$$

A monochromatic $n$-parameter set has disjoint active coordinate sets $I_1,\ldots,I_n$ and fixed letters outside their union. Put

$$
a=1+\sum_{j\notin I_1\cup\cdots\cup I_n}2^{j-1}w_j,
\qquad
x_s=\sum_{j\in I_s}2^{j-1}.
$$

Every $x_s$ is positive. As the $n$ independent variable letters range over zero and one, their images under $\Phi$ are precisely

$$
\left\{a+\sum_{s\in J}x_s:J\subseteq[n]\right\}.
$$

All these integers have one color, so they form the required monochromatic [Hilbert cube](../../../../../../hilbert-cube.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
