<h1 id="levy-construction-of-brownian-motion">Lévy construction of Brownian motion</h1>

↑ **Parent:** [Brownian motion](brownian-motion-split.md)

The Lévy construction builds [Brownian motion](brownian-motion-split.md) on $[0,1]$ by successive independent midpoint displacements on dyadic intervals. Start with $B_0=0$ and $B_1=Z_0$, where $Z_0$ has the [standard normal distribution](standard-normal-distribution.md). On each dyadic interval $[u,v]$, choose a fresh [independent](independent-random-variables.md) [standard normal random variable](standard-normal-random-variable.md) $Z$ and use the displayed midpoint rule. Conditional on the endpoints, this is the correct [Brownian bridge](brownian-bridge.md) midpoint law.

To verify the increment law, if $D=B_v-B_u\sim N(0,\ell)$ with $\ell=v-u$, the new increments are $D/2\pm\sqrt\ell Z/2$. They are [Jointly Gaussian](multivariate-normal-distribution.md), each has [variance](variance-split.md) $\ell/2$, and their [covariance](covariance.md) is zero, hence they are [independent](independent-random-variables.md). Induction gives all dyadic [Brownian increments](brownian-increment.md). The change between consecutive linear interpolants has uniform [norm](norm.md) $2^{-n/2-1}\max_{k<2^n}|Z_{n,k}|$. The [Gaussian tail bound](gaussian-tail-bound.md) and [union bound](boole-s-inequality.md) bound the chance that this maximum exceeds $n$ by $2^{n+1}e^{-n^2/2}$. The [First Borel-Cantelli lemma](borel-cantelli-first-lemma.md) and $\sum_n n2^{-n/2}<\infty$ prove [uniform convergence](uniform-convergence.md) [almost surely](almost-sure-convergence.md). The continuous limit has the required [Brownian increments](brownian-increment.md) at arbitrary times by dyadic approximation.

**Table of contents**

- [Lévy-Ciesielski expansion](levy-ciesielski-expansion.md)

## ↑ Ancestors (7)

1. [Brownian motion](brownian-motion-split.md)
2. [Stochastic process](stochastic-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Lévy-Ciesielski expansion](levy-ciesielski-expansion.md)
- [Solution](past-exam-of-the-continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford/2023/1/a/ii/solution.md)
- [Solution](past-exam-of-the-stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford/2009/a/1/d/solution.md)
