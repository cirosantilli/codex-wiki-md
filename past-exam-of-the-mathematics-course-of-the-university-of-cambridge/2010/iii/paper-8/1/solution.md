<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We first prove a compact-square form of the [Kolmogorov-Arnold representation theorem](../../../../../kolmogorov-arnold-representation-theorem.md), including the construction needed for exact representation. We then remove the compactness restriction; a mere limiting sequence of two-variable approximations would not establish a finite expression using one-variable functions.

There are five pairs of [continuous functions](../../../../../continuous-function.md) $a_q,b_q:[0,1]\to\mathbb R$ with the following [grid-separated additive coordinates](../../../../../grid-separated-additive-coordinates.md) property. At every arbitrarily small mesh, choose for each $q$ a finite family of disjoint closed intervals in each coordinate. Their product rectangles cover every point of the square in at least three families, and the images of different rectangles in family $q$ under

$$
s_q(x,y)=a_q(x)+b_q(y)
$$

are mutually disjoint compact intervals.

Here is a proof of that existence assertion. Work in the [complete metric space](../../../../../complete-metric-space.md) $X=C([0,1])^{10}$ with its maximum uniform norm. For an integer $N\ge1$, let $U_N$ comprise tuples having the preceding property with every interval shorter than $1/N$. Each $U_N$ is open: fix a witnessing finite collection of rectangles. Their compact image intervals have positive mutual separation within each family, so sufficiently small uniform perturbations of the ten functions preserve separation, while the domain cover is unchanged.

To prove density, start with any ten [continuous functions](../../../../../continuous-function.md) and any desired approximation tolerance. Choose a common grid spacing $\delta<1/N$ so fine that all ten have small oscillation over distances $2\delta$, using [uniform continuity](../../../../../uniform-continuity.md). For the five families, use grid cuts shifted successively by $\delta/5$. Remove tiny open gaps about these cuts, of radius less than $\delta/20$. Gaps from different families are disjoint. The complementary components in $[0,1]$ are closed intervals shorter than $\delta$. Every coordinate belongs to an interval in at least four families, so a pair of coordinates belongs to product rectangles in at least three common families.

In each family, approximate $a_q$ and $b_q$ by constants on those intervals and interpolate linearly across the gaps. The constants can be chosen arbitrarily close to sampled original values, so the resulting functions approximate the originals uniformly. Perturb the finitely many constants slightly so that all sums $a_{q,I}+b_{q,J}$ for distinct pairs $(I,J)$ are different. This is possible because each forbidden equality is a proper [hyperplane](../../../../../hyperplane.md), and a finite union of such hyperplanes cannot contain an open ball of choices. The rectangle images are now distinct singleton sets. Thus $U_N$ is dense. The [Baire category theorem](../../../../../baire-category-theorem.md) gives a tuple in $\bigcap_{N\ge1}U_N$. Fix that tuple once and for all.

Let $r$ be a real [continuous function](../../../../../continuous-function.md) on the square and write $M=\|r\|_\infty$. If $M=0$ there is nothing to do. Otherwise choose a sufficiently fine witnessing cover that the oscillation of $r$ in every rectangle is at most $M/10$. For each family $q$, define a one-variable [continuous function](../../../../../continuous-function.md) $g_q$ to equal $r$ at a chosen sample point of each rectangle, divided by three, throughout that rectangle's image interval. The image intervals are disjoint, so interpolate linearly between them and extend constantly beyond the extreme intervals. Then

$$
\|g_q\|_\infty\le M/3.
$$

At a point $(x,y)$, let $k\in\{3,4,5\}$ be the number of families whose rectangles contain that point. In those $k$ families the corresponding summand differs from $r(x,y)/3$ by at most $M/30$. In the other families its absolute value is at most $M/3$. Therefore

$$
\begin{aligned}
\left|r(x,y)-\sum_{q=1}^5g_q(s_q(x,y))\right|
&\le \left(\left|1-\frac{k}{3}\right|+\frac{5-k}{3}\right)M+\frac{kM}{30}\\
&\le\frac23M+\frac16M=\frac56M.
\end{aligned}
$$

This is a genuine contraction of the approximation error with the inner functions fixed.

Starting with $r_0=F\in C([0,1]^2)$, repeat the construction and put $r_{j+1}=r_j-\sum_qg_{q,j}\circ s_q$. Then $\|r_j\|_\infty\le(5/6)^j\|F\|_\infty$ and $\|g_{q,j}\|_\infty\le(5/6)^j\|F\|_\infty/3$. The series

$$
G_q=\sum_{j=0}^\infty g_{q,j}
$$

converges uniformly on all of $\mathbb R$, so each $G_q$ is continuous by the [uniform limit theorem](../../../../../uniform-limit-theorem.md). Telescoping the residuals gives the exact compact representation

$$
\boxed{F(x,y)=\sum_{q=1}^5G_q\bigl(a_q(x)+b_q(y)\bigr)}.
$$

The infinite iteration has been absorbed into five one-variable functions; the resulting expression has only finitely many additions and [function compositions](../../../../../function-composition.md).

For the [whole-plane reduction for continuous superposition](../../../../../whole-plane-reduction-for-continuous-superposition.md), let the given function be $f\in C(\mathbb R^2)$. Set

$$
M(t)=\max\left(1,\sup_{x^2+y^2\le t}|f(x,y)|\right),\qquad t\ge0.
$$

This is finite on every bounded interval by compactness. Choose a positive [continuous function](../../../../../continuous-function.md) $A$ on $[0,\infty)$ by linearly interpolating the values $A(k)=(k+2)M(k+1)$ at nonnegative integers. For $k\le t\le k+1$, monotonicity of the endpoint values gives $A(t)\ge A(k)\ge(1+t)M(t)$. Extend $A$ constantly to negative arguments. Consequently

$$
b(x,y)=\frac{f(x,y)}{A(x^2+y^2)},\qquad
|b(x,y)|\le\frac1{1+x^2+y^2}.
$$

Let $\kappa(x)=\frac12+\pi^{-1}\arctan x$. Transport $b$ to $(0,1)^2$ with $\kappa^{-1}(s)=\tan(\pi(s-1/2))$. Extend the transported function by zero on the boundary of the square. The displayed bound proves continuity at every boundary point, including corners, because approaching the boundary forces at least one original coordinate to tend to infinity. Apply the compact representation to this extension to obtain

$$
B(x,y)=b(x,y)=\sum_{q=1}^5G_q\bigl(a_q(\kappa(x))+b_q(\kappa(y))\bigr).
$$

Also $A_0(x,y)=A(x^2+y^2)$ already uses only one-variable squaring, addition and [function composition](../../../../../function-composition.md). Finally multiplication can itself be eliminated by the identity

$$
\boxed{f(x,y)=\frac{(A_0(x,y)+B(x,y))^2-(A_0(x,y)-B(x,y))^2}{4}}.
$$

Negation, squaring and division by four are continuous one-variable functions. Hence the entire expression uses only the permitted one-variable continuous functions and addition, even for an unbounded $f$ on $\mathbb R^2$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
