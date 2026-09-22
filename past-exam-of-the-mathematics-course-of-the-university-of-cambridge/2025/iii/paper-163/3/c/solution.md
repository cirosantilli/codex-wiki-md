<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The three unit normals of any selected blocks remain uniformly linearly independent. Hence the intersection of three thickness-one slabs with these normals has bounded volume, and therefore

$$
|S_1\cap S_2\cap S_3\cap B_r|\lesssim1.
$$

Expanding the cube of the requested $L^3$ norm and using nonnegativity gives

$$
\begin{aligned}
\left\|\prod_{j=1}^3\left(\sum_{S_j}c_{S_j}\chi_{S_j}\right)^{1/3}\right\|_{L^3(B_r)}^3
&=\sum_{S_1,S_2,S_3}c_{S_1}c_{S_2}c_{S_3}|S_1\cap S_2\cap S_3\cap B_r|\\
&\lesssim\prod_{j=1}^3\sum_{S_j\in\mathcal S_j}c_{S_j}.
\end{aligned}
$$

Taking cube roots proves the estimate with a constant independent of $r$, which is stronger than the allowed factor $C_\epsilon r^\epsilon$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 163](../../../paper-163-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
