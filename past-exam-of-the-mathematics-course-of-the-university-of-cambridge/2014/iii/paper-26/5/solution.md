<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the [Donsker invariance principle](../../../../../donsker-s-theorem.md): for [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) of mean zero and variance one, the linearly interpolated processes $W_n$ with $W_n(k/n)=S_k/\sqrt n$ converge in distribution to standard [Brownian motion](../../../../../brownian-motion-split.md) in $C[0,1]$ with the uniform topology. No moment beyond the finite second moment is required.

The maximum functional $F(f)=\max_{0\leq t\leq1}f(t)$ is continuous, since $|F(f)-F(g)|\leq\|f-g\|_\infty$. A linear function on each interpolation interval has its maximum at an endpoint, so $F(W_n)=M_n/\sqrt n$. The [continuous mapping theorem](../../../../../continuous-mapping-theorem.md) therefore gives

$$
\frac{M_n}{\sqrt n}\xrightarrow{d}\max_{0\leq t\leq1}B_t.
$$

By the [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md), the limiting [random variable](../../../../../random-variable-split.md) has the distribution of $|Z|$, $Z\sim N(0,1)$. Its [distribution function](../../../../../cumulative-distribution-function.md) is continuous and has no atom at any $x\geq0$, so convergence in distribution permits passage to these tail probabilities. Hence

$$
\boxed{\lim_{n\to\infty}\mathbb P(M_n\geq x\sqrt n)
=2(1-\Phi(x))=\frac2{\sqrt{2\pi}}\int_x^\infty e^{-y^2/2}\,dy\quad(x\geq0).}
$$

At $x=0$ the left side is exactly one for every $n$, because $S_0=0$ is included in the maximum, and the right side is also one.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
