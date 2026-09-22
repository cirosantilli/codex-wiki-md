<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [law of total expectation](../../../../../../law-of-total-expectation.md) gives $\mathbb E Y=\mathbb E[X/2]=q/(2p)$. The [law of total variance](../../../../../../law-of-total-variance.md) separates the two sources of randomness:

$$
\operatorname{Var}(Y)
=\mathbb E[\operatorname{Var}(Y\mid X)]
+\operatorname{Var}(\mathbb E[Y\mid X])
=\frac14\mathbb E X+\frac14\operatorname{Var}(X).
$$

Substitution gives

$$
\boxed{\mathbb E Y=\frac{1-p}{2p},\qquad
\operatorname{Var}(Y)=\frac{q(p+1)}{4p^2}
=\frac{1-p^2}{4p^2}.}
$$

The [binomial thinning of a geometric random variable](../../../../../../binomial-thinning-of-a-geometric-random-variable.md) identity supplies a further check: $Y$ itself has a zero-based [geometric distribution](../../../../../../geometric-distribution.md) with success [probability](../../../../../../probability.md) $2p/(1+p)$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
