<h1 id="26k/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The event $\{X_n=1\}$ is $T^{-n}(0,1/2)$. Since $T^n$ has $2^n$ affine branches of slope magnitude $2^n$, this preimage is, up to endpoints, a disjoint union of $2^n$ intervals of length $2^{-(n+1)}$ and has measure $1/2$.

More generally, for every binary word $(a_0,\ldots,a_{N-1})$, its [itinerary cylinder](../../../../../../../itinerary-cylinder.md)

$$
C(a_0,\ldots,a_{N-1})
=\{x:X_0(x)=a_0,\ldots,X_{N-1}(x)=a_{N-1}\}
$$

is, up to finitely many endpoints, one monotonicity interval of $T^N$ and has measure $2^{-N}$. Therefore

$$
m(C(a_0,\ldots,a_{N-1}))
=\prod_{j=0}^{N-1}m(X_j=a_j),
$$

so the $X_n$ are [independent and identically distributed random variables](../../../../../../../independent-and-identically-distributed-random-variables.md), each with the [Bernoulli distribution](../../../../../../../bernoulli-distribution.md) of parameter $1/2$.

The finite itinerary cylinders have diameters at most $2^{-N}$. Their endpoints form a dense set, so their unions generate the [Borel sigma-algebra](../../../../../../../borel-sigma-algebra.md) after [completion](../../../../../../../completion-of-a-measure.md) by null sets. Thus

$$
\sigma(X_0,X_1,\ldots)=\mathcal A
$$

in the standard probability-space convention that σ-algebras are identified modulo null sets.

There is a small literal endpoint defect in the uncompleted formulation of the question: $0$, $1$, and $2/3$ all have the all-zero itinerary, so $\sigma(X_0,X_1,\ldots)$ cannot separate these Borel singletons. Consequently the displayed equality is false as an equality of raw Borel σ-algebras with the stated open interval, but it is true after completion and modulo null sets, which is the version used in the ergodicity argument.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [26K](../../../26k.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
