# Lebesgue inner measure

↑ **Parent:** [Lebesgue measure](lebesgue-measure.md)

The [Lebesgue inner measure](lebesgue-inner-measure.md) approximates a subset of the real line from within by [compact sets](compact-space.md), while [Lebesgue outer measure](lebesgue-outer-measure.md) approximates it from outside by countable interval covers. For a finite closed interval $I$ containing $E$,

$$
m_*(E)=m(I)-m^*(I\setminus E).
$$

Indeed, every compact $K\subseteq E$ gives $m^*(I\setminus E)\leq m(I)-m(K)$. Conversely, an open cover of $I\setminus E$ with total length arbitrarily close to its [outer measure](outer-measure.md) has compact complement in $I$ lying inside $E$, giving the reverse inequality in the limit.

For $m^*(E)<\infty$, equality of inner and outer measures holds precisely when $E$ is [Lebesgue measurable](lebesgue-measurable-set.md). For an unbounded set, measurability is equivalently checked on all bounded intersections $E\cap[-n,n]$. Equality $m_*(E)=m^*(E)=\infty$ alone is insufficient: adjoining a bounded nonmeasurable subset to a disjoint half-line makes both quantities infinite without making the union measurable.

## ↑ Ancestors (8)

1. [Lebesgue measure](lebesgue-measure.md)
2. [Sigma-finite uniqueness theorem for measures](sigma-finite-uniqueness-theorem-for-measures.md)
3. [Measure theory](measure-theory-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Lebesgue inner measure](lebesgue-inner-measure.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2011/d/1/a/solution.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-i-course-of-the-university-of-oxford/2011/d/1/a/solution.md)
