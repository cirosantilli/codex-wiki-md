<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $A=g(X)$ and $B=g(Y)$. The two [conditional expectation](../../../../../conditional-expectation.md) identities supply a $\sigma(Y)$-[measurable](../../../../../measurability.md) version of $B$ and a $\sigma(X)$-[measurable](../../../../../measurability.md) version of $A$. Work with those versions, which do not change any [almost sure equality](../../../../../almost-sure-equality.md). Both lie in [L2 space](../../../../../l2-space-is-a-hilbert-space.md), and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) makes their product an [integrable random variable](../../../../../integrable-random-variable.md).

Testing the first [conditional expectation](../../../../../conditional-expectation.md) identity against $B$, and the second against $A$, gives

$$
\mathbb E[AB]=\mathbb E[B^2],\qquad
\mathbb E[AB]=\mathbb E[A^2].
$$

For completeness, these tests with unbounded multipliers are valid by first using the bounded truncations $B_m=(-m)\vee(B\wedge m)$ and $A_m=(-m)\vee(A\wedge m)$, then passing to the limit with the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and [convergence in L2](../../../../../convergence-in-l2.md). Consequently,

$$
\mathbb E[(A-B)^2]=\mathbb E[A^2]+\mathbb E[B^2]-2\mathbb E[AB]=0.
$$

A nonnegative [random variable](../../../../../random-variable-split.md) with zero [expected value](../../../../../expected-value-split.md) vanishes [almost surely](../../../../../almost-sure-convergence.md). Therefore **$g(X)=g(Y)$ almost surely**. This is [mutual conditional expectation rigidity in L2](../../../../../mutual-conditional-expectation-rigidity-in-l2.md); it also follows from the [equality case for conditional second moments](../../../../../equality-case-for-conditional-second-moments.md).

For a counterexample to equality of the original [random variables](../../../../../random-variable-split.md), let $X$ give [probability](../../../../../probability.md) $1/4$ to each of $-2,-1,1,2$, set $Y=-X$, and use the nonconstant [function](../../../../../function-split.md) $g(t)=t^2$. Then $g(X)=g(Y)=X^2$ takes both values $1$ and $4$. It is [measurable](../../../../../measurability.md) with respect to both generated [sigma-algebras](../../../../../sigma-algebra.md), so both required [conditional expectation](../../../../../conditional-expectation.md) identities hold. Symmetry gives $\mathbb EX=\mathbb EY=0$, while neither [random variable](../../../../../random-variable-split.md) can be zero. Thus

$$
\boxed{\mathbb P(X=\mathbb EX)=\mathbb P(Y=\mathbb EY)=0,\qquad\mathbb P(X=Y)=0.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
