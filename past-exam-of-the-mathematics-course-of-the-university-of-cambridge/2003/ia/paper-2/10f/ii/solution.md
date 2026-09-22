<h1 id="10f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Independence requires each joint [probability](../../../../../../probability.md) to equal the product of the relevant marginals. In particular it implies $d=(c+d)(b+d)$, equivalent to $ad=bc$.

Conversely let $p=c+d$ and $q=b+d$, and assume $ad=bc$. The [covariance](../../../../../../covariance.md) calculation gives $d=pq$. Then

$$
c=p-d=p(1-q),\qquad b=q-d=(1-p)q,\qquad a=1-b-c-d=(1-p)(1-q).
$$

All four joint [probabilities](../../../../../../probability.md) therefore factor, proving [independence](../../../../../../independent-random-variables.md). Hence

$$
\boxed{X,Y\text{ independent}\ \Longleftrightarrow\ ad=bc
\ \Longleftrightarrow\ X,Y\text{ uncorrelated}.}
$$

This is [Bernoulli independence from zero covariance](../../../../../../bernoulli-independence-from-zero-covariance.md), including degenerate marginals. It is special to two-point variables and is not a general equivalence for arbitrary random variables.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
