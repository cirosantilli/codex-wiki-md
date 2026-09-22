<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $h=x-1/\sqrt2$ and $k=y-1/(2\sqrt2)$. At the expansion point the exponent is one and the [gradient](../../../gradient.md) is $(\sqrt2e,\sqrt2e)$. The first-order [multivariable Taylor expansion](../../../multivariable-taylor-expansion.md) is

$$
\boxed{f=e+\sqrt2e(h+k)+O(h^2+k^2).}
$$

The [directional error of a first-order Taylor approximation](../../../directional-error-of-a-first-order-taylor-approximation.md) is determined by the omitted terms, not just the equal first [partial derivatives](../../../partial-derivative.md). The [Hessian matrix](../../../hessian-matrix.md) at the expansion point is $e\begin{pmatrix}4&2\\2&2\end{pmatrix}$, so

$$
f-e-\sqrt2e(h+k)=e(2h^2+2hk+k^2)+O\bigl((h^2+k^2)^{3/2}\bigr).
$$

For equal small steps along the coordinate axes, the leading error is $2eh^2$ along $x$ and $ek^2$ along $y$. **The error grows faster along the $x$ axis**, although the first-order change in the function is equal along the two axes.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2022](../../2022-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
