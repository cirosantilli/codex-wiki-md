# Moment matching for a beta prior

↑ **Parent:** [Beta distribution](beta-distribution.md)

To match mean $m\in(0,1)$ and variance $v\in(0,m(1-m))$ with a [Beta distribution](beta-distribution.md), set

$$
\kappa=\frac{m(1-m)}v-1,\qquad\alpha=m\kappa,\qquad\beta=(1-m)\kappa.
$$

The [Beta distribution](beta-distribution.md) identities $\mathbb EP=\alpha/(\alpha+\beta)$ and $\operatorname{Var}(P)=m(1-m)/(\alpha+\beta+1)$ prove the match. With binomial data the [Beta-binomial conjugacy](beta-binomial-conjugacy.md) gives a posterior mean that averages the empirical proportion and prior mean, with weights equal to sample size and $\kappa$.

// Target: statistical-inference.bigb

## ↑ Ancestors (7)

1. [Beta distribution](beta-distribution.md)
2. [Probability distribution](probability-distribution.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/4/i/solution.md)
