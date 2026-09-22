<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [measurable space](../../../../measurable-space.md) is a pair $(\Omega,\mathcal F)$ where $\mathcal F$ is a [sigma-algebra](../../../../sigma-algebra.md) of [subsets](../../../../subset.md) of $\Omega$: it contains $\Omega$, is closed under [complements](../../../../complement-of-a-set.md) relative to $\Omega$, and is closed under [countable unions](../../../../countable-union.md). A [measure](../../../../measure-split.md) on it is a [function](../../../../function-split.md) $\mu:\mathcal F\to[0,\infty]$ with $\mu(\varnothing)=0$ and [countable additivity](../../../../countable-additivity.md):

$$
\mu\left(\bigcup_{n=1}^{\infty}A_n\right)=\sum_{n=1}^{\infty}\mu(A_n)
$$

whenever the [measurable sets](../../../../measurable-set.md) $A_n$ are pairwise [disjoint](../../../../disjoint-sets.md). Infinite values are allowed. The triple $(\Omega,\mathcal F,\mu)$ is a [measure space](../../../../measure-space.md).

Because $E\in\mathcal F$, the family $\mathcal F_E$ contains $E$. If $A\in\mathcal F_E$, then $E\setminus A=E\cap(\Omega\setminus A)$ belongs to $\mathcal F$ and is a [subset](../../../../subset.md) of $E$, so it belongs to $\mathcal F_E$. If each $A_n\in\mathcal F_E$, their [countable union](../../../../countable-union.md) belongs to $\mathcal F$ and remains a [subset](../../../../subset.md) of $E$. Thus **$\mathcal F_E$ is a [sigma-algebra](../../../../sigma-algebra.md) on $E$**, with relative [complements](../../../../complement-of-a-set.md) taken in $E$, not in $\Omega$.

Equivalently,

$$
\mathcal F_E=\{E\cap B:B\in\mathcal F\},
$$

the [trace sigma-algebra](../../../../trace-sigma-algebra.md) on the [measurable set](../../../../measurable-set.md) $E$. The measurability of $E$ is what makes this equal to the family in the question.

The [function](../../../../function-split.md) $\nu$ takes values in $[0,\infty]$ and has $\nu(\varnothing)=0$. For any pairwise [disjoint](../../../../disjoint-sets.md) $A_n\in\mathcal F_E$, [countable additivity](../../../../countable-additivity.md) of $\mu$ gives

$$
\nu\left(\bigcup_nA_n\right)=\mu\left(\bigcup_nA_n\right)
=\sum_n\mu(A_n)=\sum_n\nu(A_n).
$$

Therefore **$\nu$ is a [measure](../../../../measure-split.md) on $(E,\mathcal F_E)$**: it is the [restriction of a measure to a measurable subset](../../../../restriction-of-a-measure-to-a-measurable-subset.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
