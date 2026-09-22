<h1 id="b/5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a smooth solution, the first equation is $u_x+(uv)_y=0$. Multiplying it by $v$ and adding $u$ times the second equation gives

$$
(uv)_x+\bigl(uv^2+\tfrac12u^2\bigr)_y=0.
$$

Thus the appropriate [shallow water equations](../../../../../../shallow-water-equations.md) conservation variables and [flux](../../../../../../flux.md) are

$$
W=\begin{pmatrix}u\\uv\end{pmatrix},\qquad H(W)=\begin{pmatrix}uv\\uv^2+u^2/2\end{pmatrix}.
$$

Use this conservative extension to define a [weak solution](../../../../../../weak-solution.md) across $y=F(x)$. A jump contributes $-F'[W]\delta(y-F(x))$ to $W_x$ and $[H]\delta(y-F(x))$ to $H_y$. Cancellation of the singular parts gives the [Rankine-Hugoniot conditions](../../../../../../rankine-hugoniot-conditions.md)

$$
\boxed{F'(x)\begin{pmatrix}[u]\\{[uv]}\end{pmatrix}=\begin{pmatrix}[uv]\\{[uv^2+u^2/2]}\end{pmatrix}.}
$$

Equivalently this follows by integrating each [conservation law](../../../../../../conservation-law.md) over a thin space-time control region crossing the discontinuity.

The conservative extension is essential here. Piecewise smoothness by itself does not imply any jump law. Moreover the smooth second equation can also be written $v_x+(u+v^2/2)_y=0$; imposing that different [conservation law](../../../../../../conservation-law.md) distributionally would give a different [shock](../../../../../../shock-wave.md) condition. [Weak conservation laws depend on conserved variables](../../../../../../weak-conservation-laws-depend-on-conserved-variables.md). The requested jump law specifically selects [mass](../../../../../../mass.md) $u$ and [momentum](../../../../../../momentum-split.md) $uv$, and this is the extension used below.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the differential equations and applications course of the University of Oxford](../../../../../split.md)
7. [Differential equations and applications course of the University of Oxford](../../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
