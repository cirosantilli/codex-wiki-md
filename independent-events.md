# Independent events

↑ **Parent:** [Independent sigma-algebras](independent-sigma-algebras.md)

Events $A_1,\ldots,A_n$ are mutually independent when

$$
\mathbb P\left(\bigcap_{j\in J}A_j\right)
=\prod_{j\in J}\mathbb P(A_j)
$$

for every nonempty index subset $J\subseteq\{1,\ldots,n\}$. For two [events](event.md) and $\mathbb P(B)>0$, this is equivalent to $\mathbb P(A\mid B)=\mathbb P(A)$: learning whether $B$ occurred does not change the chance of $A$.

For independent uniform dice, the [events](event.md) that the first result is an [even integer](even-number.md) and that the second result is an [even integer](even-number.md) each have [probability](probability.md) $1/2$; their [intersection](set-intersection.md) has [probability](probability.md) $9/36=1/4$. In contrast, "first result is an [even integer](even-number.md)" and "first result is an [odd integer](odd-integer.md)" are [disjoint events](disjoint-events.md) of positive [probability](probability.md), so they cannot be [independent events](independent-events.md). Learning one occurred completely rules out the other.

[Pairwise independence](pairwise-independent-events.md) is weaker than mutual independence. Take two [independent](independent-random-variables.md) fair [bits](bit.md) $X,Y$. The three [events](event.md) $X=0$, $Y=0$, and $X=Y$ each have [probability](probability.md) $1/2$ and every pair has [intersection](set-intersection.md) [probability](probability.md) $1/4$. Their triple [intersection](set-intersection.md) is the single outcome $(0,0)$, of [probability](probability.md) $1/4$ rather than $1/8$. Checking pairs alone misses the joint constraint.

**Table of contents**

- [Pairwise-independent three-event avoidance](pairwise-independent-three-event-avoidance.md)

## ↑ Ancestors (6)

1. [Independent sigma-algebras](independent-sigma-algebras.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Boolean operations on events](boolean-operations-on-events.md)
- [Borel-Cantelli lemmas](borel-cantelli-lemmas.md)
- [Borel-Cantelli second lemma](borel-cantelli-second-lemma.md)
- [Conditional probability](conditional-probability.md)
- [Disjoint events](disjoint-events.md)
- [Equality in Boole's inequality](equality-in-boole-s-inequality.md)
- [Inclusion-exclusion principle for probabilities](inclusion-exclusion-principle-for-probabilities.md)
- [Independent events](independent-events.md)
- [Independent permissive gates in an ion channel](independent-permissive-gates-in-an-ion-channel.md)
- [Infinitely many heads as a tail event](infinitely-many-heads-as-a-tail-event.md)
- [Law of total probability](law-of-total-probability.md)
- [Limsup of events](limsup-of-events.md)
- [Pairwise independent events](pairwise-independent-events.md)
- [Pairwise-independent three-event avoidance](pairwise-independent-three-event-avoidance.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/9f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/9f/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1/25j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-13/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2/4f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-2/9e/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-2/12f/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-212/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/18/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/10/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1/16/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/10/a/solution.md)
- [Percolation theory](percolation-theory-split.md)
- [Rule of product](rule-of-product.md)
- [Summable and harmonic event probabilities](summable-and-harmonic-event-probabilities.md)
