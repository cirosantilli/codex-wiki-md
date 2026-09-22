<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Normalize the [surface area](../../../../../../surface-area.md) of the [spherical cap](../../../../../../spherical-cap.md) by writing

$$
q(\rho)=\frac{\operatorname{Vol}_{n-1}(D_\rho)}{s_{n-1}},\qquad c_n=\frac{v_{n-1}}{nv_n}.
$$

Two elementary descriptions of a [spherical cap](../../../../../../spherical-cap.md) are useful. The [spherical polar coordinates](../../../../../../spherical-coordinate-system.md) formula gives

$$
q'(\rho)=(n-1)c_n\sin^{n-2}\rho,\qquad q(\pi/2)=\frac12.
$$

Projecting orthogonally onto the last $n-1$ coordinates gives

$$
q(\rho)\leq c_n\frac{\sin^{n-1}\rho}{\cos\rho}.
$$

Indeed, the upper [hemisphere](../../../../../../hemisphere.md) is the graph $x_1=\sqrt{1-\lVert x'\rVert^2}$, whose [surface area](../../../../../../surface-area.md) factor is $(1-\lVert x'\rVert^2)^{-1/2}\leq1/\cos\rho$ on $\lVert x'\rVert\leq\sin\rho$. This establishes the upper projection bound directly.

Set $F(\rho)=\sin^n\rho-q(\rho)$. The supplied ratio bound implies $c_n<\sqrt{(n+1)/(2\pi)}/n\leq1/2$ for $n\geq2$. Consequently, at $\rho=\pi/4$,

$$
q(\pi/4)\leq2c_n\,2^{-n/2}\leq2^{-n/2},\qquad F(\pi/4)\geq0.
$$

Also,

$$
F'(\rho)=\sin^{n-2}\rho\bigl(n\sin\rho\cos\rho-(n-1)c_n\bigr).
$$

On $[\pi/4,\pi/2]$, the expression in parentheses is strictly decreasing; it starts positive and ends negative. Thus $F$ first increases and then decreases, so its minimum on this interval is at an endpoint. Since $F(\pi/2)=1/2$, both endpoint values are nonnegative. **The [spherical cap area upper bound](../../../../../../spherical-cap-area-upper-bound.md) follows:**

$$
\boxed{\operatorname{Vol}_{n-1}(D_\rho)\leq\sin^n\rho\,s_{n-1}\qquad(\pi/4\leq\rho<\pi/2).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
