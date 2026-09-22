# Non-measurable set

↑ **Parent:** [Measure theory](measure-theory-split.md)

A [subset](subset.md) $A$ of a [measurable space](measurable-space.md) $(X,\Sigma)$ is non-measurable when $A\notin\Sigma$. On the [real line](real-line.md), unless another [sigma-algebra](sigma-algebra.md) is specified, this commonly means that $A$ is not a [Lebesgue measurable set](lebesgue-measurable-set.md). By [completeness of Lebesgue measure](completeness-of-lebesgue-measure.md), such a set cannot be contained in a [Lebesgue null set](lebesgue-null-set.md).

For an example, use the [axiom of choice](axiom-of-choice.md) to select one representative from each equivalence class of $[0,1]$ under $x\sim y$ if $x-y\in\mathbb Q$, and call the resulting set $V$. The translates $V+q$, for $q\in\mathbb Q\cap[-1,1]$, are pairwise disjoint, their union contains $[0,1]$, and their union is contained in $[-1,2]$. If $V$ were a [Lebesgue measurable set](lebesgue-measurable-set.md), translation invariance and countable additivity would make that union have measure zero when $m(V)=0$ and infinite measure when $m(V)>0$. Both conclusions contradict these inclusions. Thus $V$ is non-measurable.

## ↑ Ancestors (6)

1. [Measure theory](measure-theory-split.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Lebesgue measurable sections](lebesgue-measurable-sections.md)
- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2023/1/c/i/solution.md)
