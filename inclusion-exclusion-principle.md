# Inclusion-exclusion principle

↑ **Parent:** [Combinatorics](combinatorics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inclusion-exclusion_principle)

For [finite sets](finite-set.md) $A_1,\ldots,A_n$, the cardinality of their [union](set-union.md) is

$$
\left|\bigcup_{i=1}^n A_i\right|=\sum_{\varnothing\neq J\subseteq\{1,\ldots,n\}}(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.
$$

Add the individual [cardinalities](cardinality.md), subtract pairwise [intersection](set-intersection.md) counts, add triple [intersection](set-intersection.md) counts, and continue alternating. This is useful whenever one object can satisfy several conditions: a search result can match several filters, or a [permutation](permutation.md) can have several forbidden [fixed points](fixed-point.md).

Among the [integers](integer.md) from 1 to 30, let $A$ contain the multiples of 2 and $B$ the multiples of 3. Then $|A|=15$, $|B|=10$, and $|A\cap B|=5$, because their common multiples are the multiples of 6. The naive sum $25$ counts those five twice; the correct [union](set-union.md) size is **$15+10-5=20$**. The regions contain ten in $A$ alone, five in both, five in $B$ alone, and ten in neither.

<a id="image-subtracting-overlap-counts-each-selected-integer-once-a-third-divisibility-condition-requires-adding-the-triple-overlap-back"></a>
![](inclusion-exclusion-counting.png)

**[Figure 21](#image-subtracting-overlap-counts-each-selected-integer-once-a-third-divisibility-condition-requires-adding-the-triple-overlap-back). Subtracting overlap counts each selected integer once; a third divisibility condition requires adding the triple overlap back**.

Add a third [set](set-split.md) $C$ containing the multiples of 5. Its size is 6; the three pairwise [intersections](set-intersection.md) have sizes $5,3,2$; and the triple [intersection](set-intersection.md) contains only 30. The [inclusion-exclusion principle](inclusion-exclusion-principle.md) gives **$15+10+6-5-3-2+1=22$** integers divisible by at least one of 2, 3, and 5.

The alternating corrections have a local explanation. An object belonging to exactly $r\geq1$ of the [sets](set-split.md) is counted $\binom r1-\binom r2+\cdots+(-1)^{r+1}\binom rr=1$ times, by the [binomial theorem](binomial-theorem.md) applied to $(1-1)^r$. An object in none contributes zero. Thus overlapping descriptions are repaired without requiring the [sets](set-split.md) themselves to be disjoint. For [probability](probability.md), the same calculation applies to event probabilities in place of [cardinalities](cardinality.md), giving the [inclusion-exclusion principle for probabilities](inclusion-exclusion-principle-for-probabilities.md).

**Table of contents**

- [Inclusion-exclusion principle for probabilities](inclusion-exclusion-principle-for-probabilities.md)
- [Weighted inclusion-exclusion principle](weighted-inclusion-exclusion-principle.md)
- [Inclusion-exclusion for exact block occupancy](inclusion-exclusion-for-exact-block-occupancy.md)
- [Cyclic difference constraints](cyclic-difference-constraints.md)
- [Bonferroni inequalities](bonferroni-inequalities.md)
  - [Jordan-Bonferroni exact-occurrence inequalities](jordan-bonferroni-exact-occurrence-inequalities.md)

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (58)

- [Asymmetric Dirichlet hyperbola split](asymmetric-dirichlet-hyperbola-split.md)
- [Avoidance probabilities determine a simple chordal curve law](avoidance-probabilities-determine-a-simple-chordal-curve-law.md)
- [Binary relations with no empty row or column](binary-relations-with-no-empty-row-or-column.md)
- [Bonferroni inequalities](bonferroni-inequalities.md)
- [Bounded weak compositions](bounded-weak-compositions.md)
- [Combinatorics](combinatorics-split.md)
- [Cyclic difference constraints](cyclic-difference-constraints.md)
- [Cyclic digit run](cyclic-digit-run.md)
- [Derangement of a permutation](derangement-of-a-permutation.md)
- [Dirichlet hyperbola method](dirichlet-hyperbola-method.md)
- [Exchangeable invariant laws of symmetric exclusion](exchangeable-invariant-laws-of-symmetric-exclusion.md)
- [Finite additivity of a set function](finite-additivity-of-a-set-function.md)
- [Fixed point count of a uniform random permutation](fixed-point-count-of-a-uniform-random-permutation.md)
- [Inclusion-exclusion principle](inclusion-exclusion-principle.md)
- [Inclusion-exclusion principle for probabilities](inclusion-exclusion-principle-for-probabilities.md)
- [Jordan's totient function](jordan-s-totient-function.md)
- [Kolmogorov axioms](kolmogorov-axioms.md)
- [Legendre prime-counting formula](legendre-prime-counting-formula.md)
- [Mark and recapture](mark-and-recapture.md)
- [Pairwise-independent three-event avoidance](pairwise-independent-three-event-avoidance.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4/6f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4/6f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4/6f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-28/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-4/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-4/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/12/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-37/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-4/5e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/11/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-13/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-13/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-39/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-4/6e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/7e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/7e/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-10/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-4/6e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-4/6e/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/8e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/8e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-203/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-4/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4/6e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-4/6e/b/solution.md)
- [Percolation theory](percolation-theory.md)
- [Probability measure](probability-measure.md)
- [Stars and bars (combinatorics)](stars-and-bars-combinatorics.md)
- [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md)
