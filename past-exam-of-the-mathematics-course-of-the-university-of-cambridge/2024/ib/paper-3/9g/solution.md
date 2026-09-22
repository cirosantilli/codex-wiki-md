<h1 id="9g/solution">Solution</h1>

↑ **Parent:** [9G](../9g.md)

Fix $y\in V$. The map $x\mapsto\theta(x,y)$ is a linear functional, so the finite-dimensional [Riesz representation theorem](../../../../../riesz-representation-theorem.md) gives a unique [vector](../../../../../vector.md) $\beta(y)$ such that

$$
\theta(x,y)=\langle x,\beta(y)\rangle
\qquad(x\in V).
$$

For [scalars](../../../../../scalar.md) $\lambda,\mu$,

$$
\begin{aligned}
\langle x,\beta(\lambda y+\mu z)\rangle
&=\theta(x,\lambda y+\mu z)\\
&=\overline\lambda\,\theta(x,y)
 +\overline\mu\,\theta(x,z)\\
&=\langle x,\lambda\beta(y)+\mu\beta(z)\rangle.
\end{aligned}
$$

Uniqueness gives

$$
\boxed{\beta(\lambda y+\mu z)=\lambda\beta(y)+\mu\beta(z)},
$$

so $\beta$ is linear.

For $\alpha\in\operatorname{End}(V)$, apply this result to

$$
\theta(x,y)=\langle\alpha x,y\rangle.
$$

It produces a unique [linear map](../../../../../linear-map.md) $\alpha^*$ satisfying

$$
\boxed{\langle\alpha x,y\rangle=\langle x,\alpha^*y\rangle},
$$

which proves existence and uniqueness of the adjoint.

## ↑ Ancestors (10)

1. [9G](../9g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
