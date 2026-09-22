<h1 id="27i/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Passing to the deterministic-service limit in part (c), near zero, gives

$$
\phi_B(\theta)=\exp\!\left[\frac{\theta+\lambda(\phi_B(\theta)-1)}{\mu}\right].
$$

Differentiation at zero gives $\mathbb EB=(1+\lambda\mathbb EB)/\mu$. Alternatively, the same branching expectation equation gives $\mathbb EB_k=1/(\mu-\lambda)$ for every $k$, because $\mathbb ES_k=1/\mu$. The assumed convergence of finite moment-generating functions at a positive point near zero bounds exponential moments and makes these means uniformly integrable, so the means pass to the limit. Since $T=A+B$, **the answers are**

$$
\boxed{\mathbb EB=\frac1{\mu-\lambda},\qquad\mathbb ET=\frac1\lambda+\frac1{\mu-\lambda}}.
$$

They correspond to an [M/D/1 queue](../../../../../../m-d-1-queue.md) with deterministic service time $1/\mu$. The calculation only needs finite transforms near zero; the literal assumption of finite transforms for every $\theta<\lambda$ is stronger than necessary and is not generally true for positive busy-period arguments. For instance, with $k=1$ and $\lambda=\mu/2$, part (c) gives $\lambda b^2-(\mu+\lambda-\theta)b+\mu=0$. Its discriminant is negative for $(\sqrt\mu-\sqrt\lambda)^2<\theta<\lambda$, so no finite busy-period transform can exist there.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [27I](../../27i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
