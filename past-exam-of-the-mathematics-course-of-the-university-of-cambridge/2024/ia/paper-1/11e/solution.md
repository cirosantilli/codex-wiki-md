<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

The [intermediate value theorem](../../../../../intermediate-value-theorem.md) states that if $f:[\alpha,\beta]\to\mathbb R$ is continuous and $y$ lies between $f(\alpha)$ and $f(\beta)$, then some $c\in[\alpha,\beta]$ satisfies $f(c)=y$.

It is enough to prove the case

$$
f(\alpha)<y<f(\beta).
$$

Let

$$
E=\{x\in[\alpha,\beta]:f(x)<y\},
\qquad c=\sup E.
$$

Choose $x_n\in E$ with $x_n\to c$. Continuity gives $f(c)\leq y$. If $f(c)<y$, continuity would make $f(x)<y$ for some $x>c$, contradicting that $c$ is an upper bound of $E$. Thus $f(c)=y$. The case with reversed endpoint inequalities follows by replacing $f$ with $-f$.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
