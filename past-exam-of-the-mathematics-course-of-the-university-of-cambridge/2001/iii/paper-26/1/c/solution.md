<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Varadhan's lemma](../../../../../../varadhan-s-lemma.md) states that if $U_n$ has a [large deviation principle](../../../../../../large-deviation-principle.md) with [good rate function](../../../../../../good-rate-function.md) $K$ and [large-deviation speed](../../../../../../large-deviation-speed.md) $a_n$, then for every bounded [continuous](../../../../../../continuous-function.md) real function $h$,

$$
\lim_n\frac1{a_n}\log\mathbb E e^{a_nh(U_n)}=\sup_u\{h(u)-K(u)\}.
$$

For a continuous function unbounded above, the same conclusion holds under the [exponential tail extension of Varadhan's lemma](../../../../../../exponential-tail-extension-of-varadhan-s-lemma.md), for example when the weighted contribution from $h>M$ is superexponentially negligible as $M\to\infty$.

The [scalar clipping](../../../../../../scalar-clipping.md) map $g(m)=\min(b,\max(a,m))$ is continuous. The [rate function under scalar clipping](../../../../../../rate-function-under-scalar-clipping.md) has endpoint costs $\inf_{m\le a}J(m)$ and $\inf_{m\ge b}J(m)$. Since $a<\mu<b$ and the costs decrease towards $\mu$ from the left and increase to its right, both infima are attained at the corresponding endpoints. Thus the [good rate function](../../../../../../good-rate-function.md) of $Z_n$ equals $J(z)$ on $[a,b]$ and is infinite outside. The function $\log z$ is bounded and continuous on that compact interval, so

$$
\lim_n\frac1n\log\mathbb E[Z_n^n]
=\max_{a\le z\le b}\{\log z-J(z)\}.
$$

On $[a,\mu]$, the derivative of $\log z-I(z)$ is $2/z-\lambda>0$, so the maximum there is $\log\mu$. On $[\mu,b]$, the derivative is $(k+1)/z-k\lambda$, with negative second derivative. Its unconstrained maximizer is

$$
z_* =\frac{k+1}{k\lambda}.
$$

It lies in $[\mu,b]$ whenever $k\ge(\lambda b-1)^{-1}$. The right-hand objective increases initially at $\mu$, so this maximizer dominates the whole left-hand interval. Substitution gives the limit for [high moments of a clipped minimum of exponential sample means](../../../../../../high-moments-of-a-clipped-minimum-of-exponential-sample-means.md)

$$
\boxed{\lim_n\frac1n\log\mathbb E[Z_n^n]
=(k+1)\log\frac{k+1}{k}-\log\lambda-1.}
$$

The moment here is the [expectation](../../../../../../expected-value.md) of the $n$th power. If the printed notation were instead read as $(\mathbb E Z_n)^n$, its logarithmic limit would be $\log\mu=-\log\lambda$, since boundedness and [convergence in probability](../../../../../../convergence-in-probability.md) give $\mathbb E Z_n\to\mu$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
