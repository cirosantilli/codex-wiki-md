<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce [conformal time](../../../../../../conformal-time.md)

$$
\eta=\int_0^t\frac{ds}{\cosh s}=2\arctan[\tanh(t/2)]=\arcsin(\tanh t),
\qquad -\frac\pi2<\eta<\frac\pi2.
$$

It satisfies $d\eta/dt=\operatorname{sech}t$ and $\cos\eta=\operatorname{sech}t$, so the metric becomes $ds^2=\sec^2\eta(-d\eta^2+d\xi^2)$. Choose [null coordinates](../../../../../../null-coordinate.md)

$$
\boxed{u=\xi-\eta,\qquad v=\xi+\eta,\qquad
ds^2=\sec^2\!\left(\frac{v-u}{2}\right)du\,dv.}
$$

Thus $f(u,v)=\sec[(v-u)/2]$ is positive on $-\pi<v-u<\pi$. Choosing the two null coordinates with these orientations gives the requested positive coefficient of $du\,dv$.

There is a global-topology distinction in the source: unrestricted $\xi\in\mathbb R$ gives the [universal cover of two-dimensional de Sitter spacetime](../../../../../../universal-cover-of-two-dimensional-de-sitter-spacetime.md). The usual [two-dimensional de Sitter spacetime](../../../../../../two-dimensional-de-sitter-spacetime.md) has $\xi$ periodic modulo $2\pi$. Indeed its standard embedding is $X^0=\sinh t$, $X^1=\cosh t\cos\xi$, $X^2=\cosh t\sin\xi$, and is unchanged by $\xi\mapsto\xi+2\pi$. The local metric and the null-coordinate calculation apply to either choice.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
