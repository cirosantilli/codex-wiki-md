<h1 id="7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [integer norm lower bound for rational approximation to a quadratic irrational](../../../../../../integer-norm-lower-bound-for-rational-approximation-to-a-quadratic-irrational.md). The [integer](../../../../../../integer.md) $2q^2-a^2$ is nonzero, since $\sqrt2$ is irrational. If $a/q<2$, then

$$
\left|\sqrt2-\frac aq\right|
=\frac{|2q^2-a^2|}{q^2(\sqrt2+a/q)}
>\frac1{4q^2},
$$

because $\sqrt2+a/q<\sqrt2+2<4$. If $a/q\geq2$, the difference is at least $2-\sqrt2>1/4\geq1/(4q^2)$. Thus

$$
\boxed{\left|\sqrt2-\frac aq\right|>\frac1{4q^2}\quad(a,q\geq1).}
$$

In particular, $\sqrt2$ is a [badly approximable number](../../../../../../badly-approximable-number.md).

To estimate the prime-weighted [exponential sum](../../../../../../exponential-sum.md), let $Q=\lfloor N^{1/2}\rfloor$. The [Dirichlet approximation theorem](../../../../../../dirichlet-s-approximation-theorem.md) gives a reduced fraction $a/q$ with

$$
1\leq q\leq Q,\qquad
\left|\sqrt2-\frac aq\right|\leq\frac1{qQ}\leq\frac1{q^2}.
$$

Combining this with the lower bound gives $q>Q/4$. Thus $q\asymp N^{1/2}$; the approximation cannot have a small denominator.

The relevant analytic input is the [prime exponential-sum estimate from Vaughan identity](../../../../../../prime-exponential-sum-estimate-from-vaughan-identity.md):

$$
\sum_{n\leq N}\Lambda(n)e(\alpha n)
\ll\left(\frac N{\sqrt q}+N^{4/5}+\sqrt{Nq}\right)\log^4(2N)
\quad\left(\left|\alpha-\frac aq\right|\leq q^{-2},\ (a,q)=1\right).
$$

Here is the structure behind that estimate. With [Dirichlet convolution](../../../../../../dirichlet-convolution.md) and cutoffs $U,V$, the [Vaughan identity](../../../../../../vaughan-s-identity.md) is

$$
\Lambda=\mu_{\leq U}*\log
-\mu_{\leq U}*\Lambda_{\leq V}*1
+\Lambda_{\leq V}
+\mu_{>U}*\Lambda_{>V}*1.
$$

It follows from $\Lambda=\mu*\log$, $\log=\Lambda*1$, and $\mu*1=\delta_1$. The first two [Dirichlet convolution](../../../../../../dirichlet-convolution.md) terms become [type I sums](../../../../../../type-i-sum.md) with one short factor; the last becomes a bilinear [type II sum](../../../../../../type-ii-sum.md) with both factors bounded below. Split these sums into dyadic blocks and use $U=V=N^{2/5}$. For the [type I sums](../../../../../../type-i-sum.md), the inner [finite geometric series](../../../../../../finite-geometric-series.md) has bound $\min(L,(2\|\alpha m\|)^{-1})$. For the [type II sums](../../../../../../type-ii-sum.md), the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) followed by expansion introduces analogous sums in differences of indices. Rational approximation separates the phases into blocks of length comparable to $q$, bounding these reciprocal-distance sums. The [Dirichlet convolution](../../../../../../dirichlet-convolution.md) coefficients are divisor-bounded, producing the logarithmic factors. These steps give the displayed estimate; no unproved cancellation of arbitrary weighted sums is being assumed.

With $\alpha=\sqrt2$ and $q\asymp N^{1/2}$, the two denominator-dependent terms are $O(N^{3/4})$. Consequently

$$
\boxed{\sum_{n\leq N}\Lambda(n)e(n\sqrt2)
=O(N^{4/5}\log^4(2N))=O(N^{9/10}).}
$$

The final passage absorbs the logarithm using the positive exponent margin $9/10-4/5=1/10$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
