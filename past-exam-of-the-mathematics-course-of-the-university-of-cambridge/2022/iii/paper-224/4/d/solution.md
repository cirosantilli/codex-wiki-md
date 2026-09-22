<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $\lambda\in\mathbb R$, define the finite-alphabet [exponential family](../../../../../../exponential-family-split.md)

$$
P_\lambda(x)=\frac{2^{\lambda f(x)}}{Z(\lambda)},
\qquad
Z(\lambda)=\sum_{y\in A}2^{\lambda f(y)}.
$$

The mean $\mathbb E_{P_\lambda}f$ is continuous and nondecreasing in $\lambda$, with limits $\min f$ and $\max f$ as $\lambda\to-\infty$ and $+\infty$. The strict interior assumption on $v$ therefore supplies a $\lambda$ with $\mathbb E_{P_\lambda}f=v$.

For any other $P$ satisfying the same constraint,

$$
D(P\Vert P_\lambda)
=-H(P)-\lambda v+\log_2Z(\lambda),
$$

so

$$
H(P)=\log_2Z(\lambda)-\lambda v-D(P\Vert P_\lambda)
\leq H(P_\lambda).
$$

Equality in [Gibbs inequality](../../../../../../gibbs-inequality.md) holds only for $P=P_\lambda$. Hence this Gibbs-form mass function is the unique entropy maximizer.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
