<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The characteristic polynomial is $(r+\gamma)^2+c^2k^2$, with roots $r=-\gamma\pm ick$. For $ck\ne0$, the transformed general solution is

$$
\boxed{\widetilde u(k,t)=e^{-\gamma t}\big[A(k)e^{-ickt}+B(k)e^{ickt}\big].}
$$

The repeated-root case $ck=0$ is $e^{-\gamma t}[A_0+B_0t]$, rather than two independent copies of the same exponential. An alternative basis regular at $k=0$ is $e^{-\gamma t}[C(k)\cos(ckt)+D(k)\sin(ckt)/(ck)]$, using the limit $t$ for the last factor at zero.

For $c\ne0$, the [Fourier shift theorem](../../../../../fourier-shift-theorem.md) turns the two exponential factors into translations. Equivalently, set $v=e^{\gamma t}u$; then $v_{tt}=c^2v_{xx}$. The [D'Alembert formula](../../../../../d-alembert-s-formula.md) gives the general form

$$
\boxed{u(x,t)=e^{-\gamma t}[F(x-|c|t)+G(x+|c|t)],\qquad c\ne0,}
$$

where $F,G$ are arbitrary functions with the required regularity and decay. The arbitrary profiles can accommodate a spatially transformed zero-frequency velocity by their integral components; the isolated repeated root must not be used to discard that degree of freedom. If $c=0$, the equation instead has $u=e^{-\gamma t}[F(x)+tG(x)]$.

This is the [exponentially conjugated wave equation](../../../../../exponentially-conjugated-wave-equation.md). Positive $\gamma$ produces damping, but the algebra also covers negative $\gamma$, which gives exponential amplification. The sign of $c$ is immaterial because the differential equation contains only $c^2$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
