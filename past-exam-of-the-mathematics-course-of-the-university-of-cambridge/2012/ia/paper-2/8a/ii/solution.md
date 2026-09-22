<h1 id="8a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Before the impulse the zero initial data force $y_2=0$. An impulse modeled by the [Dirac delta function](../../../../../../dirac-delta-function.md) requires continuity of $y_2$: a jump in $y_2$ would introduce an unwanted derivative of a delta in $y_2''$. Integrating the equation across $t=a$ then gives the velocity jump $y_2'(a+)-y_2'(a-)=1$.

The [causal Green function of a damped oscillator](../../../../../../causal-green-function-of-a-damped-oscillator.md) is

$$
g(s)=e^{-ks}\frac{\sin\omega s}{\omega},\qquad g(0)=0,\quad g'(0)=1.
$$

The jump conditions give the causal impulse response

$$
\boxed{y_2(t,a)=H(t-a)e^{-k(t-a)}\frac{\sin[\omega(t-a)]}{\omega}}.
$$

Here $H$ is the [Heaviside step function](../../../../../../heaviside-step-function.md). For $\omega=0$, interpret the quotient continuously as $t-a$, giving $H(t-a)(t-a)e^{-k(t-a)}$. Both initial values are zero because $a>0$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [8A](../../8a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
