# Kolmogorov axioms

↑ **Parent:** [Probability measure](probability-measure.md)

The [Kolmogorov axioms](kolmogorov-axioms.md) describe a consistent way to assign [probabilities](probability.md) to [events](event.md). Start with a [sample space](sample-space.md) $\Omega$ and an [event](event.md) [sigma-algebra](sigma-algebra.md) $\mathcal F$: it contains $\Omega$ and is closed under [complements](complement-of-a-set.md) and countable [unions](set-union.md), hence also countable [intersections](set-intersection.md). The [probability measure](probability-measure.md) is a [function](function-split.md) $\mathbb P:\mathcal F\to\mathbb R$ satisfying

$$
\begin{aligned}
&\mathbb P(A)\geq0 &&\text{for every }A\in\mathcal F,\\
&\mathbb P(\Omega)=1,\\
&\mathbb P\left(\bigcup_{j=1}^{\infty}A_j\right)
=\sum_{j=1}^{\infty}\mathbb P(A_j)
&&\text{if }A_i\cap A_j=\varnothing\text{ for }i\ne j.
\end{aligned}
$$

The triple $(\Omega,\mathcal F,\mathbb P)$ is a [probability space](probability-space.md). The third axiom is [countable additivity](countable-additivity.md); the infinite [series](series-mathematics.md) means the [limit of a sequence](limit-of-a-sequence.md) of nonnegative partial sums. It applies to pairwise [disjoint events](disjoint-events.md), not to overlapping [events](event.md) and not to arbitrary uncountable [unions](set-union.md).[Introduction to Probability, Lecture 1: Probability Models and Axioms by John Tsitsiklis and others](introduction-to-probability-lecture-1-probability-models-and-axioms-by-john-tsitsiklis-and-others.md)

The [sigma-algebra](sigma-algebra.md) specifies which questions have [probabilities](probability.md), while the axioms specify how those [probabilities](probability.md) fit together. For a finite [sample space](sample-space.md) one can take the entire [power set](power-set.md); a continuous model commonly uses a [Borel sigma-algebra](borel-sigma-algebra.md). Nonnegativity and normalization do not require equally likely outcomes or [independence](independent-random-variables.md): those are additional modelling choices.

For an exact six-outcome model, take $\Omega=\{1,2,3,4,5,6\}$, $\mathcal F=\mathcal P(\Omega)$, and assign $\mathbb P(\{k\})=k/21$. The total is one because $1+2+3+4+5+6=21$. Define the [probability](probability.md) of an [event](event.md) by summing the weights of its outcomes. The [disjoint events](disjoint-events.md) $A=\{1,2\}$, $B=\{3,4\}$ and $C=\{5,6\}$ form a [partition of a set](partition-of-a-set.md) with

$$
\mathbb P(A)=\frac3{21},\qquad \mathbb P(B)=\frac7{21},\qquad
\mathbb P(C)=\frac{11}{21},\qquad
\mathbb P(A\cup B)=\frac{10}{21}=1-\mathbb P(C).
$$

This is a specified mathematical model, not measured die frequencies. The figure makes [probability](probability.md) literal area: each region has the same height and a width proportional to its assigned mass. Regrouping [disjoint events](disjoint-events.md) preserves their total area.

<a id="image-exact-six-outcome-model-with-masses-k-21-grouping-disjoint-outcomes-adds-their-probability-areas"></a>
![](probability-axioms-continuity-weighted-partition.png)

**[Figure 14](#image-exact-six-outcome-model-with-masses-k-21-grouping-disjoint-outcomes-adds-their-probability-areas). Exact six-outcome model with masses k/21: grouping disjoint outcomes adds their probability areas**.

Several familiar rules are consequences, not further axioms. [Finite additivity of a set function](finite-additivity-of-a-set-function.md) follows by appending empty [events](event.md) to the sequence in [countable additivity](countable-additivity.md); $\mathbb P(\varnothing)=0$ follows already by writing $\Omega=\Omega\cup\varnothing$ as a disjoint [union](set-union.md). The [complement rule of probability](complement-rule-of-probability.md) gives $\mathbb P(A^c)=1-\mathbb P(A)$ and therefore $0\leq\mathbb P(A)\leq1$. Splitting larger [events](event.md) into a smaller [event](event.md) and a [set difference](set-difference.md) shows $A\subseteq B\Rightarrow\mathbb P(A)\leq\mathbb P(B)$.

For overlapping [events](event.md), the [inclusion-exclusion principle](inclusion-exclusion-principle.md) corrects double counting:

$$
\mathbb P(D\cup E)=\mathbb P(D)+\mathbb P(E)-\mathbb P(D\cap E).
$$

In the six-outcome model, $D=\{2,3\}$ and $E=\{3,4\}$ give $5/21+7/21-3/21=9/21$, agreeing with the weight of $\{2,3,4\}$. This decomposition is useful because a complicated [event](event.md) can be assembled from simpler questions with known [probabilities](probability.md).

On a finite [sample space](sample-space.md), a family of pairwise [disjoint events](disjoint-events.md) has only finitely many nonempty members, so [finite additivity of a set function](finite-additivity-of-a-set-function.md) already handles every countable disjoint [union](set-union.md). On an infinite [sample space](sample-space.md), the countable axiom additionally controls what is left beyond every finite stage. In the fair-coin waiting model of [continuity of probability](continuity-of-probability.md), the finite-stage calculations $\mathbb P(\text{first head at toss }j)=2^{-j}$ sum to $1-2^{-n}$ through toss $n$. [Countable additivity](countable-additivity.md) makes the [probability](probability.md) of a head at some finite toss equal to $\sum_{j\geq1}2^{-j}=1$; finite-stage sums alone do not justify that passage. For the [continuous uniform distribution](continuous-uniform-distribution.md) on $[0,1]$, each [singleton](singleton-mathematics.md) instead has [probability](probability.md) zero, while their uncountable [union](set-union.md) has [probability](probability.md) one. Countable, rather than unrestricted, additivity accommodates both models.

Historically, Kolmogorov's 1933 book _[Grundbegriffe der Wahrscheinlichkeitsrechnung](grundbegriffe-der-wahrscheinlichkeitsrechnung-by-andrei-n-kolmogorov.md)_ established the influential axiomatic framework connecting [probability theory](probability-theory-split.md) with [measure theory](measure-theory-split.md). The three conditions above are the modern presentation on a [sigma-algebra](sigma-algebra.md). Shafer and Vovk's historical study explains that the original presentation began with finite additivity on an [algebra of sets](algebra-of-sets.md) and added continuity for decreasing [events](event.md) with empty [intersection](set-intersection.md), which supplies the countable extension.[The Sources of Kolmogorov’s Grundbegriffe by Glenn Shafer and others](the-sources-of-kolmogorov%E2%80%99s-grundbegriffe-by-glenn-shafer-and-others.md)

## ↑ Ancestors (7)

1. [Probability measure](probability-measure.md)
2. [Probability space](probability-space.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Complement rule of probability](complement-rule-of-probability.md)
- [Kolmogorov axioms](kolmogorov-axioms.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-2/9f/a/solution.md)
- [Probability theory](probability-theory-split.md)
