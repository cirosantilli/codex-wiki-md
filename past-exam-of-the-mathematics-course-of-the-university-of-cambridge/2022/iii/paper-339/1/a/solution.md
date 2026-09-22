<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A vector $g$ is a [subgradient](../../../../../../subgradient.md) of the [convex function](../../../../../../convex-function.md) $f$ at $x$ when

$$
f(y)\geq f(x)+g^T(y-x)
$$

for every $y$. The set of all such vectors is the [subdifferential](../../../../../../subdifferential.md) $\partial f(x)$. The [proximal operator](../../../../../../proximal-operator.md) satisfies

$$
\boxed{u=\operatorname{prox}_f(x)
\quad\Longleftrightarrow\quad x-u\in\partial f(u).}
$$

More generally, $u=\operatorname{prox}_{tf}(x)$ exactly when $(x-u)/t\in\partial f(u)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
