<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a linear spatial operator, let $U(t,s)$ denote the formal homogeneous evolution from time $s$ to time $t$, satisfying $\partial_tU(t,s)h+D(t)U(t,s)h=0$ and $U(s,s)h=h$. This also allows time-dependent coefficients in the spatial operator. The [Duhamel principle](../../../../../../duhamel-s-principle.md) states

$$
\boxed{f(t)=U(t,0)f_0+\int_0^tU(t,s)g(s)\,ds}.
$$

Differentiation of the [integral](../../../../../../integral.md) contributes $g(t)$ at its upper endpoint and $-D(t)$ times the [integral](../../../../../../integral.md), while the initial value is $f_0$. If $D$ is time-independent, one writes $U(t,s)=S(t-s)=e^{-(t-s)D}$. The principle uses [linearity](../../../../../../linearity.md); an arbitrary nonlinear differential operator would not justify this superposition formula. No analytic construction of $U$ or boundary conditions is required for this formal statement.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
