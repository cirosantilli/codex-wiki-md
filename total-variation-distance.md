# Total variation distance

↑ **Parent:** [Probability and statistics](probability-and-statistics-split.md)

[Total variation distance](total-variation-distance.md) asks how much two [probability distributions](probability-distribution.md) can disagree about the same [event](event.md). For [probability measures](probability-measure.md) $P,Q$ on one [measurable space](measurable-space.md) $(S,\mathcal F)$, its definition is

$$
d_{\mathrm{TV}}(P,Q)=\lVert P-Q\rVert_{\mathrm{TV}}=\sup_{A\in\mathcal F}|P(A)-Q(A)|.
$$

The [supremum](supremum.md) ranges over all [measurable sets](measurable-set.md), so $d_{\mathrm{TV}}(P,Q)\leq\varepsilon$ guarantees that every yes-or-no prediction has [probability](probability.md) error at most $\varepsilon$. This [metric](metric.md) takes values between zero and one; it is zero exactly when the two [probability measures](probability-measure.md) agree. This makes it useful for comparing a sampling [algorithm](algorithm.md)'s output with its target [probability distribution](probability-distribution.md), and for defining the [mixing time of a Markov chain](mixing-time-of-a-markov-chain.md).

On a [finite set](finite-set.md), add the excess [probability mass](probability-mass.md) wherever $P$ exceeds $Q$. That excess is also half the sum of all absolute differences:

$$
d_{\mathrm{TV}}(P,Q)=\frac12\sum_{x\in S}|P(x)-Q(x)|=1-\sum_{x\in S}\min\{P(x),Q(x)\}.
$$

The last expression reveals the common [probability mass](probability-mass.md) that the two [probability distributions](probability-distribution.md) can share.[§4.1, Proposition 4.2 and Remark 4.3, printed p. 48; §4.2, equation (4.13), printed p. 51](markov-chains-and-mixing-times-second-edition-by-david-a-levin-and-others.md) The [coupling characterization of total variation distance](coupling-characterization-of-total-variation-distance.md) turns this overlap into an actual joint construction; [minimum sum of errors in a simple hypothesis test](minimum-sum-of-errors-in-a-simple-hypothesis-test.md) gives it a statistical interpretation. One quantity connects probability bookkeeping, comparison of sampling methods, and the limits of a [statistical test](statistical-test.md).

**Table of contents**

- [Total variation distance on a finite set](total-variation-distance-on-a-finite-set.md)
- [Total variation distance and hypothesis testing](total-variation-distance-and-hypothesis-testing.md)
- [Coupling characterization of total variation distance](coupling-characterization-of-total-variation-distance.md)
- [Coupling inequality for total variation](coupling-inequality-for-total-variation.md)
- [Total variation distance under a measurable map](total-variation-distance-under-a-measurable-map.md)
- [Pinsker's inequality](pinsker-s-inequality.md)

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (64)

- [Burn-in total variation comparison](burn-in-total-variation-comparison.md)
- [Chi-squared divergence of product measures](chi-squared-divergence-of-product-measures.md)
- [Contiguity of probability measures](contiguity-of-probability-measures.md)
- [Coupling characterization of total variation distance](coupling-characterization-of-total-variation-distance.md)
- [Doeblin's condition](doeblin-s-condition.md)
- [Eigenvalue lower bound for total variation mixing](eigenvalue-lower-bound-for-total-variation-mixing.md)
- [Fidelity of commuting mixed states](fidelity-of-commuting-mixed-states.md)
- [Gaussian location minimax lower bound under absolute-error loss](gaussian-location-minimax-lower-bound-under-absolute-error-loss.md)
- [Helstrom measurement for the zero and plus states](helstrom-measurement-for-the-zero-and-plus-states.md)
- [Maximal coupling](maximal-coupling.md)
- [Mean-estimation minimax lower bound for continuous densities](mean-estimation-minimax-lower-bound-for-continuous-densities.md)
- [Metric squared-loss two-point bound](metric-squared-loss-two-point-bound.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-55/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-37/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-36/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-36/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/2/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-215/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-348/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-210/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-326/3/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-326/3/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-326/3/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-326/3/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-224/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-210/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-216/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-216/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-201/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-201/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-208/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-215/1/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-326/2/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-215/2/b/solution.md)
- [Poisson approximation with dependency neighborhoods](poisson-approximation-with-dependency-neighborhoods.md)
- [Poisson limit for triangles in a binomial random graph](poisson-limit-for-triangles-in-a-binomial-random-graph.md)
- [Quantum Pinsker inequality](quantum-pinsker-inequality.md)
- [Scheffé lemma](scheffe-lemma.md)
- [Separation distance](separation-distance.md)
- [Stein-Chen bound with the Poisson Stein factor](stein-chen-bound-with-the-poisson-stein-factor.md)
- [Stein-Chen method](stein-chen-method.md)
- [Summable-memory coupling](summable-memory-coupling.md)
- [Total variation distance](total-variation-distance.md)
- [Total variation distance and hypothesis testing](total-variation-distance-and-hypothesis-testing.md)
- [Total variation distance on a finite set](total-variation-distance-on-a-finite-set.md)
- [Total variation distance under a measurable map](total-variation-distance-under-a-measurable-map.md)
- [Total variation–Hellinger–relative entropy inequality](total-variation-hellinger-relative-entropy-inequality.md)
- [Trace distance](trace-distance.md)
- [Two-point lower bound with a triangular bump](two-point-lower-bound-with-a-triangular-bump.md)
- [Variational characterization of trace distance](variational-characterization-of-trace-distance.md)
- [Well-posed Bayesian inverse problem in Hellinger distance](well-posed-bayesian-inverse-problem-in-hellinger-distance.md)
- [Well-posed Bayesian inverse problem in total variation](well-posed-bayesian-inverse-problem-in-total-variation.md)
