# Uniform almost-sure fluid limit of the SI model

↑ **Parent:** [SI model](si-model.md)

The stochastic [SI model](si-model.md) with susceptible fraction $X_n$, initial limit $a$, and total infection rate $n\lambda X_n(1-X_n)$ has deterministic limit

$$
x(t)=\frac{ae^{-\lambda t}}{1-a+ae^{-\lambda t}}.
$$

The [Poisson time-change representation of a Markov chain](poisson-time-change-representation-of-a-markov-chain.md) writes $X_n$ as its integrated drift minus a centered Poisson error. On $[0,T]$ its clock is at most $n\lambda T/4$. The [Poisson maximal concentration bound](poisson-maximal-concentration-bound.md) makes every fixed error tolerance have summable probabilities in $n$, so the [Borel-Cantelli lemma](borel-cantelli-lemmas.md) gives uniform error decay [almost surely](almost-sure-convergence.md). The [Gronwall inequality](gronwall-inequality.md) transfers that decay to $X_n-x$, because the drift is [Lipschitz continuous](lipschitz-continuity.md). The assertion is for fixed finite intervals and does not claim approximation over times growing with $n$.

## ↑ Ancestors (6)

1. [SI model](si-model.md)
2. [Compartmental models (epidemiology)](compartmental-models-epidemiology.md)
3. [Mathematical biology](mathematical-biology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-36/1/b/solution.md)
