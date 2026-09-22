<h1 id="5d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The order of an element $x$ is the least positive integer $d$ such that $x^d=e$, and the order of a finite group is its number of elements.

[Lagrange theorem](../../../../../../lagrange-s-theorem.md) states that if $H\leq G$ and $G$ is finite, then

$$
|H|\mid |G|,
\qquad
|G|=[G:H]|H|.
$$

Indeed, the left cosets of $H$ partition $G$. Multiplication by a coset representative is a bijection from $H$ to each coset, so every coset has $|H|$ elements. Summing over the $[G:H]$ cosets proves the formula.

The cyclic subgroup $\langle x\rangle$ has exactly $d$ elements when $x$ has order $d$. Applying Lagrange to $\langle x\rangle\leq G$ gives

$$
\boxed{\operatorname{ord}(x)\mid |G|}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
