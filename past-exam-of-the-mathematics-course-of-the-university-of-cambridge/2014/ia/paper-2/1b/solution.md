<h1 id="1b/solution">Solution</h1>

↑ **Parent:** [1B](../1b.md)

With $\tau=1/t$, the [chain rule](../../../../../chain-rule.md) gives $d/dt=-\tau^2d/d\tau$. Since $u=v/\tau$,

$$
\frac{du}{dt}=v-\tau v',\qquad \frac{d^2u}{dt^2}=\tau^3v''.
$$

Substituting into the [ordinary differential equation](../../../../../ordinary-differential-equation.md) and multiplying by $\tau>0$ leaves $v''+\lambda^2v=0$, the [harmonic oscillator equation](../../../../../simple-harmonic-motion.md). Its two independent real solutions are $\cos(\lambda\tau)$ and $\sin(\lambda\tau)$. Undoing the [change of variables](../../../../../change-of-variables-formula.md) gives

$$
\boxed{u(t)=t\left[A\cos\frac\lambda t+B\sin\frac\lambda t\right],\qquad t>0.}
$$

The constants $A,B$ are arbitrary real numbers. The [reciprocal-coordinate reduction of a beam-type equation](../../../../../reciprocal-coordinate-reduction-of-a-beam-type-equation.md) works on the entire positive half-line, where the coordinate transformation is invertible.

## ↑ Ancestors (10)

1. [1B](../1b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
