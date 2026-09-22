# Progressive illness-death model

↑ **Parent:** [Continuous-time multi-state model](continuous-time-multi-state-model.md)

This [continuous-time multi-state model](continuous-time-multi-state-model.md) permits progression $1\to2$, direct death $1\to3$, and death after progression $2\to3$, with no recovery and death an [absorbing state](absorbing-state.md). For constant positive rates $a,b,c$, write $\lambda=a+b$. Integrating over the time of the progression arrow gives

$$
p_{12}(t)=\int_0^t e^{-\lambda u}a e^{-c(t-u)}\,du
=\frac{a(e^{-ct}-e^{-\lambda t})}{\lambda-c}.
$$

Use $at e^{-ct}$ when $\lambda=c$. The other [transition probabilities](transition-probability.md) are $p_{11}=e^{-\lambda t}$, $p_{13}=1-p_{11}-p_{12}$, $p_{22}=e^{-ct}$, $p_{23}=1-e^{-ct}$ and $p_{33}=1$. Unlike a purely sequential [irreversible three-state disease model](irreversible-three-state-disease-model.md), the direct-death rate contributes to the first-state exit rate. A [mixed panel and exact-death likelihood](mixed-panel-and-exact-death-likelihood.md) accounts for panel visits and exact death times with different kinds of factors.

## ↑ Ancestors (6)

1. [Continuous-time multi-state model](continuous-time-multi-state-model.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/6/b/i/solution.md)
