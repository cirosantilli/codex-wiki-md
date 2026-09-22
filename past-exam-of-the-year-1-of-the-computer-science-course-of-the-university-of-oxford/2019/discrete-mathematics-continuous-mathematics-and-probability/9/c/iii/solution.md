<h1 id="9/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Represent the removed half as the first $m=500$ cards in a uniformly random ordering. Every unordered half is then equally likely. Let $X_1,\ldots,X_{500}$ be their values. Each has mean zero and [variance](../../../../../../variance-split.md) one, and every distinct pair has [covariance](../../../../../../covariance.md) $-1/999$ by the same ordered-pair argument as in (ii).

The general [covariance](../../../../../../covariance.md) expansion from (b), applied without imposing [independence](../../../../../../independent-random-variables.md), gives

$$
\boxed{\mathbb E[Z]=0,\qquad
\operatorname{Var}(Z)=500-\frac{500\cdot499}{999}
=\frac{250000}{999}.}
$$

This is the [finite population correction](../../../../../../finite-population-correction.md) for a half-sample; treating the draws as [independent](../../../../../../independent-random-variables.md) would give the wrong [variance](../../../../../../variance-split.md).

Finally $\{Z\ge50\}\subseteq\{|Z|\ge50\}$, so [Chebyshev's inequality](../../../../../../chebyshev-s-inequality.md) yields

$$
\boxed{\mathbb P(Z\ge50)\le
\frac{\operatorname{Var}(Z)}{50^2}
=\frac{250000}{999\cdot2500}
=\frac{100}{999}.}
$$

The cards returned before this sampling step restore the original population; no conditioning on the earlier two observed values is imposed.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
