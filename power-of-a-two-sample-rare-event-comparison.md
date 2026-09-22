# Power of a two-sample rare-event comparison

↑ **Parent:** [Statistical power](statistical-power.md)

For two independent samples of size $n$ with event probabilities $p_0,p_1$, put $\delta=p_0-p_1$, $\bar p=(p_0+p_1)/2$, $s_0^2=2\bar p(1-\bar p)/n$ and $s_1^2=[p_0(1-p_0)+p_1(1-p_1)]/n$. The normal approximation to a two-sided level-$\alpha$ test has power

$$
1-\Phi\left(\frac{z_{1-\alpha/2}s_0-\delta}{s_1}\right)+\Phi\left(\frac{-z_{1-\alpha/2}s_0-\delta}{s_1}\right).
$$

For rare events, independent [Poisson distributions](poisson-distribution.md) approximate the counts. Conditional on their total, the null count allocation is [binomial distribution](binomial-distribution.md) with probability one half; under the alternative the allocation probability is $p_0/(p_0+p_1)$. Averaging its exact rejection probability over the alternative total supplies a discrete power calculation.

// Target: probability-theory.bigb

## ↑ Ancestors (6)

1. [Statistical power](statistical-power.md)
2. [Clinical trial](clinical-trial.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/3/a/i/solution.md)
