# Bias from returning a rejected proposal after a rejection-sampling cap

↑ **Parent:** [Rejection sampling](rejection-sampling.md)

Consider independent [rejection sampling](rejection-sampling.md) trials with proposal density $q$, accepted-value density $f$, acceptance probability $a\in(0,1)$ and rejection probability $r=1-a$. Splitting the proposal law by its accept/reject outcome gives $q=af+rg_R$, where $g_R$ is the [rejected-proposal distribution](rejected-proposal-distribution.md).

If an algorithm permits $n$ trials, returns the first accepted value when one occurs, and otherwise returns the final rejected proposal, its output density is the displayed mixture. The event of $n$ failures has probability $r^n$ and gives the conditional law $g_R$; every successful stopping trial gives law $f$. Hence the forced return introduces bias unless $g_R=f$, and its contribution decays geometrically with the cap. Conditional on success before any specified trial, the output still has law $f$, since accepted value and successful-trial index are independent.

## ↑ Ancestors (6)

1. [Rejection sampling](rejection-sampling.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-statistics-and-options-i-course-of-the-university-of-oxford/2011/s/1/c/solution.md)
