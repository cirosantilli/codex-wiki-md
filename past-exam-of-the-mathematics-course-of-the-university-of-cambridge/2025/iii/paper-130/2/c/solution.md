<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Restrict the coloring to the diagonal by setting $d(n)=c(n,n)$. We give the direct focusing proof of a monochromatic three-term [arithmetic progression](../../../../../../arithmetic-progression.md). For each $1\leq s\leq k$, induction constructs a finite interval in which either there is a monochromatic three-term progression or there are $s$ [color-focused](../../../../../../color-focused-arithmetic-progression.md) two-term progressions. The case $s=1$ is the [pigeonhole principle](../../../../../../pigeonhole-principle.md). For the induction step, take sufficiently many equal blocks that two have identical color patterns. Translate the $s-1$ focused pairs in the first block to the second and join corresponding points. These give $s-1$ focused pairs at a translated focus; the pair formed by the old and translated focuses supplies the last one. If its color repeated one of the previous colors, the associated pair and the focus would already form a monochromatic three-term progression. Thus the alternative holds.

At $s=k$, the common focus has one of the $k$ colors and completes the pair of that color, so there are $a,r>0$ with $d(a)=d(a+r)=d(a+2r)$. Therefore

$$
(a,a),(a+r,a+r),(a+2r,a+2r)
$$

is the required monochromatic two-dimensional progression. This proves the result without invoking the [Van der Waerden theorem](../../../../../../van-der-waerden-theorem.md) as a black box.

## ↑ Ancestors (11)

1. [C](../c.md)
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
