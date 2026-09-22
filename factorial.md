# Factorial

↑ **Parent:** [Combinatorics](combinatorics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Factorial)

For a [nonnegative integer](natural-number.md) $n$, the [factorial](factorial.md) $n!$ is the [product](product-of-numbers.md) of the [positive integers](positive-integer.md) from $1$ to $n$, with the [empty product](empty-product.md) equal to $1$:

$$
n!=\prod_{j=1}^{n}j,\qquad 0!=1.
$$

Thus $1!=1$, $2!=2$, $3!=6$, $4!=24$ and $5!=120$. The [factorial](factorial.md) counts the [permutations](permutation.md) of $n$ distinct objects: arranging $A,B,C$ gives exactly $ABC,ACB,BAC,BCA,CAB,CBA$. The choice tree in [permutation](permutation.md) shows the three choices for the first position, two for the second, and one for the last.

The value $0!=1$ has a counting explanation: the [empty set](empty-set.md) has exactly one ordering, the empty list. Equivalently, it has exactly one [bijection](bijection.md) to itself, the empty [function](function-split.md). There are no choices to make, and one completed outcome. The [factorial](factorial.md) therefore obeys the [recurrence relation](recurrence-relation.md)

$$
0!=1,\qquad n!=n(n-1)!\quad(n\geq1).
$$

The useful distinction is how many positions are filled. For [integers](integer.md) $0\leq k\leq n$, choosing and ordering $k$ distinct objects by [sampling without replacement](sampling-without-replacement.md) gives the [falling factorial](falling-factorial.md), while choosing an unordered $k$-element [subset](subset.md) gives the [binomial coefficient](binomial-coefficient.md):

$$
\underbrace{n(n-1)\cdots(n-k+1)}_{k\text{ factors}}=\frac{n!}{(n-k)!},\qquad
\binom nk=\frac{n!}{k!(n-k)!}.
$$

For five people, assigning captain and deputy gives $5!/3!=20$ outcomes; choosing a two-person team gives $\binom52=10$. Every team has exactly $2!$ assignments of the two roles, explaining the division. When $k=0$, both counts are one. The [factorial](factorial.md) is useful here because one count of full orderings yields both formulas by cancellation and by forgetting order. [OpenStax, College Algebra 2e, section 9.5: counting ordered selections and combinations](https://openstax.org/books/college-algebra-2e/pages/9-5-counting-principles)

Distinctness matters. If the two copies of $A$ in $AAB$ are indistinguishable, the visible arrangements are just $AAB,ABA,BAA$, numbering $3!/2!=3$. Temporarily labelling them $A_1,A_2$ gives six [permutations](permutation.md), but exchanging the two labels leaves each visible word unchanged, so every word was counted $2!$ times.

**Proof outline.** For $n\geq1$, choose the first object in $n$ ways, then order the remaining $n-1$ objects in $(n-1)!$ ways. The [rule of product](rule-of-product.md) gives the [recurrence relation](recurrence-relation.md); repeated application gives the displayed [product](product-of-numbers.md), starting from the one empty ordering. This explains why the [factorial](factorial.md) grows quickly: every additional distinct object introduces another multiplicative factor.

**Table of contents**

- [Double factorial](double-factorial.md)
- [Falling factorial](falling-factorial.md)
- [Rising factorial](rising-factorial.md)

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (49)

- [Asymptotic equivalence](asymptotic-equivalence.md)
- [Bernoulli number](bernoulli-number.md)
- [Binomial coefficient](binomial-coefficient.md)
- [Boltzmann entropy of a two-box occupancy](boltzmann-entropy-of-a-two-box-occupancy.md)
- [Comparison sorting lower bound](comparison-sorting-lower-bound.md)
- [Correlation function of a point process](correlation-function-of-a-point-process.md)
- [Cyclic permutation](cyclic-permutation.md)
- [Double counting (proof technique)](double-counting-proof-technique.md)
- [Empty product](empty-product.md)
- [Exponential generating function](exponential-generating-function.md)
- [Factorial](factorial.md)
- [Factorial graph formula via remainder coding](factorial-graph-formula-via-remainder-coding.md)
- [Gamma function](gamma-function.md)
- [Generating function](generating-function.md)
- [Hasse derivative](hasse-derivative.md)
- [Hockey-stick identity](hockey-stick-identity.md)
- [Hook-length formula](hook-length-formula.md)
- [Legendre's formula](legendre-s-formula.md)
- [Maclaurin series](maclaurin-series.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/7e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/7e/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4/7b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-22/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-4/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/12/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-53/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/2e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-4/6e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4/6d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-31/1/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4/1e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4/8e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/5d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/5d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-304/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/40c/d/solution.md)
- [Permanent (mathematics)](permanent-mathematics.md)
- [Permutation](permutation.md)
- [Size of a type class](size-of-a-type-class.md)
- [Stirling formula](stirling-formula.md)
- [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md)
- [Taylor polynomial](taylor-polynomial.md)
- [Taylor series](taylor-series.md)
- [Uniform order statistic](uniform-order-statistic.md)
- [Wilson's theorem](wilson-s-theorem.md)
