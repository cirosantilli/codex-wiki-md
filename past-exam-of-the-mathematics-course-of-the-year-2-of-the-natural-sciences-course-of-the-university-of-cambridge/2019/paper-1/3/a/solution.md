<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each source point $z$, construct the [Green function](../../../../../green-s-function-split.md) from homogeneous solutions on either side:

$$
G(x,z)=\begin{cases}A(z)y_a(x),&a\leq x<z,\\B(z)y_b(x),&z<x\leq b.\end{cases}
$$

The endpoint conditions are then automatic. The equation $L_xG=\delta(x-z)$ requires continuity of $G$ and a unit jump in its first [derivative](../../../../../derivative.md): a discontinuity in $G$ would introduce an unwanted delta [derivative](../../../../../derivative.md), while integrating across the source fixes $G_x(z^+,z)-G_x(z^-,z)=1$. Thus

$$
A y_a(z)=B y_b(z),\qquad B y_b'(z)-A y_a'(z)=1.
$$

Solving this two-by-two system, with the [Wronskian](../../../../../wronskian.md) $W=y_a y_b'-y_b y_a'\ne0$, gives

$$
\boxed{G(x,z)=\begin{cases}y_a(x)y_b(z)/W(z),&a\leq x\leq z,\\y_b(x)y_a(z)/W(z),&z\leq x\leq b.\end{cases}}
$$

This derivation also remains valid if one of the solution values at the matching point vanishes: only the [Wronskian](../../../../../wronskian.md) must be nonzero. For a regular nonsingular two-point problem it supplies the inverse kernel; at a singular endpoint, uniqueness requires separate checking, as part (d) illustrates.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
