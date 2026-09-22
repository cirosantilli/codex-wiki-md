<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

On a probability [measure-preserving system](../../../../../measure-preserving-system.md), for a finite [measurable partition](../../../../../measurable-partition.md) $\xi=\{A_1,\ldots,A_r\}$, the [entropy of a finite measurable partition](../../../../../entropy-of-a-finite-measurable-partition.md) is

$$
H_\mu(\xi)=-\sum_{i=1}^r\mu(A_i)\log\mu(A_i),\qquad0\log0=0.
$$

Use natural logarithms, so [information entropy](../../../../../information-entropy.md) is measured in nats; another fixed logarithm base rescales all answers. The [join of measurable partitions](../../../../../join-of-measurable-partitions.md) is their common refinement, and write $\xi_a^b=\bigvee_{j=a}^bT^{-j}\xi$, with an empty join the trivial partition. The [entropy rate of a measurable partition](../../../../../entropy-rate-of-a-measurable-partition.md) and [Kolmogorov-Sinai entropy](../../../../../kolmogorov-sinai-entropy.md) are respectively

$$
\boxed{h_\mu(T,\xi)=\lim_{N\to\infty}\frac1NH_\mu(\xi_0^{N-1}),\qquad h_\mu(T)=\sup_{\xi\text{ finite}}h_\mu(T,\xi)}.
$$

The block entropies form a [subadditive sequence](../../../../../subadditive-sequence.md), so the first limit exists by the [Fekete lemma](../../../../../fekete-s-lemma.md). For finite partitions the [conditional entropy of finite measurable partitions](../../../../../conditional-entropy-of-finite-measurable-partitions.md) is $H(\eta\mid\zeta)=H(\eta\vee\zeta)-H(\zeta)$.

Put $c_0=H(\xi)$ and $c_k=H(\xi\mid\xi_1^k)$ for $k\ge1$. The [chain rule for information entropy](../../../../../chain-rule-for-information-entropy.md), applied from the last coordinate backwards, and measure preservation give

$$
H(\xi_0^{N-1})=\sum_{j=0}^{N-1}H(T^{-j}\xi\mid\xi_{j+1}^{N-1})=\sum_{k=0}^{N-1}c_k.
$$

The second equality uses invariance of the joint [partition atom](../../../../../partition-atom.md) probabilities under the common pullback $T^{-j}$; invertibility is unnecessary. Since [conditioning reduces entropy](../../../../../conditioning-reduces-entropy.md), $c_k$ decreases to a nonnegative limit $c$. The [Cesaro convergence of a sequence](../../../../../cesaro-convergence-of-a-sequence.md) of this convergent sequence has the same limit. Therefore

$$
\boxed{h_\mu(T,\xi)=\lim_{k\to\infty}H_\mu(\xi\mid\xi_1^k)}.
$$

Equivalently $h_\mu(T,\xi)=H_\mu(\xi\mid\mathcal F_1)$, where $\mathcal F_1=\sigma(\bigvee_{j\ge1}T^{-j}\xi)$. Here [conditional entropy of a countable measurable partition](../../../../../conditional-entropy-of-a-countable-measurable-partition.md) conditioned on a [sigma-algebra](../../../../../sigma-algebra.md) is computed using conditional [partition atom](../../../../../partition-atom.md) probabilities; the [martingale convergence theorem](../../../../../martingale-convergence-theorem.md) gives continuity under increasing conditioning [sigma-algebras](../../../../../sigma-algebra.md). This is the [infinite-future formula for partition entropy rate](../../../../../infinite-future-formula-for-partition-entropy-rate.md).

The [Kolmogorov-Sinai generator theorem](../../../../../kolmogorov-sinai-generator-theorem.md) states that if a finite or countable [measurable partition](../../../../../measurable-partition.md) $\eta$ has finite [entropy of a countable measurable partition](../../../../../entropy-of-a-countable-measurable-partition.md) and its iterates generate the whole completed [sigma-algebra](../../../../../sigma-algebra.md) modulo null sets, then $h_\mu(T)=h_\mu(T,\eta)$. For an invertible system, generating means $\sigma(\bigvee_{j\in\mathbb Z}T^{-j}\eta)=\mathcal B$ modulo null sets. For a noninvertible system a [one-sided generator](../../../../../one-sided-generator.md), using $j\ge0$, suffices. The two-sided and one-sided versions must not be confused.

For a [Bernoulli shift](../../../../../bernoulli-shift.md) with discrete symbol probabilities $(p_i)$, the coordinate-zero [measurable partition](../../../../../measurable-partition.md) has independent coordinate iterates. Thus

$$
H(\eta_0^{N-1})=N\left(-\sum_i p_i\log p_i\right),\qquad\boxed{h_\mu(T)=-\sum_i p_i\log p_i}.
$$

For a finite alphabet the coordinate partition is a generator of finite [entropy of a finite measurable partition](../../../../../entropy-of-a-finite-measurable-partition.md); on the two-sided sequence space use all integer coordinate iterates, and on the one-sided space use the nonnegative ones. The [Kolmogorov-Sinai generator theorem](../../../../../kolmogorov-sinai-generator-theorem.md) proves the displayed answer in both cases. The same calculation applies to countably many symbols when their [Shannon entropy](../../../../../information-entropy.md) is finite, using the countable finite-entropy version of the theorem. If the [Shannon entropy](../../../../../information-entropy.md) is infinite, merge all but the first $r$ symbols into one cell. These finite coordinate partitions have entropy rate $-\sum_{i\le r}p_i\log p_i-p_{>r}\log p_{>r}\to\infty$, so the system entropy is infinite. Zero-probability symbols contribute zero. In particular a fair $r$-symbol shift has entropy $\log r$.

For the final assertion, let $\mathcal F_0=\sigma(\bigvee_{j\ge0}T^{-j}\xi)$ and complete it modulo null sets. The approximation property forces $\mathcal F_0=\mathcal B$ modulo null sets. Indeed for each $A\in\mathcal B$, choose approximating sets from finite blocks with error tending to zero. Their indicators approach $\mathbf1_A$ in $L^2$, and $L^2(\mathcal F_0)$ is a closed [vector subspace](../../../../../vector-subspace.md), so $A$ is $\mathcal F_0$-measurable modulo a null set.

Invertibility now gives $\mathcal F_1=T^{-1}\mathcal F_0=T^{-1}\mathcal B=\mathcal B$ modulo null sets. In particular the present partition $\xi$ is measurable with respect to its entire future, so $H(\xi\mid\mathcal F_1)=0$. The infinite-future formula gives $h_\mu(T,\xi)=0$. Since the given [one-sided generator](../../../../../one-sided-generator.md) is also a two-sided generator, the [Kolmogorov-Sinai generator theorem](../../../../../kolmogorov-sinai-generator-theorem.md) finishes the proof:

$$
\boxed{h_\mu(T)=0}.
$$

This is [finite one-sided generator of an invertible system forces zero entropy](../../../../../finite-one-sided-generator-of-an-invertible-system-forces-zero-entropy.md). Invertibility is essential: a fair binary one-sided [Bernoulli shift](../../../../../bernoulli-shift.md) has a finite [one-sided generator](../../../../../one-sided-generator.md) and [Kolmogorov-Sinai entropy](../../../../../kolmogorov-sinai-entropy.md) $\log2$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
