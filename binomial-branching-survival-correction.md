# Binomial branching survival correction

↑ **Parent:** [Binomial branching process](binomial-branching-process.md)

For $p=(1+\varepsilon)/n$, the [branching survival probability](survival-probability-of-a-branching-process.md) satisfies $1-\rho=(1-p\rho)^n$. If $(1+\varepsilon)^2<n$, comparison with a [Poisson branching process](poisson-branching-process.md) and expansion of the [logarithm](logarithm.md) give

$$
\frac{2\varepsilon}{1+2\varepsilon}\leq\rho\leq\frac{2\varepsilon}{1-(1+\varepsilon)^2/n}.
$$

For the upper bound use $\varepsilon=\sum_{j\geq1}(1-np^{j+1})\rho^j/(j+1)$ and retain its first nonnegative term. For fixed $n>1$, the leading term is instead $2n\varepsilon/(n-1)$. In particular $n=2$ gives $\rho=4\varepsilon/(1+\varepsilon)^2$, showing that the uncorrected exact bound $\rho\leq2\varepsilon$ is false for small positive $\varepsilon$.

For $0<\varepsilon\leq1/4$ and $n\varepsilon\geq2$, the uncorrected exact upper bound does hold for the [binomial branching process](binomial-branching-process.md). Here $np^2\leq\varepsilon$ and $np^3\leq1/4$, so at $x=2\varepsilon$ the first two terms of the nonnegative series give $\varepsilon(1-np^2)+(4/3)\varepsilon^2(1-np^3)\geq\varepsilon$. Monotonicity of that series yields $\rho\leq2\varepsilon$. This recovers the intended large-$n$ bracket without claiming it for every finite reproduction law.

## ↑ Ancestors (6)

1. [Binomial branching process](binomial-branching-process.md)
2. [Galton-Watson process](galton-watson-process.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Barely-supercritical largest-component expectation](barely-supercritical-largest-component-expectation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/4/ii/solution.md)
- [Survival probability of a branching process](survival-probability-of-a-branching-process.md)
