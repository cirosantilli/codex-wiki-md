<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On an [interval](../../../../interval-mathematics.md) with $x>0$, use the [power-law ansatz](../../../../power-law-ansatz.md) $y=x^r$. Substitution gives $r(r-1)+2r+1=r^2+r+1=0$, whose roots are $r=-1/2\pm i\sqrt3/2$. Taking real and imaginary parts of $x^r$ gives

$$
\boxed{y(x)=x^{-1/2}\left[C_1\cos\left(\frac{\sqrt3}{2}\log x\right)+C_2\sin\left(\frac{\sqrt3}{2}\log x\right)\right].}
$$

These two real solutions are [linearly independent](../../../../linear-independence.md): their [Wronskian](../../../../wronskian.md) is $(\sqrt3/2)x^{-2}\ne0$. They therefore span the solution space of the second-order [linear ordinary differential equation](../../../../linear-ordinary-differential-equation-split.md) on that [interval](../../../../interval-mathematics.md).

For $x<0$, replace $x^{-1/2}$ by $|x|^{-1/2}$ and $\log x$ by $\log|x|$, with independent real constants on the negative [interval](../../../../interval-mathematics.md). This follows equally by the change of variable $t=\log|x|$, which turns the [Cauchy-Euler equation](../../../../cauchy-euler-equation.md) into $d^2y/dt^2+dy/dt+y=0$. The [coefficient](../../../../coefficient.md) of $y''$ vanishes at zero, so the general formula is stated separately on either side. Every nonzero mode has an unbounded oscillatory envelope as $x\to0$; a continuous extension through zero requires the solution to vanish identically on both sides.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
