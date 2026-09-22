# Nested interval theorem

↑ **Parent:** [Nested intervals](nested-intervals.md)

If $I_1\supseteq I_2\supseteq\cdots$ are nonempty [closed intervals](closed-real-interval.md) with finite endpoints, then at least one [real number](real-number.md) belongs to every member. If their lengths tend to zero, exactly one [real number](real-number.md) belongs to every member. The result turns an unlimited sequence of consistent enclosures into an existence guarantee.

Write $I_n=[a_n,b_n]$. Nesting makes the left endpoints [nondecreasing](nondecreasing-function.md) and the right endpoints [nonincreasing](nonincreasing-function.md). Their bounds give finite [supremum](supremum.md) and [infimum](infimum.md), with

$$
\bigcap_{n=1}^{\infty}I_n=
\left[\sup_{n\geq1}a_n,\ \inf_{n\geq1}b_n\right].
$$

Indeed, every $b_n$ is an [upper bound](upper-bound-in-a-partially-ordered-set.md) for all the $a_j$, so the [least-upper-bound property](least-upper-bound-property.md) gives $\sup_j a_j\leq b_n$ for every $n$. This proves the displayed interval is nonempty. If $b_n-a_n\to0$, its two endpoints must coincide. This is the connection to the [completeness of the real numbers](completeness-of-the-real-numbers.md) discussed in [Günther Hörmann and David Langer, Einführung in die Analysis, §§3.15–3.16: nested intervals and order completeness](https://homepage.univie.ac.at/christian.schmeiser/einfanalysis.pdf).

<a id="image-nested-enclosures-can-converge-to-one-point-retain-a-whole-interval-or-have-no-common-point-when-endpoints-are-excluded"></a>
![](nested-intervals-intersection-cases.png)

**[Figure 11](#image-nested-enclosures-can-converge-to-one-point-retain-a-whole-interval-or-have-no-common-point-when-endpoints-are-excluded). Nested enclosures can converge to one point, retain a whole interval, or have no common point when endpoints are excluded**.

The distinction between existence and uniqueness is useful in computation. If an unknown point $x_*$ lies in every $[a_n,b_n]$, the [midpoint](midpoint.md) $m_n=(a_n+b_n)/2$ satisfies

$$
|m_n-x_*|\leq\frac{b_n-a_n}{2}.
$$

Thus the enclosure itself certifies an [absolute error](absolute-error.md) without knowing the answer. The [bisection error bound](bisection-error-bound.md) is the special case where each update halves the width.

Closedness and a finite initial enclosure matter. The [open intervals](open-interval.md) $(0,1/n)$ have no common point, while the closed but unbounded intervals $[n,\infty)$ also have empty intersection. A picture of a few intervals cannot certify the intersection of an infinite family; the hypotheses of the [nested interval theorem](nested-interval-theorem.md) do that work.

## ↑ Ancestors (8)

1. [Nested intervals](nested-intervals.md)
2. [Interval (mathematics)](interval-mathematics.md)
3. [Real line](real-line.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Bisection error bound](bisection-error-bound.md)
- [Closed real interval](closed-real-interval.md)
- [Nested-bracket proof of the intermediate value theorem](nested-bracket-proof-of-the-intermediate-value-theorem.md)
- [Nested interval theorem](nested-interval-theorem.md)
- [Nested intervals](nested-intervals.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-1/4f/solution.md)
