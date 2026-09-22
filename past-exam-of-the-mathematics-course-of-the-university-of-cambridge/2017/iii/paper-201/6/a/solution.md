<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $a>0$, the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) gives, for $t>0$,

$$
\mathbb P(H_a>t)=2\Phi(a/\sqrt t)-1\longrightarrow0,
$$

where $\Phi$ is the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md). Hence $H_a<\infty$ [almost surely](../../../../../../almost-sure-convergence.md); for $a=0$, $H_0=0$.

For $u\geq0$, use the [Exponential martingale for Brownian motion](../../../../../../exponential-martingale-for-brownian-motion.md) $Z_t=\exp(uB_t-u^2t/2)$. At $H_a\wedge t$, it is bounded by $e^{ua}$ because $B_s<a$ before the first hit and $B_{H_a}=a$ by continuity. The bounded [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives $\mathbb EZ_{H_a\wedge t}=1$. Its limit is $e^{ua-u^2H_a/2}$, and the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) yields $\mathbb E e^{ua-u^2H_a/2}=1$. Equivalently, the [Brownian first-passage Laplace transform](../../../../../../brownian-first-passage-laplace-transform.md) is

$$
\boxed{\mathbb E e^{-\lambda H_a}=e^{-a\sqrt{2\lambda}}\qquad(a,\lambda\geq0).}
$$

Taking $\lambda=u^2/2$ proves the displayed exponential identity. The cases $u=0$ and $a=0$ are included. The restriction $u\geq0$ is what gives the upper bound on the stopped exponential.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
