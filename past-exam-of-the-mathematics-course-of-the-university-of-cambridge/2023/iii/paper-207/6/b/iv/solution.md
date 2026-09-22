<h1 id="6/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

With administrative censoring at $c$, one patient is observed to experience $A$ with probability

$$
\int_0^c\theta e^{-(\theta+\phi)t}\,dt
=\frac{\theta}{\theta+\phi}
\left(1-e^{-(\theta+\phi)c}\right),
$$

so

$$
\mathbb E[v_+]
=n\frac{\theta}{\theta+\phi}
\left(1-e^{-(\theta+\phi)c}\right).
$$

The observed time is $\min(T_A,T_B,c)$, whose mean follows from the [tail-sum formula for expectation](../../../../../../../tail-sum-formula-for-expectation.md):

$$
\mathbb E[\min(T_A,T_B,c)]
=\int_0^ce^{-(\theta+\phi)t}\,dt
=\frac{1-e^{-(\theta+\phi)c}}{\theta+\phi}.
$$

Hence

$$
\boxed{\mathbb E[x_+]
=n\frac{1-e^{-(\theta+\phi)c}}{\theta+\phi},
\qquad
\frac{\mathbb E[v_+]}{\mathbb E[x_+]}=\theta.}
$$

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
