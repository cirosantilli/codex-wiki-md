<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In natural logarithms, [Fano's inequality](../../../../../../fano-s-inequality.md) for a uniform index $J$ among $N$ alternatives states $\mathbb P(\widehat J\ne J)\geq1-(I(J;G)+\log2)/\log N$. The [mutual information](../../../../../../mutual-information.md) is at most the average [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) to any fixed reference law. With the supplied packing, nearest-neighbour decoding turns partition error below half the separation into correct decoding. Thus the packing alone proves a bound at radius $n(1/4-\varepsilon/2)$, with the unavoidable $\log2$ term. It does not automatically prove the much larger printed radius.

A [list-decoding Fano inequality](../../../../../../list-decoding-fano-inequality.md) supplies the intended near-half error threshold. Assume $0<\varepsilon<1/4$, since otherwise that threshold is nonpositive and its event is automatic. Take a uniform prior on all $N=\binom n{n/2}/2$ unlabelled balanced partitions, and let $r=n(1/2-2\varepsilon)$. A [Hamming ball](../../../../../../hamming-ball.md) of radius less than $r$ around any estimated partition contains at most $B=\sum_{j<r}\binom nj$ such partitions. This follows by selecting the representative closer to the estimated group; each unlabelled partition contributes at most one such representative because $r<n/2$. The [entropy bound for a Hamming ball](../../../../../../entropy-bound-for-a-hamming-ball.md) gives $\log B\leq n h(r/n)$, where $h$ is the [binary entropy function](../../../../../../binary-entropy-function.md) measured in natural logarithms. Its curvature gives $\log2-h(1/2-2\varepsilon)\geq8\varepsilon^2$. Also $\binom n{n/2}\geq2^n/(n+1)$, so

$$
\log(N/B)\geq8\varepsilon^2n-\log(2(n+1)).
$$

Use the all-$1/2$ independent-edge law $P_*$ as a reference. Only the $n^2/4$ crossing pairs differ; the preceding [Bernoulli distribution](../../../../../../bernoulli-distribution.md) divergence estimate gives $D_{\mathrm{KL}}(P_S\Vert P_*)\leq nt^2$. Hence $I(J;G)\leq nt^2$. Whenever the denominator is positive, the [list-decoding Fano inequality](../../../../../../list-decoding-fano-inequality.md) proves the finite-sample answer

$$
\boxed{\inf_{\widehat S}\max_S P_S\{\Delta(\widehat S,S)\geq r\}\geq1-\frac{nt^2+\log2}{8\varepsilon^2n-\log(2(n+1))}.}
$$

For $4\varepsilon^2n\geq\log(2(n+1))$, this is at least $1-t^2/(4\varepsilon^2)-\log2/(4\varepsilon^2n)$. If in addition $nt^2\geq\log2$, it implies the intended form with $c'=1/2$. This proves the claimed information-theoretic scale with its needed finite-sample qualifications.

**As a uniform finite-sample assertion for every positive $t$, the printed form is false.** At $t=0$ every partition has the same data law, and a uniformly random balanced guess has a positive chance of being correct, giving error strictly below one. Such randomness can also be extracted from the finite graph sample: assign distinct graph outcomes to the finitely many balanced partitions; under the common law every selected outcome has positive [probability](../../../../../../probability.md). The worst error remains strictly below one for sufficiently small positive $t$, by continuity. The printed lower bound tends to one as $t\downarrow0$ for any fixed universal $c'$, which contradicts this. The entropy correction cannot be dropped without an asymptotic or signal-size condition.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
