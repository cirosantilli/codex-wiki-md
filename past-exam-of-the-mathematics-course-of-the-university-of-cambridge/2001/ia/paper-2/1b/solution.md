<h1 id="1b/solution">Solution</h1>

↑ **Parent:** [1B](../1b.md)

An [integrating factor](../../../../../integrating-factor.md) is $\mu(x)=\cosh x$, since $\mu'/\mu=\tanh x$. Thus

$$
(\cosh x\,y)'=\cosh x\,H(x),\qquad
\cosh x\,y(x)=1+\int_0^x\cosh t\,H(t)\,dt.
$$

For negative $x$ the integral vanishes; for positive $x$ it is $\sinh x$. Consequently

$$
\boxed{y(x)=\begin{cases}
\operatorname{sech}x,&x\le0,\\
\operatorname{sech}x+\tanh x,&x\ge0.
\end{cases}}
$$

Both branches give $y(0)=1$. This is [Heaviside forcing in a first-order integrating-factor equation](../../../../../heaviside-forcing-in-a-first-order-integrating-factor-equation.md): the solution is continuous and piecewise differentiable, while its one-sided derivatives at zero are $0$ and $1$. The [Heaviside step function](../../../../../heaviside-step-function.md)'s value at zero does not affect the integral solution. The equation holds classically on the two open half-lines and in the weak sense across zero.

The left branch rises from zero at $-\infty$ to one. On the right,

$$
y'(x)=\frac{1-\sinh x}{\cosh^2x},
$$

so its unique maximum is **$y=\sqrt2$ at $x=\operatorname{arsinh}1$**, after which it decreases to the horizontal asymptote $y=1$ from above.

<a id="1b/image-continuous-step-forced-solution-with-its-derivative-jump-maximum-and-asymptotes"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-2-step-solution.png)

**[Figure 1](#1b/image-continuous-step-forced-solution-with-its-derivative-jump-maximum-and-asymptotes). Continuous step-forced solution with its derivative jump, maximum and asymptotes**.

## ↑ Ancestors (10)

1. [1B](../1b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
