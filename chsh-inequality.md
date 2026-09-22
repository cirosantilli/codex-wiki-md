# CHSH inequality

↑ **Parent:** [Bell theorem](bell-theorem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/CHSH_inequality)

For local outcomes $A_0,A_1,B_0,B_1\in\{-1,1\}$, the Clauser–Horne–Shimony–Holt inequality is

$$
|E(A_0B_0)+E(A_0B_1)+E(A_1B_0)-E(A_1B_1)|\leq2.
$$

An arbitrary no-signalling correlation can reach the algebraic maximum $4$, while quantum correlations are bounded by $2\sqrt2$.

For a short proof of the local bound, fix a [deterministic local hidden-variable model](deterministic-local-hidden-variable-model.md) assignment. The combination is $A_0(B_0+B_1)+A_1(B_0-B_1)$. Exactly one bracket vanishes and the other is $\pm2$, so every assignment contributes $\pm2$. Averaging with a single setting-independent [probability distribution](probability-distribution-split.md) preserves the interval $[-2,2]$. Mixtures also cover stochastic [local hidden-variable theories](local-hidden-variable-theory.md). Rejecting a different sample at each setting would invalidate precisely that common-average step.

The quantum bound follows just as economically. For [Hermitian operators](hermitian-operator.md) with $A_i^2=B_j^2=I$, the [CHSH inequality](chsh-inequality.md) operator $C=A_0\otimes(B_0+B_1)+A_1\otimes(B_0-B_1)$ obeys $C^2=4I-[A_0,A_1]\otimes[B_0,B_1]$. Each [commutator](commutator.md) has [operator norm](operator-norm.md) at most two, giving $\|C\|\leq2\sqrt2$. The [Polarization CHSH count model](polarization-chsh-count-model.md) attains this bound without allowing either station to control the distant marginal [probability distribution](probability-distribution-split.md).

**Table of contents**

- [Reflected real-basis CHSH strategy](reflected-real-basis-chsh-strategy.md)
- [CHSH game](chsh-game.md)
- [Maximal CHSH witness for a fixed Bell state](maximal-chsh-witness-for-a-fixed-bell-state.md)
- [CHSH self-testing](chsh-self-testing.md)
- [Polarization CHSH count model](polarization-chsh-count-model.md)
- [CHSH optimum from the correlation tensor](chsh-optimum-from-the-correlation-tensor.md)
- [Gisin's theorem](gisin-s-theorem.md)
  - [CHSH axes for an entangled pure two-qubit state](chsh-axes-for-an-entangled-pure-two-qubit-state.md)
- [No-signalling box](no-signalling-box.md)
  - [Popescu–Rohrlich box](popescu-rohrlich-box.md)
    - [One-bit computation using Popescu–Rohrlich boxes](one-bit-computation-using-popescu-rohrlich-boxes.md)

## ↑ Ancestors (6)

1. [Bell theorem](bell-theorem.md)
2. [Foundations of quantum mechanics](foundations-of-quantum-mechanics-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (43)

- [Aspect switching experiment](aspect-switching-experiment.md)
- [Bell inequality](bell-inequality.md)
- [Bell local causality](bell-local-causality.md)
- [Bell theorem](bell-theorem.md)
- [Chained modular Bell inequality](chained-modular-bell-inequality.md)
- [CHSH axes for an entangled pure two-qubit state](chsh-axes-for-an-entangled-pure-two-qubit-state.md)
- [CHSH game](chsh-game.md)
- [CHSH inequality](chsh-inequality.md)
- [CHSH self-testing](chsh-self-testing.md)
- [CHSH Tsirelson bound](chsh-tsirelson-bound.md)
- [Detection loophole](detection-loophole.md)
- [Freedman-Clauser experiment](freedman-clauser-experiment.md)
- [Gisin's theorem](gisin-s-theorem.md)
- [Measurement-independence loophole](measurement-independence-loophole.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information/1/c/ii/solution.md)
- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2021/2/d/solution.md)
- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2021/2/e/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2009/8/2/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2009/8/3/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2021/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-54/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-59/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-59/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-59/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-62/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-325/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-325/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-325/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-325/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-325/2/c/solution.md)
- [Solution](past-exam-of-the-philosophy-of-science-supplementary-subject-of-the-university-of-oxford/2021/7/solution.md)
- [Solution](past-exam-of-the-philosophy-of-space-time-and-philosophy-of-quantum-mechanics-paper-of-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford/2019/8/b/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2012/paper-1/2/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2015/paper-1/2/c/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2015/paper-1/2/e/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2016/paper-1/1/solution.md)
- [Solution](past-exam-of-the-short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford/2015/s28/3/solution.md)
- [Solution](past-exam-of-the-short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford/2017/s28/1/solution.md)
- [Polarization CHSH count model](polarization-chsh-count-model.md)
- [Popescu–Rohrlich box](popescu-rohrlich-box.md)
- [Setting-independent heralding preserves Bell locality](setting-independent-heralding-preserves-bell-locality.md)
