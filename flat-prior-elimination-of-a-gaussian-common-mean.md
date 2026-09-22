# Flat-prior elimination of a Gaussian common mean

↑ **Parent:** [Bayesian posterior](bayesian-posterior.md)

For independent observations $y_s\sim N(\beta+d_s,V_s)$, put $a_s=V_s^{-1}$, $S=\sum_sa_s$, $r_s=y_s-d_s$, $\bar r=S^{-1}\sum_sa_sr_s$ and $Q=\sum_sa_s(r_s-\bar r)^2$. Integrating the [likelihood function](likelihood-function.md) against a flat [improper prior](improper-prior.md) on $\beta$ gives, up to the arbitrary prior constant,

$$
(2\pi)^{-(N-1)/2}S^{-1/2}\prod_sV_s^{-1/2}\exp(-Q/2).
$$

Indeed $\sum_sa_s(r_s-\beta)^2=Q+S(\beta-\bar r)^2$, and the remaining one-dimensional [Gaussian integral](gaussian-integral.md) is $\sqrt{2\pi/S}$. The conditional [Bayesian posterior](bayesian-posterior.md) of $\beta$ is $N(\bar r,S^{-1})$.

## ↑ Ancestors (7)

1. [Bayesian posterior](bayesian-posterior.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Jeffreys prior for an additive variance component](jeffreys-prior-for-an-additive-variance-component.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/2/iii/solution.md)
