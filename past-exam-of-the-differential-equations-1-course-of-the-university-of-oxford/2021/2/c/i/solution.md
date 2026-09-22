<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat both sides of $a$ at once: for $\sigma\in\{-1,1\}$ set $w(t)=v(a+\sigma t)$, $0\leq t\leq h$. Nonnegativity gives

$$
\left|\int_a^{a+\sigma t}v(s)\,ds\right|=\int_0^t w(r)\,dr,
\qquad w(t)\leq ct+A\int_0^t w(r)\,dr.
$$

Define $W(t)=ct+A\int_0^t w(r)\,dr$. By the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md), $W'(t)=c+Aw(t)\leq c+AW(t)$ and $W(0)=0$. The [integrating factor](../../../../../integrating-factor.md) $e^{-At}$ gives

$$
\frac{d}{dt}(e^{-At}W(t))\leq ce^{-At},\qquad
W(t)\leq\frac{c}{A}(e^{At}-1).
$$

Since $w\leq W$, this proves the [affine Gronwall estimate](../../../../../affine-gronwall-estimate.md)

$$
\boxed{v(x)\leq\frac{c}{A}\bigl(e^{A|x-a|}-1\bigr),\qquad |x-a|\leq h.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
