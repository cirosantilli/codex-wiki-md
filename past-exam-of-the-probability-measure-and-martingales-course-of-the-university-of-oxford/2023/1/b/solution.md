<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $m\geq1$, fix signs $x_1,\ldots,x_m$. The constraints $X_j=x_j$ leave exactly two choices for the $(m+1)$ signs $Y_0,\ldots,Y_m$: choose $Y_0$ freely, then set $Y_1=Y_0x_1$ and $Y_j=x_{j-1}x_j$ for $2\leq j\leq m$. Each input tuple has [probability](../../../../probability.md) $2^{-(m+1)}$ by [independence](../../../../independent-random-variables.md). Consequently

$$
\mathbb P(X_1=x_1,\ldots,X_m=x_m)=2^{-m}
=\prod_{j=1}^m\mathbb P(X_j=x_j).
$$

Every finite subfamily is a [marginal distribution](../../../../marginal-distribution.md) of one such initial segment, so **the entire sequence is independent**, with fair sign [probability distributions](../../../../probability-distribution-split.md).

Using the usual everywhere sign-valued representatives, for every $n\geq1$ we have

$$
Y_0=X_n\prod_{j=1}^nY_j.
$$

The right side is [measurable](../../../../measurability.md) with respect to $\sigma(\mathcal Y,\mathcal T_n)$. Therefore $Y_0$ is [measurable](../../../../measurability.md) with respect to their [intersection](../../../../set-intersection.md) $\mathcal G$.

Write $\mathcal T=\bigcap_n\mathcal T_n$. The [Kolmogorov zero-one law](../../../../kolmogorov-s-zero-one-law.md) applies to the [independent random variables](../../../../independent-random-variables.md) $(X_n)$, so every [event](../../../../event.md) $C\in\mathcal T$ has [probability](../../../../probability.md) zero or one. Also $Y_0$ is [independent](../../../../independent-random-variables.md) of $\mathcal Y$: this follows first for finite [intersections](../../../../set-intersection.md) of sign [events](../../../../event.md) from the given [independence](../../../../independent-random-variables.md), then for their generated [sigma-algebra](../../../../sigma-algebra.md) by part (a).

The [sets](../../../../set-split.md) $D\cap C$ with $D\in\mathcal Y$ and $C\in\mathcal T$ form a [pi-system](../../../../pi-system.md) generating $\mathcal H$. If $\mathbb P(C)=0$, the [event](../../../../event.md) $D\cap C$ has [probability](../../../../probability.md) zero and is [independent](../../../../independent-random-variables.md) of every [event](../../../../event.md) in $\sigma(Y_0)$. If $\mathbb P(C)=1$, it differs from $D$ by a [null set](../../../../null-set.md), so the same [independence](../../../../independent-random-variables.md) follows from that of $Y_0$ and $\mathcal Y$. Another application of part (a) proves

$$
\boxed{Y_0\text{ is }\mathcal G\text{-measurable,}\qquad\sigma(Y_0)\text{ and }\mathcal H\text{ are independent}.}
$$

In particular $\mathcal H$ cannot contain the nontrivial [event](../../../../event.md) $\{Y_0=1\}$, whereas $\mathcal G$ does. Thus adjoining a [sigma-algebra](../../../../sigma-algebra.md) need not commute with a decreasing [intersection](../../../../set-intersection.md).

There is a small version qualification if the assumptions specify only the [probability distributions](../../../../probability-distribution-split.md), allowing exceptional values other than signs. Put $q_n=X_n/(Y_1\cdots Y_n)$ when the denominator is nonzero, and $q_n=0$ otherwise. For $k\geq n$, $q_k$ is [measurable](../../../../measurability.md) with respect to $\sigma(\mathcal Y,\mathcal T_n)$. The [limit superior](../../../../limit-superior.md) of $(q_k)$, after [scalar clipping](../../../../scalar-clipping.md) to $[-1,1]$, is therefore $\mathcal G$-[measurable](../../../../measurability.md) and equals $Y_0$ [almost surely](../../../../almost-sure-convergence.md). Literal [measurability](../../../../measurability.md) of an arbitrary version of $Y_0$ need not follow without choosing sign-valued representatives or adjoining the ambient [null sets](../../../../null-set.md). All the [independence](../../../../independent-random-variables.md) conclusions are unaffected.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../split.md)
5. [Probability, measure and martingales course of the University of Oxford](../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
