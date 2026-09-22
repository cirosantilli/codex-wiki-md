<h1 id="13e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The string is initially at rest, so $y(x,0)=y_t(x,0)=0$. Taking the [Laplace transform](../../../../../../laplace-transform.md) in $t$ converts the [wave equation](../../../../../../wave-equation-split.md) into

$$
p^2\widehat y=c^2\frac{\partial^2\widehat y}{\partial x^2}.
$$

For $\operatorname{Re}p>0$, the solution that decays as $x\to\infty$ is $\widehat y=A(p)e^{-px/c}$. The transformed boundary condition $\widehat y(0,p)=\widehat f(p)$ fixes $A=\widehat f$, and therefore

$$
\boxed{\widehat y(x,p)=\widehat f(p)e^{-px/c}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [13E](../../13e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
