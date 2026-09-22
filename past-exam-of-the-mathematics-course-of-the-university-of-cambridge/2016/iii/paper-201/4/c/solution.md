<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every $w\in C^\alpha[0,1]$, its finite [Hölder seminorm](../../../../../../holder-seminorm.md) gives the deterministic bound

$$
\sum_{k=0}^{2^n-1}\bigl(w((k+1)2^{-n})-w(k2^{-n})\bigr)^2
\leq2^n\|w\|_\alpha^2\,2^{-2n\alpha}
=\|w\|_\alpha^2\,2^{n(1-2\alpha)}.
$$

When $\alpha>1/2$, the right-hand side tends to zero. Thus under any [probability measure](../../../../../../probability-measure.md) on the stated [coordinate sigma-algebra](../../../../../../cylinder-sigma-algebra.md), these measurable finite-coordinate sums converge to zero on every path, and hence almost surely.

If the coordinate process were a [Brownian motion](../../../../../../brownian-motion-split.md), part (b) would make the same sums converge to one in $L^2$, and hence in probability. [Almost sure convergence](../../../../../../almost-sure-convergence.md) to zero also implies [convergence in probability](../../../../../../convergence-in-probability.md) to zero. Uniqueness of a limit in probability is a contradiction. Therefore **no such Brownian measure exists**:

$$
\boxed{\alpha>\tfrac12\quad\Longrightarrow\quad\text{no Brownian coordinate law on }C^\alpha[0,1].}
$$

This is the [quadratic variation obstruction to Hölder regularity](../../../../../../quadratic-variation-obstruction-to-holder-regularity.md). It does not address the critical exponent $\alpha=1/2$, where the displayed deterministic bound does not tend to zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
