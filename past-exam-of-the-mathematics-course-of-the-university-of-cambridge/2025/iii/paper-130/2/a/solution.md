<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Hales-Jewett theorem](../../../../../../hales-jewett-theorem.md) states that for positive integers $m,k$ there is $N$ such that every $k$-coloring of the words $[m]^N$ contains a monochromatic [combinatorial line](../../../../../../combinatorial-line.md).

Here is the standard focused-line proof. Induct on the alphabet size $m$, the case $m=1$ being immediate. Assume the result for $m-1$ and every number of colors. For $1\leq s\leq k$, prove inductively that some dimension has the following alternative: either there is a monochromatic combinatorial line, or there are $s$ color-focused lines, meaning that the lines without their common focus are monochromatic in $s$ distinct colors. For $s=1$, restrict to words on $[m-1]$ and use the induction hypothesis on $m$.

For the step from $s-1$ to $s$, let $n$ work for $s-1$ and view a longer word as $(a,b)\in[m]^n\times[m]^M$. Color each $b\in[m-1]^M$ by the complete pattern

$$
(c(a,b))_{a\in[m]^n},
$$

which uses at most $k^{m^n}$ colors. Taking $M=HJ(m-1,k^{m^n})$ gives a line on which this entire pattern is constant. Append its missing $m$-letter endpoint. Applying the $s-1$ alternative to the induced coloring of the first block and joining the active coordinate sets produces either a monochromatic line or $s$ lines with one common focus and distinct colors. At $s=k$, the focus has one of the $k$ colors, so it completes the line carrying that color. This proves the theorem.

To deduce the [Van der Waerden theorem](../../../../../../van-der-waerden-theorem.md), let $N=HJ(m,k)$ and color a word $(x_1,\ldots,x_N)\in[m]^N$ by the color of $x_1+\cdots+x_N$. On a combinatorial line with active set $I$, these sums are

$$
A+|I|,A+2|I|,\ldots,A+m|I|,
$$

a monochromatic [arithmetic progression](../../../../../../arithmetic-progression.md) of length $m$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
