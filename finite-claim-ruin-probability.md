# Finite-claim ruin probability

↑ **Parent:** [Classical risk model](classical-risk-model.md)

In a [classical risk model](classical-risk-model.md), $T_j$ is the time of the $j$th claim. The displayed probability restricts ruin to the first $n$ claims and increases to the [ultimate ruin probability](ultimate-ruin-probability.md). Conditioning on the first arrival and severity gives $\psi_{n+1}(u)=\mathbb E[\overline F_X(u+cT_1)+\int_0^{u+cT_1}\psi_n(u+cT_1-x)f_X(x)\,dx]$, with $\psi_0=0$. For [exponential distribution](exponential-distribution.md) claims of mean $\mu$ and [relative safety loading](relative-safety-loading.md) $\rho$, put $d=1+\rho$ and $h=d+1$. Then $\psi_1(u)=e^{-u/\mu}/h$ and $\psi_2(u)=e^{-u/\mu}(h^{-1}+(u/\mu)h^{-2}+dh^{-3})$. The recursion follows because a surviving first claim leaves fresh independent future arrivals and claims. The formulas follow by integrating the rate-$\lambda$ first-arrival density; the claim-arrival rate cancels with $c=d\lambda\mu$.

## ↑ Ancestors (6)

1. [Classical risk model](classical-risk-model.md)
2. [Actuarial statistics](actuarial-statistics-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-35/2/solution.md)
