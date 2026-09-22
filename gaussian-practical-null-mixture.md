# Gaussian practical-null mixture

↑ **Parent:** [Bayes factor](bayes-factor.md)

A [Gaussian practical-null mixture](gaussian-practical-null-mixture.md) compares a narrow centered [normal distribution](normal-distribution.md) prior with a wider centered [normal distribution](normal-distribution.md) prior. Neither component is a point mass. With observed mean $y\mid\beta\sim N(\beta,1/n)$ and prior precisions $q_0>q_1>0$, its model predictive variances are $V_i=1/n+1/q_i$, and the [Bayes factor](bayes-factor.md) is

$$
B_{01}(y)=\sqrt{V_1/V_0}\exp[-y^2(V_0^{-1}-V_1^{-1})/2].
$$

The overall [posterior density](posterior-density.md) is a [Bayesian model averaging](bayesian-model-averaging.md) mixture with component means $ny/(n+q_i)$. A wide-prior penalty can favor the practical null near zero; its dominance depends quantitatively on both prior scales and the observation, not merely on the observation being of order $n^{-1/2}$.

## ↑ Ancestors (8)

1. [Bayes factor](bayes-factor.md)
2. [Bayesian model evidence](bayesian-model-evidence.md)
3. [Bayesian statistics](bayesian-statistics.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gaussian practical-null mixture](gaussian-practical-null-mixture.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/h/solution.md)
