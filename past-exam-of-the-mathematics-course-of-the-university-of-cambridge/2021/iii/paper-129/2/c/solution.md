<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a [Regular Bohr set](../../../../../../regular-bohr-set.md) $B'=B_\lambda\subseteq B$ with $1/2\leq\lambda\leq1$. Standard Bohr-set size estimates give $|B'|\geq2^{-O(d)}|B|$. Set $\eta=c_0/d$ with $c_0$ small enough that regularity gives

$$
|B'_{1-\eta}|\geq\frac12|B'|.
$$

For each $z\in B'_\eta$ and $y\in B'_{1-\eta}$, the triangle inequality in every frequency gives

$$
z-y,\ z, z+y\in B'.
$$

Because $|G|$ is odd, multiplication by two is a bijection, and the pair $(z,y)$ determines the ordered three-term [arithmetic progression](../../../../../../arithmetic-progression.md) uniquely. The lower size bound for a [Dilate of a Bohr set](../../../../../../dilate-of-a-bohr-set.md) gives

$$
|B'_\eta|\geq(\eta/8)^d|G|\geq(cd)^{-O(d)}|B'|.
$$

The number of progressions in $B$ is therefore at least

$$
\boxed{|B'_\eta|\,|B'_{1-\eta}|
\geq(cd)^{-O(d)}|B'|^2
\geq(cd)^{-O(d)}|B|^2.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
