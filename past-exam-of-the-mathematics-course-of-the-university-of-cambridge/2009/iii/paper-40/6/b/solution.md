<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\theta_0=\theta^{(t)}$ and $h_0(z)=f(x,z;\theta_0)/L(x\mid\theta_0)$. Assume the likelihoods are positive and the expected log likelihoods used in the step are finite. On the support where $h_0>0$, let $r(z)=f(x,z;\theta)/f(x,z;\theta_0)$. Integrating over that support gives

$$
\frac{L(x\mid\theta)}{L(x\mid\theta_0)}\ge\int h_0(z)r(z)\,dz.
$$

It is an equality when the candidate joint density has no additional mass outside the old support. Concavity of the logarithm and the [Jensen inequality](../../../../../../jensen-s-inequality.md) now imply

$$
\begin{aligned}
\log L(x\mid\theta)-\log L(x\mid\theta_0)&\ge\log\mathbb E_{h_0}r(Z)\\
&\ge\mathbb E_{h_0}\log r(Z)\\
&=Q(\theta\mid\theta_0)-Q(\theta_0\mid\theta_0).
\end{aligned}
$$

Thus the argument does not silently require an identical support at every parameter. The M-step selects a value whose right-hand side is nonnegative, proving [EM likelihood monotonicity](../../../../../../em-likelihood-monotonicity.md):

$$
\boxed{\log L(x\mid\theta^{(t+1)})\ge\log L(x\mid\theta^{(t)}).}
$$

When the conditional densities allow finite divergence, the same calculation has the informative exact form

$$
\log L(x\mid\theta)-\log L(x\mid\theta_0)=Q(\theta\mid\theta_0)-Q(\theta_0\mid\theta_0)+\operatorname{KL}(h_0\Vert h_\theta).
$$

The [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) is nonnegative, since $\mathbb E_{h_0}\log(h_\theta/h_0)\le\log\int_{\{h_0>0\}}h_\theta\le0$. This also explains why an increase of the surrogate objective guarantees an increase of the observed objective, while equality of the two likelihoods is possible.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
