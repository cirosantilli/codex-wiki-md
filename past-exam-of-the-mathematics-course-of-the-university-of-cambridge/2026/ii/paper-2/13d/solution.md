<h1 id="13d/solution">Solution</h1>

↑ **Parent:** [13D](../13d.md)

A [branch point](../../../../../branch-point.md) is a point around which analytic continuation changes a value; a branch cut removes curves so continuation becomes single-valued, and a branch is one such single-valued analytic choice. Define

$$
\operatorname{Arcsin}z=\int_0^z(1-t^2)^{-1/2}dt
$$

on $\mathbb C\setminus((-∞,-1]\cup[1,∞))$, choosing the square root equal to $1$ at zero. Monodromy around $\pm1$ explains multivaluedness.

On the upper lip $0+$ of the cut convention, the branch remains positive on $(0,1)$, so $\int_{0+}^1dt/\sqrt{1-t^2}=\pi/2$. Define $\operatorname{Arccos}z=\pi/2-\operatorname{Arcsin}z$ on the same slit domain.

Also

$$
\arctan z=\frac1{2i}[\log(1+iz)-\log(1-iz)].
$$

Changing logarithm branches changes the value by multiples of $\pi$ (already visible at $z=1$). Principal logarithms give a single branch on the plane cut from $\pm i$ outward. Differentiating both sides and checking the value at zero proves

$$
\operatorname{Arctan}z=\operatorname{Arcsin}\frac z{\sqrt{1+z^2}}
$$

where the compatible principal branches are defined.

## ↑ Ancestors (10)

1. [13D](../13d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
