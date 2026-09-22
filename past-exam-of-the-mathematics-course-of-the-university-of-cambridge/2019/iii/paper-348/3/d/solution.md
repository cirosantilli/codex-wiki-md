<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $\nu=(T^\dagger)_\#\mu$ and use the two [Kantorovich potentials](../../../../../../kantorovich-potential.md)

$$
u(x)=(1-\lambda)|x|^2,\qquad
v(y)=\left(1-\frac1\lambda\right)|y|^2.
$$

For every $x,y\in\mathbb R^d$,

$$
\begin{aligned}
|x-y|^2-u(x)-v(y)
&=\lambda|x|^2+\lambda^{-1}|y|^2-2x\cdot y\\
&=\lambda^{-1}|y-\lambda x|^2\geq0.
\end{aligned}
$$

Thus the pair is dual feasible, with equality precisely on $y=\lambda x$. Finite second [moments](../../../../../../moment.md) make both potentials integrable; compactness of $X$ is more than sufficient. For any admissible [transport map](../../../../../../transport-map.md) $T$, integrating the inequality and using its [pushforward measure](../../../../../../pushforward-measure.md) gives

$$
\int|x-T(x)|^2\,d\mu\geq\int u\,d\mu+\int v\,d\nu.
$$

The admissible map $T^\dagger(x)=\lambda x$ attains equality. Consequently

$$
\boxed{T^\dagger(x)=\lambda x\ \text{is optimal},\qquad\min\mathbb M=(1-\lambda)^2\int|x|^2\,d\mu.}
$$

The same certificate proves optimality of its graph [transport plan](../../../../../../transport-plan.md) among all [transport plans](../../../../../../transport-plan.md). Notice that $u$ need not be a [convex function](../../../../../../convex-function.md) when $\lambda>1$: it is a cost dual potential. The associated [convex](../../../../../../convex-function.md) gradient potential is instead $\Phi(x)=\lambda|x|^2/2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
