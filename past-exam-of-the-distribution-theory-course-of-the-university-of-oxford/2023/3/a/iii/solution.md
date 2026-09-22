<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Define two [open sets](../../../../../open-set.md) by

$$
Z(u)=\bigcup\{U\subseteq\Omega:U\text{ open},\ u|_U=0\},\qquad
G(u)=\bigcup\{U\subseteq\Omega:U\text{ open},\ u|_U\in C^\infty(U)\}.
$$

The [support of a distribution](../../../../../support-of-a-distribution.md) and its [singular support](../../../../../singular-support.md) are

$$
\boxed{\operatorname{supp}u=\Omega\setminus Z(u),\qquad
\operatorname{sing\,supp}u=\Omega\setminus G(u).}
$$

Both are relatively closed because the removed sets are open. The [locality of distributions](../../../../../locality-of-distributions.md) gives $u|_{Z(u)}=0$. On an overlap of two open smoothness regions, the two [smooth functions](../../../../../smooth-function.md) represent the same [distribution](../../../../../distribution-mathematical-analysis.md), so their difference is zero [almost everywhere](../../../../../almost-everywhere.md) and hence everywhere by [continuity](../../../../../continuous-function.md). They therefore join to one [smooth function](../../../../../smooth-function.md) on $G(u)$. The same [partition of unity](../../../../../partition-of-unity.md) argument shows that it represents $u$ there.

For $u=\mathbf1_\omega$, openness of $\omega$ implies

$$
\boxed{\operatorname{supp}\mathbf1_\omega=\overline\omega^{\,\Omega}.}
$$

Indeed every neighborhood of a point in this relative closure meets $\omega$ in an [open set](../../../../../open-set.md) containing a nonnegative [test function](../../../../../test-function.md) with positive integral; outside the closure the [indicator function](../../../../../indicator-function.md) is identically zero near the point.

The [singular support of an indicator function](../../../../../singular-support-of-an-indicator-function.md) needs a measure-sensitive boundary. For a [Lebesgue measurable set](../../../../../lebesgue-measurable-set.md) $A\subseteq\Omega$, define its [essential closure](../../../../../essential-closure.md) by

$$
\operatorname{esscl}_\Omega A
=\{x\in\Omega:|A\cap B_r(x)|>0\text{ whenever }r>0\text{ and }B_r(x)\subseteq\Omega\}.
$$

Then the general answer is

$$
\boxed{\operatorname{sing\,supp}\mathbf1_\omega
=\overline\omega^{\,\Omega}\cap\operatorname{esscl}_\Omega(\Omega\setminus\omega).}
$$

Outside this intersection, some ball has either no points of $\omega$ or a complement of [Lebesgue measure](../../../../../lebesgue-measure.md) zero. The [regular distribution](../../../../../regular-distribution.md) is respectively the constant zero or one on that ball and is smooth. Conversely, at a point of the intersection, every sufficiently small ball has positive [Lebesgue measure](../../../../../lebesgue-measure.md) in both sets. If a [smooth function](../../../../../smooth-function.md) represented the [indicator function](../../../../../indicator-function.md) there, its values would be in $\{0,1\}$ everywhere: any other value, by [continuity](../../../../../continuous-function.md), would give a ball of positive [Lebesgue measure](../../../../../lebesgue-measure.md) on which equality [almost everywhere](../../../../../almost-everywhere.md) fails. On a connected ball such a continuous two-valued [function](../../../../../function-split.md) is constant, contradicting the two positive measures.

In particular, the answer need not be the full topological [boundary](../../../../../boundary-of-a-set.md). For $\Omega=\mathbb R^n$ and $\omega=\mathbb R^n\setminus\{0\}$, the [indicator function](../../../../../indicator-function.md) is the constant one [almost everywhere](../../../../../almost-everywhere.md), so its [singular support](../../../../../singular-support.md) is empty although the [boundary](../../../../../boundary-of-a-set.md) is $\{0\}$. The full relative [boundary](../../../../../boundary-of-a-set.md) is the answer when every neighborhood of each boundary point contains a positive [Lebesgue measure](../../../../../lebesgue-measure.md) portion of the complement, as for an [open set](../../../../../open-set.md) with smooth boundary.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
