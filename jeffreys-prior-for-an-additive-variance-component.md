# Jeffreys prior for an additive variance component

↑ **Parent:** [Jeffreys prior](jeffreys-prior.md)

For independent normal observations with fixed means and variances $v+r_s$, where $v\ge0$ is unknown and all known $r_s>0$, the scalar [Fisher information](fisher-information-matrix.md) for $v$ is $I_{vv}=\frac12\sum_s(v+r_s)^{-2}$. Thus its scalar [Jeffreys prior](jeffreys-prior.md) is finite at zero and behaves like $1/v$ at infinity. Unlike a log-flat prior $1/v$, it avoids a divergent integral at the zero-variance boundary. After [flat-prior elimination of a Gaussian common mean](flat-prior-elimination-of-a-gaussian-common-mean.md), the integrated likelihood is bounded by a constant times $v^{-(N-1)/2}$, so this prior yields a proper posterior for $N>1$ and a proper prior on any remaining mean-shape parameters. In the homoscedastic case it reduces to $1/(v+r)$, which is log-flat for the total variance rather than for the latent variance alone.

## ↑ Ancestors (9)

1. [Jeffreys prior](jeffreys-prior.md)
2. [Fisher information matrix](fisher-information-matrix.md)
3. [Informant function](informant-function.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/2/iv/solution.md)
