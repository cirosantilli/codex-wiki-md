<h1 id="2/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First take integers $1\leq k<n$. For independent copies $X_1,\ldots,X_n$ of $X$, define

$$
A=k^{-1/\alpha}\sum_{j=1}^kX_j,\qquad B=(n-k)^{-1/\alpha}\sum_{j=k+1}^nX_j.
$$

The two blocks involve disjoint families of [independent random variables](../../../../../independent-random-variables.md), so $A$ and $B$ are independent. The assumed [strictly stable distribution](../../../../../strictly-stable-distribution.md) gives $A\overset d=X$, $B\overset d=X$, and

$$
(k/n)^{1/\alpha}A+(1-k/n)^{1/\alpha}B=n^{-1/\alpha}\sum_{j=1}^nX_j\overset d=X.
$$

Therefore, on any fixed [probability space](../../../../../probability-space-split.md) carrying $X$ and an independent copy $X'$, their [joint probability distribution](../../../../../joint-probability-distribution.md) gives

$$
(k/n)^{1/\alpha}X+(1-k/n)^{1/\alpha}X'\overset d=X.
$$

Now fix an arbitrary $0<c<1$ and choose rationals $r_m=k_m/n_m\in(0,1)$ tending to $c^\alpha$. Continuity of the real powers gives, on that fixed [probability space](../../../../../probability-space-split.md),

$$
r_m^{1/\alpha}X+(1-r_m)^{1/\alpha}X'\longrightarrow cX+(1-c^\alpha)^{1/\alpha}X'\quad\text{almost surely}.
$$

The left sides all have the [probability distribution](../../../../../probability-distribution-split.md) of $X$. Since [almost sure convergence](../../../../../almost-sure-convergence.md) implies [convergence in distribution](../../../../../convergence-in-distribution.md), their limit has that same [probability distribution](../../../../../probability-distribution-split.md). Hence

$$
\boxed{R_c=(1-c^\alpha)^{1/\alpha}X',\qquad R_c\text{ independent of }X,\qquad cX+R_c\overset d=X.}
$$

This proves [strict stability implies self-decomposability](../../../../../strict-stability-implies-self-decomposability.md). The limit argument uses no [moment-generating function](../../../../../moment-generating-function.md) or finite [moments](../../../../../moment.md), which is essential for general [stable distributions](../../../../../stable-distribution.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
