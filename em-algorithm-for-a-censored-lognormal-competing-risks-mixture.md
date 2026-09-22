# EM algorithm for a censored lognormal competing-risks mixture

↑ **Parent:** [Competing risks model](competing-risks-model.md)

Let eventual outcome $I=j$ have probability $\pi_j$, with $\log T\mid I=j\sim N(\mu_j,\sigma_j^2)$. An observed outcome at time $t$ contributes $\pi_j f_j(t)$ to the [likelihood](likelihood-function.md), while [right censoring](right-censoring.md) at $c$ contributes $\sum_j\pi_j S_j(c)$. The [expectation-maximization algorithm](expectation-maximization-algorithm.md) imputes both the censored outcome and its latent log event time. Its E-step uses the displayed conditional weights and the first two moments of a [truncated normal distribution](truncated-normal-distribution.md) above $\log c$. With $z=(\log c-\mu_j)/\sigma_j$ and [Inverse Mills ratio](inverse-mills-ratio.md) $\psi(z)$, these moments are $m=\mu_j+\sigma_j\psi(z)$ and $s=m^2+\sigma_j^2[1-\psi(z)(\psi(z)-z)]$. Observed outcomes use deterministic class weights and moments $\log t,(\log t)^2$. The M-step updates each class probability to its average weight, its mean to the weighted first moment, and its variance to the weighted second moment minus the squared new mean. Outcome-specific cumulative probabilities are [cumulative incidence functions](cumulative-incidence-function.md), not the conditional distributions $F(t\mid I=j)$ themselves.

## ↑ Ancestors (7)

1. [Competing risks model](competing-risks-model.md)
2. [Competing risks](competing-risks.md)
3. [Survival analysis](survival-analysis-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37/5/c/solution.md)
