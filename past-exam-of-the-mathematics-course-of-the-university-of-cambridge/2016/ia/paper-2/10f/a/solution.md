<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For any fixed bin, each ball supplies an independent [Bernoulli distribution](../../../../../../bernoulli-distribution.md) indicator with success probability $1/m$. Summing the $n$ [indicator variables](../../../../../../indicator-variable.md) gives

$$
\boxed{B_i\sim\operatorname{Bin}(n,1/m).}
$$

The full occupancy vector has a [multinomial distribution](../../../../../../multinomial-distribution.md), the basic [uniform balls-in-bins allocation](../../../../../../uniform-balls-in-bins-allocation.md). Distinct bin counts are **not independent** when $n\geq1$ and $m\geq2$. To see this, write $B_i=\sum_{r=1}^n I_{r,i}$. For the same ball, $I_{r,i}I_{r,j}=0$ if $i\ne j$, while indicators from distinct balls are independent. Their [covariance](../../../../../../covariance.md) is therefore

$$
\boxed{\operatorname{Cov}(B_i,B_j)=-\frac{n}{m^2}<0\quad(i\ne j).}
$$

With no balls the counts are deterministic; with one bin there are no distinct bin pairs. These degenerate cases do not contradict the conclusion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
