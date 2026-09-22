<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Now the inverse integrand can be written

$$
\lambda^{-s}H(s)=\frac{e^{s\log(1/(2\lambda))}}{2(s+1)},\qquad\gamma>-1.
$$

For $0<\lambda<1/2$, the exponent has a positive real time parameter. Close the [Bromwich contour](../../../../../bromwich-contour.md) to the left; the [residue](../../../../../residue.md) at $s=-1$ is $\tfrac12(2\lambda)=\lambda$. For $1/2<\lambda<1$, close to the right, where there are no [poles](../../../../../pole.md). The reversed orientation there still gives zero. Consequently

$$
\boxed{h(\lambda)=\begin{cases}\lambda,&0<\lambda<\tfrac12,\\0,&\tfrac12<\lambda<1.\end{cases}}
$$

The same result follows from the [Laplace transform time-shift rule](../../../../../laplace-transform-time-shift-rule.md): $H(s)=\tfrac12e^{-s\log2}/(s+1)$ corresponds to $f(t)=e^{-t}\Theta(t-\log2)$, where $\Theta$ is the [Heaviside step function](../../../../../heaviside-step-function.md).

The original transform cannot fix a value at the single point $\lambda=1/2$. The [Bromwich inversion formula](../../../../../bromwich-inversion-formula.md) chooses the average of the limiting values $1/2$ and zero, giving $\boxed{h(1/2)=1/4}$ under that convention. Indeed,

$$
\int_0^1\lambda^{s-1}h(\lambda)\,d\lambda=\int_0^{1/2}\lambda^s\,d\lambda=\frac{2^{-s-1}}{s+1},\qquad\operatorname{Re}s>-1,
$$

regardless of the assigned value at the jump.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
