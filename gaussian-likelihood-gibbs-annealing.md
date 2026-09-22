# Gaussian likelihood Gibbs annealing

↑ **Parent:** [Likelihood-power annealing](likelihood-power-annealing.md)

Let $\bar x=m^{-1}\sum_i x_i$ and $S=\sum_i(x_i-\bar x)^2>0$. With Lebesgue base measure $d\mu\,dv$ for $v=\sigma^2$, the likelihood-power law has conditionals

$$
\mu\mid v\sim N(\bar x,Tv/m),\qquad
v\mid\mu\sim\operatorname{InvGamma}\left(\frac{m}{2T}-1,\frac{S+m(\mu-\bar x)^2}{2T}\right).
$$

The joint law is proper for $T<m/3$, since its marginal $v$ is [inverse-gamma distribution](inverse-gamma-distribution.md) with shape $m/(2T)-3/2$ and scale $S/(2T)$. There is also a direct convergence proof for successive [Gibbs sampling](gibbs-sampler.md) updates with deterministic $0<T_n\leq m/10$ and $T_n\to0$. Update $\mu_n$ from $v_{n-1}$, then $v_n$ from $\mu_n$. [Inverse-gamma distribution](inverse-gamma-distribution.md) moments and conditional normal moments give

$$
\mathbb E v_n=\frac{S+T_n\mathbb E v_{n-1}}{m-4T_n},\qquad
\mathbb E v_n^2=\frac{S^2+2ST_n\mathbb E v_{n-1}+3T_n^2\mathbb E v_{n-1}^2}{(m-4T_n)(m-6T_n)}.
$$

The coefficients of the preceding moments are bounded by $1/6$ and $1/8$, so these moments stay bounded from a finite deterministic initial [variance](variance-split.md). Letting $T_n\to0$ gives $\mathbb E v_n\to S/m$ and $\mathbb E v_n^2\to(S/m)^2$. Also $\mathbb E(\mu_n-\bar x)^2=T_n\mathbb E v_{n-1}/m\to0$. Thus the iterates converge in [mean](expected-value.md) square to the normal [maximum-likelihood estimate](maximum-likelihood-estimator.md).

## ↑ Ancestors (7)

1. [Likelihood-power annealing](likelihood-power-annealing.md)
2. [Simulated annealing](simulated-annealing.md)
3. [Heuristic optimization](heuristic-optimization.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/4/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/6/solution.md)
