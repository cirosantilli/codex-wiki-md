# Empty-box indicators in uniform allocation

↑ **Parent:** [Uniform balls-in-bins allocation](uniform-balls-in-bins-allocation.md)

Place $n\ge1$ balls independently and uniformly into $m\ge2$ boxes. If $I_i$ indicates that box $i$ is empty, then $\mathbb E I_i=p$, $\operatorname{var}(I_i)=p(1-p)$, and, for $i\ne j$,

$$
\operatorname{cov}(I_i,I_j)=q-p^2<0.
$$

Indeed all balls avoid one specified box with [probability](probability.md) $p$ and two specified boxes with [probability](probability.md) $q$. The [indicator random variable](indicator-random-variable.md) identities give the [expectations](expected-value-split.md), [variances](variance-split.md), and [covariance](covariance.md). Finally $1-2/m<(1-1/m)^2$ proves strict negativity. Thus the number $K$ of empty boxes has $\mathbb E K=mp$ and $\operatorname{var}(K)=mp(1-p)+m(m-1)(q-p^2)$ by the [variance of a sum](variance-of-a-sum.md).

## ↑ Ancestors (9)

1. [Uniform balls-in-bins allocation](uniform-balls-in-bins-allocation.md)
2. [Multinomial distribution](multinomial-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Concentration of the empty-box fraction](concentration-of-the-empty-box-fraction.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/probability/7/b/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/probability/7/b/iv/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/probability/7/b/v/solution.md)
