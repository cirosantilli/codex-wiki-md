<h1 id="1/i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under independent assignment,

$$
\mathbb P(Z=z)=\prod_{i=1}^n\pi_{z_i}
=\prod_{r=0}^2\pi_r^{N_r(z)}.
$$

The arm-count vector has a [multinomial distribution](../../../../../../../multinomial-distribution.md). Conditional on $N_r=n_r$ for $r=0,1,2$, every compatible vector has the same factor $\prod_r\pi_r^{n_r}$, so

$$
\mathbb P(Z=z\mid N_0=n_0,N_1=n_1,N_2=n_2)
=\frac{n_0!n_1!n_2!}{n!}
$$

for compatible $z$, and zero otherwise. Conditioning independent assignment on its arm sizes therefore recovers [complete randomization](../../../../../../../complete-randomization.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [I](../../i.md)
3. [1](../../../1.md)
4. [Paper 221](../../../../paper-221-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
