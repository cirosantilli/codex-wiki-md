<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [total variation distance](../../../../../total-variation-distance.md) and [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) are

$$
\operatorname{TV}(P,Q)=\sup_A|P(A)-Q(A)|,
\qquad
\operatorname{KL}(P,Q)=
\int\log\left(\frac{dP}{dQ}\right)dP,
$$

with the divergence $+\infty$ when $P$ is not absolutely continuous with respect to $Q$.

For $P=\operatorname{Laplace}(0)$ and $Q=\operatorname{Laplace}(\mu)$,

$$
\log\frac{dP}{dQ}(x)=|x-\mu|-|x|.
$$

If $X\sim P$, direct integration on the intervals cut by $0$ and $\mu$ gives

$$
\mathbb E|X-\mu|=|\mu|+e^{-|\mu|},
\qquad
\mathbb E|X|=1.
$$

Consequently

$$
\operatorname{KL}(P,Q)=e^{-|\mu|}-1+|\mu|.
$$

One squared-loss form of [Assouad's lemma](../../../../../assouad-s-lemma.md) is as follows. Suppose $(P_\omega,\theta_\omega)_{\omega\in\{0,1\}^k}$ is an [Assouad hypercube](../../../../../assouad-hypercube.md) such that

$$
d(\theta_\omega,\theta_{\omega'})^2
\geq a\,d_H(\omega,\omega')
$$

and every pair of neighboring vertices satisfies $\operatorname{TV}(P_\omega,P_{\omega'})\leq\eta$. Then

$$
\inf_{\widehat\theta}\sup_\omega
\mathbb E_\omega d(\widehat\theta,\theta_\omega)^2
\geq\frac{ak}{8}(1-\eta).
$$

To prove it, decode from $\widehat\theta$ a nearest hypercube vertex. The separation condition converts estimation loss into a constant multiple of its Hamming error. Average this error under the uniform prior on $\omega$ and sum coordinatewise. For each coordinate, the two equally weighted mixtures with that bit equal to zero or one have total variation at most $\eta$ by convexity. The minimum average error of any binary test is $(1-\operatorname{TV})/2$, which gives the displayed bound after the nearest-vertex factor.

We now build such a hypercube inside the monotone cone. Let $k=\lfloor c_0n^{1/3}\rfloor$ and $m=\lfloor n/k\rfloor$. Divide the first $km$ coordinates into $k$ consecutive blocks. For $\omega\in\{0,1\}^k$, set on block $j$

$$
\theta_{\omega,i}=2\delta(j-1)+\delta\omega_j,
\qquad
\delta=\frac{c_1}{\sqrt m},
$$

and extend the remaining coordinates at the last level. If $c_0,c_1$ are sufficiently small universal constants, every signal is nondecreasing and belongs to $[0,1]^n$.

Neighboring vertices differ by $\delta$ on one block, so their squared Euclidean separation is $m\delta^2$. Their product experiments differ only on that block and have

$$
\operatorname{KL}(P_\omega,P_{\omega'})
=m(e^{-\delta}-1+\delta)
\leq\frac{m\delta^2}{2}
=\frac{c_1^2}{2}.
$$

By [Pinsker's inequality](../../../../../pinsker-s-inequality.md), choosing $c_1$ small makes every neighboring total variation distance at most, say, $1/4$.

Apply Assouad's lemma with normalized squared loss $d^2(\theta,\theta')=n^{-1}\lVert\theta-\theta'\rVert^2$. Here $a=m\delta^2/n=c_1^2/n$, and hence

$$
\inf_{\widehat\theta}
\sup_{\theta\in\mathcal M_n\cap[0,1]^n}
\frac1n\mathbb E_\theta\lVert\widehat\theta-\theta\rVert^2
\geq c\frac{k}{n}
\geq c'n^{-2/3}.
$$

This proves the lower half of the [minimax rate for isotonic sequence estimation](../../../../../minimax-rate-for-isotonic-sequence-estimation.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
