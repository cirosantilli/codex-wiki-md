<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the ideal [electric dipole](../../../../../electric-dipole.md) limit with a fixed smooth [electric dipole moment](../../../../../electric-dipole-moment.md) $\mathbf p(t)$, so that $\mathbf r_0(t)=\mathbf p(t)/(2q)$; its required time [derivatives](../../../../../derivative.md) are bounded on the time interval under consideration. Fix $r>0$ and put $\mathbf n=\mathbf r/r$, $t_0=t-r/c$. For $s=+1$ or $-1$, the source position is $s\mathbf p(t)/(2q)$. A [Taylor expansion](../../../../../taylor-expansion.md) of the distance gives

$$
R_s(t_r^s)=\left|\mathbf r-\frac{s\mathbf p(t_r^s)}{2q}\right|
=r-\frac{s\mathbf n\cdot\mathbf p(t_r^s)}{2q}+O(q^{-2}).
$$

Substitute this into the defining equation for [retarded time](../../../../../retarded-time.md):

$$
t_r^s=t_0+\frac{s\mathbf n\cdot\mathbf p(t_r^s)}{2qc}+O(q^{-2}).
$$

Boundedness first implies $t_r^s-t_0=O(q^{-1})$. The [Taylor expansion](../../../../../taylor-expansion.md) $\mathbf p(t_r^s)=\mathbf p(t_0)+O(q^{-1})$ then changes the displayed correction only by $O(q^{-2})$. Hence

$$
\boxed{t_r^+=t_0+\frac{\mathbf p(t_0)\cdot\mathbf r}{2qrc}+O(q^{-2}),\qquad
t_r^-=t_0-\frac{\mathbf p(t_0)\cdot\mathbf r}{2qrc}+O(q^{-2}).}
$$

The nearer positive displacement reduces the propagation distance and consequently increases the [retarded time](../../../../../retarded-time.md). The [Big O notation](../../../../../big-o-notation.md) here is for $q\to\infty$ at a fixed observation event away from the origin. Keeping a fixed smooth $\mathbf p$ is essential: bounded amplitude alone, with arbitrarily increasing time frequency as $q$ varies, would not justify this [Taylor expansion](../../../../../taylor-expansion.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
