# Dual norm

↑ **Parent:** [Norm](norm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_norm)

A [dual norm](dual-norm.md) measures how strongly a [bounded linear functional](continuous-linear-functional.md) can respond to a unit-sized input. If $p$ is a [bounded linear functional](continuous-linear-functional.md) on a [normed vector space](normed-vector-space-split.md) $X$, write $\langle p,x\rangle=p(x)$ and define

$$
\|p\|_* =\sup_{\|x\|\le1}|p(x)|.
$$

It is the [operator norm](operator-norm.md) of $p$ when its scalar output is measured by [absolute value](absolute-value.md). On $\mathbb R^n$, represent $p(x)=a^Tx$ using a coefficient [vector](vector.md) $a$. The [unit ball](unit-ball.md) is symmetric, so maximizing $|a^Tx|$ gives the same value as maximizing $a^Tx$: negate an input whenever its output is negative.[§A.1.6, printed p. 636: dual norm and scalar operator-norm interpretation](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

For an original two-coordinate example, fix $a=(2,-1)^T$, so $p(x)=2x_1-x_2$. The input [norm](norm.md) changes the allowable [unit ball](unit-ball.md) and hence the [dual norm](dual-norm.md):

$$
\begin{aligned}
\|x\|_1\le1&:\quad\|p\|_*=2,
&&x_*=(1,0)^T,\\
\|x\|_2\le1&:\quad\|p\|_*=\sqrt5,
&&x_*=(2,-1)^T/\sqrt5,\\
\|x\|_\infty\le1&:\quad\|p\|_*=3,
&&x_*=(1,-1)^T.
\end{aligned}
$$

Under the [L1 norm](l1-norm.md), $|2x_1-x_2|\le2(|x_1|+|x_2|)\le2$, and $(1,0)^T$ attains the bound. Under the [Euclidean norm](euclidean-norm.md), the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $|a^Tx|\le\|a\|_2\|x\|_2\le\sqrt5$, with equality at the displayed normalized [vector](vector.md). Under the [maximum norm](supremum-norm.md), each coordinate can reach unit [absolute value](absolute-value.md), so $|2x_1-x_2|\le2+1=3$; $(1,-1)^T$ attains it. Thus the [dual norms](dual-norm.md) of these three [vector norms](norm.md) are respectively the [maximum norm](supremum-norm.md), the [Euclidean norm](euclidean-norm.md), and the [L1 norm](l1-norm.md). For $1\le p\le\infty$, [Lp norms](lp-norm.md) on a finite coordinate space pair with their [Holder conjugate exponents](conjugate-exponents.md).[§A.1.6, printed p. 637: Euclidean self-duality and one-, infinity- and p-norm duality; the numerical vector and maximizing points here are independent examples](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

<a id="image-the-same-linear-functional-has-three-dual-norms-on-three-input-unit-balls"></a>
![](dual-norm-unit-balls-supporting-lines.png)

**[Figure 2](#image-the-same-linear-functional-has-three-dual-norms-on-three-input-unit-balls). The same linear functional has three dual norms on three input unit balls**. Original geometry for $p(x)=2x_1-x_2$. The orange [supporting line](supporting-line.md) $2x_1-x_2=\|p\|_*$ touches each [unit ball](unit-ball.md) at the marked maximizing point. Blue regions use the [L1 norm](l1-norm.md), [Euclidean norm](euclidean-norm.md) and [maximum norm](supremum-norm.md), respectively.

This geometry explains the usefulness of a [dual norm](dual-norm.md): it translates a bound on inputs into the sharp bound on a linear output. The [support function](support-function.md) of the [unit ball](unit-ball.md) gives its value in the coefficient direction $a$. Changing the input budget changes the set of possible inputs; the three different answers do not conflict. In finite dimensions a closed [unit ball](unit-ball.md) is [compact](compact-space.md), so a [continuous linear functional](continuous-linear-functional.md) achieves its maximum [absolute value](absolute-value.md). In an infinite-dimensional [normed vector space](normed-vector-space-split.md), the [supremum](supremum.md) remains the definition and need not be achieved.

**Table of contents**

- [Dual norm as a worst-case linear error bound](dual-norm-as-a-worst-case-linear-error-bound.md)
- [Dual norm supremum need not be attained](dual-norm-supremum-need-not-be-attained.md)

## ↑ Ancestors (7)

1. [Norm](norm.md)
2. [Normed vector space](normed-vector-space-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Block mixed norm](block-mixed-norm.md)
- [Coercive bilinear form](coercive-bilinear-form.md)
- [Dual norm](dual-norm.md)
- [Dual norm as a worst-case linear error bound](dual-norm-as-a-worst-case-linear-error-bound.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/8c/solution.md)
