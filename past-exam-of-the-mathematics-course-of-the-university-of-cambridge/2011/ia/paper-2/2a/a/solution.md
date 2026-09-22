<h1 id="2a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [equilibrium of an autonomous differential equation](../../../../../../equilibrium-of-an-autonomous-differential-equation.md) is a constant $y_*$ with $f(y_*)=0$. Put $y=y_*+\eta$. For differentiable $f$, the [linear stability analysis](../../../../../../linear-stability.md) gives

$$
\eta'=f'(y_*)\eta+o(\eta).
$$

Thus the linear perturbation is proportional to $e^{f'(y_*)x}$. More directly, continuity of $f'$ makes $f(y)$ point toward $y_*$ on both sides when $f'(y_*)<0$, and away from it when $f'(y_*)>0$. Hence

$$
\boxed{f'(y_*)<0:\ \text{asymptotically stable};\qquad f'(y_*)>0:\ \text{unstable}.}
$$

The sign refers to evolution toward increasing $x$. If $f'(y_*)=0$, [linear stability analysis](../../../../../../linear-stability.md) is inconclusive: the leading nonzero nonlinear term or the signs of $f$ on either side are needed. For example $\eta'=-\eta^3$ is attracting whereas $\eta'=\eta^3$ is repelling, despite the same zero linear coefficient.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2A](../../2a.md)
3. [Section I](../../section-i.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
