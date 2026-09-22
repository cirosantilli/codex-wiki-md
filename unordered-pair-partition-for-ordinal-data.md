# Unordered-pair partition for ordinal data

↑ **Parent:** [Ordinal categorical variable](ordinal-categorical-variable.md)

For $n$ observations of two ordered variables, every unordered pair is concordant, discordant, tied only on the first variable, tied only on the second variable, or tied on both. Consequently

$$
\binom n2=C+D+T_X+T_Y+T_{XY}.
$$

The proof is an exhaustive partition: if neither coordinate is tied the two nonzero comparison signs agree or disagree; otherwise exactly one or both coordinates are tied. For contingency-table counts $n_{ij}$ with row totals $n_{i+}$ and column totals $n_{+j}$,

$$
T_{XY}=\sum_{ij}\binom{n_{ij}}2,\quad T_X=\sum_i\binom{n_{i+}}2-T_{XY},\quad T_Y=\sum_j\binom{n_{+j}}2-T_{XY}.
$$

Two records tied on both variables belong to each marginal tie total, so subtracting them once from each produces the exclusive $T_X,T_Y$. Using incompatible exclusive and inclusive conventions corrupts [Somers' D](somers-d.md) and [Kendall's tau-b](kendall-s-tau-b.md) even if the untied concordances are correct. The identities also provide a direct arithmetic check on a printed statistical summary.

## ↑ Ancestors (8)

1. [Ordinal categorical variable](ordinal-categorical-variable.md)
2. [Categorical variable](categorical-variable.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2020/3/solution.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2020/5/solution.md)
