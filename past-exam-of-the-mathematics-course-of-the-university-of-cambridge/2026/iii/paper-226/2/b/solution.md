<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Strong Markov property](../../../../../../strong-markov-property.md) at the first visit to $0$ gives the [singleton equilibrium potential from the Green function](../../../../../../singleton-equilibrium-potential-from-the-green-function.md)

$$
h_x=P_x(\tau<\infty)=\frac{g(x,0)}{g(0,0)}.
$$

Let $U_n$ be an increasing exhaustion of $G$ by finite sets containing $0$, and let $g_{U_n}(x,0)$ be the [Green function of a transient weighted graph](../../../../../../green-function-of-a-transient-weighted-graph.md) stopped on leaving $U_n$. Each $g_{U_n}(\mathord\cdot,0)$ has finite support. The Green identity and the [Markov property](../../../../../../markov-property.md) give, for $m\geq n$,

$$
\mathcal E\bigl(g_{U_m}(\mathord\cdot,0)-g_{U_n}(\mathord\cdot,0),
g_{U_m}(\mathord\cdot,0)-g_{U_n}(\mathord\cdot,0)\bigr)
=g_{U_m}(0,0)-g_{U_n}(0,0).
$$

By the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md), the right side tends to zero as $m,n\to\infty$, while $g_{U_n}(x,0)\uparrow g(x,0)$. Thus $g(\mathord\cdot,0)$ is an $H_0$ limit of finitely supported functions. Dividing by the positive number $g(0,0)$ proves $h\in H_0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 226](../../../paper-226-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
