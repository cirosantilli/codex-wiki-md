# Autologistic binary-image model

↑ **Parent:** [Markov random field](markov-random-field.md)

On a graph, a binary configuration has probability proportional to $\exp(\alpha\sum_v x_v+\beta\sum_{\{v,w\}}x_vx_w)$, with each edge counted once. The full [conditional probability](conditional-probability.md) of a one is logistic with [linear predictor](linear-predictor.md) $\alpha+\beta\sum_{w\sim v}x_w$. Local neighbor sums eliminate the need to evaluate the [normalizing constant](normalizing-constant.md).

**Table of contents**

- [Gaussian-noise posterior for an autologistic image](gaussian-noise-posterior-for-an-autologistic-image.md)

## ↑ Ancestors (7)

1. [Markov random field](markov-random-field.md)
2. [Probabilistic graphical model](probabilistic-graphical-model.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-38/4/solution.md)
