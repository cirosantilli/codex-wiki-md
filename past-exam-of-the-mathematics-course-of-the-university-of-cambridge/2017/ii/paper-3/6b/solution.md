<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

In the [birth-death master equation](../../../../../birth-death-master-equation.md), The upward jump has rate $\lambda$ and the downward jump rate $\beta x$, so the first two jump moments per unit time are $A(x)=\lambda-\beta x$ and $B(x)=\lambda+\beta x$. The second-order [Kramers-Moyal expansion](../../../../../kramers-moyal-expansion.md) gives the [diffusion approximation of a birth-death process](../../../../../diffusion-approximation-of-a-birth-death-process.md)

$$
\boxed{\partial_tP=-\partial_x[(\lambda-\beta x)P]+\frac12\partial_x^2[(\lambda+\beta x)P].}
$$

For the associated [Fokker-Planck equation](../../../../../fokker-planck-equation.md), integrating by parts with vanishing moment boundary terms gives $d\langle f\rangle/dt=\langle Af'+\tfrac12Bf''\rangle$. Taking $f=x,x^2$ yields

$$
\boxed{\frac{d\langle x\rangle}{dt}=\lambda-\beta\langle x\rangle,\qquad
\frac{d\langle x^2\rangle}{dt}=-2\beta\langle x^2\rangle+(2\lambda+\beta)\langle x\rangle+\lambda.}
$$

For example, if $m_0=\langle x(0)\rangle$, then $m(t)=\lambda/\beta+(m_0-\lambda/\beta)e^{-\beta t}$, while the [variance](../../../../../variance-split.md) satisfies $v'=-2\beta v+\lambda+\beta m$. The two boxed [moment equations](../../../../../moment-equation.md) also follow exactly from the discrete [Markov jump-process generator](../../../../../markov-jump-process-generator.md), since quadratic functions have no higher jump terms. A reflecting diffusion confined to $x\geq0$ can have extra boundary contributions; the formal approximation near extinction is not an exact replacement for the discrete process.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
