<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let

$$
a=(-1,2,0,4),\qquad\|a\|_2^2=21,
$$

so $T(\theta)=a^T(\theta_1,\ldots,\theta_4)$. In the [Gaussian sequence model](../../../../../gaussian-sequence-model.md), put $h_k=\sqrt n(\theta_k-Y_k)$. For each relevant coordinate, the posterior density of $h_k$ relative to the standard-normal density $\varphi$ is

$$
\frac{\pi(Y_k+h_k/\sqrt n)}
{\int\pi(Y_k+u/\sqrt n)\varphi(u)du}.
$$

The log-Lipschitz assumption implies

$$
e^{-c|h_k|/\sqrt n}
\leq\frac{\pi(Y_k+h_k/\sqrt n)}{\pi(Y_k)}
\leq e^{c|h_k|/\sqrt n}.
$$

These bounds provide Gaussian-integrable domination, while the ratio converges pointwise to one. Dominated convergence, coordinate independence, and the same argument after multiplying by $e^{ta^Th}$ show that, under the posterior,

$$
\mathbb E^\Pi\left[
 e^{t\sqrt n\{T(\theta)-T(Y)\}}\mid Y
\right]
\longrightarrow e^{21t^2/2}
$$

almost surely. The supplied moment-generating-function criterion therefore gives the finite-functional [Bernstein-von Mises theorem](../../../../../bernstein-von-mises-theorem.md)

$$
\sqrt n\{T(\theta)-T(Y)\}\mid Y
\Longrightarrow N(0,21),
$$

with uniform convergence of distribution functions.

If $z_{1-\alpha}=\Phi^{-1}(1-\alpha)$, the posterior quantile defining $R_n$ consequently satisfies

$$
\boxed{\sqrt nR_n\longrightarrow
\sqrt{21}\,z_{1-\alpha}}
$$

in probability. Under $P_{\theta_0}^Y$,

$$
\sqrt n\{T(\theta_0)-T(Y)\}=-a^Tg\sim N(0,21)
$$

for every $n$. Quantile convergence and the [Slutsky theorem](../../../../../slutsky-theorem.md) now yield

$$
\mathbb P_{\theta_0}^Y(T(\theta_0)\in C_n)
\longrightarrow1-\alpha.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
