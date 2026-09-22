<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\tau=T_a\wedge T_b$. The walk exits the finite interval $[a,b]$ almost surely, and the stopped martingale $\phi(S_{n\wedge\tau})$ is bounded between $\lambda^b$ and $\lambda^a$. The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) and [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md) give

$$
1=\phi(0)=\mathbb E[\phi(S_\tau)]
=\lambda^a\mathbb P(T_a<T_b)
+\lambda^b\mathbb P(T_b<T_a).
$$

Solving for the first probability gives the [biased gambler's ruin probability](../../../../../../biased-gambler-s-ruin-probability.md)

$$
\boxed{\mathbb P(T_a<T_b)
=\frac{\lambda^b-1}{\lambda^b-\lambda^a}
=\frac{\phi(b)-\phi(0)}{\phi(b)-\phi(a)}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
