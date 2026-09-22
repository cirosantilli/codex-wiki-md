<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

Take the [wave speed](../../../../../wave-speed.md) $c>0$ and introduce [characteristic coordinates](../../../../../characteristic-coordinate.md) $\xi=x+ct$, $\eta=x-ct$. The [chain rule](../../../../../chain-rule.md) gives

$$
\partial_x=\partial_\xi+\partial_\eta,\qquad\partial_t=c\partial_\xi-c\partial_\eta,\qquad y_{tt}-c^2y_{xx}=-4c^2y_{\xi\eta}.
$$

The [wave equation](../../../../../wave-equation-split.md) therefore says $y_{\xi\eta}=0$. Integrating first with respect to $\eta$ gives $y_\xi=F(\xi)$, and integrating with respect to $\xi$ gives **$y=f(x+ct)+g(x-ct)$** with twice differentiable $f,g$. Conversely substitution shows that every such sum solves the [wave equation](../../../../../wave-equation-split.md). The two terms are [travelling waves](../../../../../travelling-wave.md) of unchanged shape, moving respectively to the left and right at speed $c$.

The zero initial displacement gives $g(x)=-f(x)$, and the initial velocity gives $2cf'(x)=\psi(x)$. Hence the [D'Alembert formula with initial velocity](../../../../../d-alembert-formula-with-initial-velocity.md) is

$$
\boxed{y(x,t)=\frac1{2c}\int_{x-ct}^{x+ct}\psi(s)\,ds.}
$$

For a classical twice differentiable solution one may take $\psi\in C^1$. [Differentiation](../../../../../differentiation.md) gives $y_t(x,0)=\psi(x)$ and $y(x,0)=0$ directly. The coordinate calculation also works for any nonzero signed $c$, with physical speed $|c|$. If the printed constant is allowed to be $c=0$, the equation instead gives $y=A(x)+tB(x)$ and these initial data give $y=t\psi(x)$; the displayed travelling-wave representation requires $c\ne0$.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
