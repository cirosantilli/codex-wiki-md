<h1 id="o/o4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The totals are [independent](../../../../../../independent-random-variables.md) binomials, $n\sim\operatorname{Bin}(2N,q)$ and $m\sim\operatorname{Bin}(2M,p)$. Thus

$$
L(p,q)=\binom{2N}n\binom{2M}m q^n(1-q)^{2N-n}p^m(1-p)^{2M-m}.
$$

Differentiating the log [likelihood](../../../../../../likelihood-function.md), or maximizing the two factors separately, gives

$$
\boxed{\hat p=\frac m{2M},\qquad\hat q=\frac n{2N}.}
$$

This remains the constrained [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) at zero or one when a total is at an endpoint. At interior parameters the sample information, in coordinate order $(p,q)$, is

$$
\boxed{I(p,q)=\begin{pmatrix}2M/[p(1-p)]&0\\0&2N/[q(1-q)]\end{pmatrix}.}
$$

For example $-\mathbb E\ell_{pp}=\mathbb E[m/p^2+(2M-m)/(1-p)^2]=2M/[p(1-p)]$; the cross [derivative](../../../../../../derivative.md) is zero. As both sample sizes grow with nondegenerate interior probabilities, the joint approximation is normal with mean $(p,q)$ and [covariance](../../../../../../covariance.md) $\operatorname{diag}(p(1-p)/(2M),q(1-q)/(2N))$. The [independence](../../../../../../independent-random-variables.md) of the two estimators is exact, inherited from the two data samples.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [O4](../../../o4.md)
4. [O](../../../../o.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
