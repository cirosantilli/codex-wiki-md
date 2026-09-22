# Segregating-site likelihood under the neutral coalescent

↑ **Parent:** [Infinite sites mutation model](infinite-sites-mutation-model.md)

For $n\ge2$, the [probability generating function](probability-generating-function.md) of the segregating-site count conditional on mutation parameter $\theta$ is

$$
E[z^S\mid\theta]=\prod_{i=1}^{n-1}\frac{i}{i+\theta(1-z)}.
$$

This follows by integrating the Poisson generating function over the independent exponential epoch lengths. With $W=L/2$, its density is $(n-1)e^{-w}(1-e^{-w})^{n-2}$. Expanding the binomial factor and integrating $w^k e^{-(\theta+r+1)w}$ gives

$$
P(S=k\mid\theta)=(n-1)\theta^k\sum_{r=0}^{n-2}\frac{(-1)^r\binom{n-2}{r}}{(\theta+r+1)^{k+1}}.
$$

For $k=0$ use $\theta^0=1$, including at $\theta=0$. A posterior density divided by a positive prior density is proportional to this likelihood, allowing posterior simulation output to estimate its maximizer.

## ↑ Ancestors (5)

1. [Infinite sites mutation model](infinite-sites-mutation-model.md)
2. [Population genetics](population-genetics.md)
3. [Genetics](genetics.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45/3/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-45/4/g/solution.md)
- [Watterson estimator](watterson-estimator.md)
