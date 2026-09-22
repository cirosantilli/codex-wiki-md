# Weighted interval testing for a piecewise-constant mean

↑ **Parent:** [Multiple hypothesis testing](multiple-hypothesis-testing.md)

Given valid [p-values](p-value.md) $q_J$ for constancy on intervals of length at least two, reject $I$ when $\max_{J\supseteq I}nq_J/|J|\leq\alpha$. Every rejected true interval forces rejection of its maximal constant block. A [union bound](boole-s-inequality.md) over the non-singleton maximal blocks gives [familywise error rate](familywise-error-rate.md) at most $\alpha$, since their lengths sum to at most $n$. Singleton blocks have no tested interval in this formulation.

## ↑ Ancestors (8)

1. [Multiple hypothesis testing](multiple-hypothesis-testing.md)
2. [Statistical hypothesis test](statistical-hypothesis-test.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-205/1/solution.md)
