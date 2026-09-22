<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We first prove the stronger compact-square form, in which all the one-variable functions are continuous. There are five fixed pairs of [continuous functions](../../../../../continuous-function.md) $a_q,b_q$ on the unit interval such that every real $f\in C([0,1]^2)$ has a representation

$$
\boxed{f(x,y)=\sum_{q=1}^5G_q\big(a_q(x)+b_q(y)\big),}
$$

with continuous one-variable $G_q$. We construct the inner functions and then prove convergence of the outer functions, rather than assume the [Kolmogorov-Arnold representation theorem](../../../../../kolmogorov-arnold-representation-theorem.md).

**Constructing separating inner functions.** Work in the [Banach space](../../../../../banach-space-split.md) $\mathcal X=C([0,1])^{10}$ with the maximum of the ten [supremum norms](../../../../../supremum-norm.md). For each positive integer $n$, let $U_n$ consist of tuples $(a_q,b_q)_{q=1}^5$ for which there are, for each $q$, finite families of closed intervals $I_{qi}$ and $J_{qj}$ of length less than $1/n$, satisfying two conditions. Each point of the unit interval belongs to at least four of the five unions $\bigcup_iI_{qi}$, and likewise for the $J$ families. Within each fixed $q$, the compact sets

$$
K_{qij}=a_q(I_{qi})+b_q(J_{qj})
$$

are pairwise disjoint for distinct pairs $(i,j)$. Each $K_{qij}$ is a closed interval, by [continuity](../../../../../continuous-function.md) and the [intermediate value theorem](../../../../../intermediate-value-theorem.md). These are [grid-separated additive coordinates](../../../../../grid-separated-additive-coordinates.md).

The set $U_n$ is open: for a tuple and its finitely many witnessing intervals, the distinct compact image intervals have a positive minimum separation. A sufficiently small uniform change in the inner functions preserves that separation, while the interval-cover conditions do not change.

To prove density, start with any ten [continuous functions](../../../../../continuous-function.md) and any positive approximation tolerance. Choose a common fine partition so that each original function oscillates by less than a small fraction of the tolerance on a partition cell and its immediate neighbours; choose its mesh smaller than $1/(2n)$. Near every internal division point put five small, pairwise disjoint open gaps, one for each $q$. Use these gaps to divide the interval into closed towns for family $q$, including the two endpoints in towns. Gaps from different families are disjoint, so any point misses at most one family; every town has length less than $1/n$ if the gaps are sufficiently small. Do this for both coordinates.

Approximate $a_q$ and $b_q$ by functions which are constant on their respective towns, and interpolate linearly across the gaps. The towns lie near single partition cells, so [uniform continuity](../../../../../uniform-continuity.md) makes these approximations as close to the original functions as desired. For each $q$, perturb the finitely many town values $\alpha_{qi},\beta_{qj}$ arbitrarily slightly so that all sums $\alpha_{qi}+\beta_{qj}$ are distinct. This is possible because each unwanted equality between distinct pairs is a proper [affine hyperplane](../../../../../affine-hyperplane.md) in the [finite-dimensional vector space](../../../../../finite-dimensional-vector-space.md) of values; finitely many such hyperplanes cannot fill any [open ball](../../../../../open-ball.md). Interpolating the perturbed values still approximates the original functions, and the rectangle images are now distinct singleton sets. Thus $U_n$ is dense.

By the [Baire category theorem](../../../../../baire-category-theorem.md), choose one tuple in $\bigcap_{n\geq1}U_n$. To recall why completeness suffices here, start inside any [open ball](../../../../../open-ball.md) and successively choose [closed balls](../../../../../closed-ball.md) of positive radii tending to zero, each contained in the preceding ball and in the next dense open $U_n$. Their centers form a [Cauchy sequence](../../../../../cauchy-sequence.md), and its limit belongs to every ball, hence every $U_n$. Fix this tuple once and for all: it does not depend on $f$.

**A quantitative approximation step.** Let a continuous residual $r$ have [supremum norm](../../../../../supremum-norm.md) $M>0$. Choose $n$ large enough that the oscillation of $r$ on any rectangle of side lengths below $1/n$ is at most $M/20$. For each rectangle $I_{qi}\times J_{qj}$ choose a sample point $(x_{qi},y_{qj})$. Define a one-variable $h_q$ to have constant value $r(x_{qi},y_{qj})/3$ on $K_{qij}$. The image intervals are disjoint, so interpolate linearly in their gaps and extend constantly beyond the outermost ones. Then $h_q$ is continuous on the real line and

$$
\|h_q\|_\infty\leq M/3.
$$

At a given $(x,y)$, at most one family fails to contain $x$ in an $I$ town and at most one fails to contain $y$ in a $J$ town. Thus the point belongs to rectangles in $k$ families, where $3\leq k\leq5$. For each of these families the summand differs from $r(x,y)/3$ by at most $M/60$. Each remaining summand has absolute value at most $M/3$. Consequently

$$
\begin{aligned}
\left|r(x,y)-\sum_{q=1}^5h_q(a_q(x)+b_q(y))\right|
&\leq\left(\frac{k-3}{3}+\frac{5-k}{3}\right)M+\frac{kM}{60}\\
&\leq\frac23M+\frac1{12}M=\frac34M.
\end{aligned}
$$

This proves a strict contraction uniformly over the square, including points in gaps.

**Summing the corrections.** Set $r_0=f$ and apply that step repeatedly, subtracting the five summands at each stage. The residuals satisfy $\|r_m\|_\infty\leq(3/4)^m\|f\|_\infty$, and the corresponding corrections satisfy $\|h_{qm}\|_\infty\leq(3/4)^m\|f\|_\infty/3$. If a residual is zero, take all subsequent corrections to be zero. The series

$$
G_q=\sum_{m=0}^{\infty}h_{qm}
$$

converges uniformly on the real line to a [continuous function](../../../../../continuous-function.md). The residuals tend uniformly to zero, proving the boxed representation. An affine change of each coordinate treats any compact rectangle.

**Removing a restriction to a compact domain.** For a continuous real function $f$ on the whole plane, set

$$
M(t)=\max_{x^2+y^2\leq t}|f(x,y)|\quad(t\geq0).
$$

Choose a positive continuous one-variable $A$ by linear interpolation of $A(n)=(n+2)(1+M(n+1))$ at nonnegative integers. Since these values increase, for $n\leq t\leq n+1$ we have $A(t)\geq(n+2)(1+M(n+1))\geq(1+t)(1+M(t))$. Therefore

$$
b(x,y)=\frac{f(x,y)}{A(x^2+y^2)}
\quad\text{satisfies}\quad |b(x,y)|\leq\frac1{1+x^2+y^2}.
$$

Let $\sigma(x)=\tfrac12+\pi^{-1}\arctan x$. Transport $b$ to the open square by $\widetilde b(s,t)=b(\tan(\pi(s-1/2)),\tan(\pi(t-1/2)))$, and set it to zero on the square's boundary. The displayed decay estimate proves [continuity](../../../../../continuous-function.md) at every boundary point, including the corners. Apply the compact-square representation to $\widetilde b$ and substitute $s=\sigma(x)$, $t=\sigma(y)$ to obtain $b$ using continuous one-variable functions and [addition](../../../../../addition.md).

Finally multiply this expression by $A(x^2+y^2)$. Multiplication itself uses only [addition](../../../../../addition.md) and one-variable functions, because

$$
uv=\frac{(u+v)^2-(u-v)^2}{4}.
$$

Squaring, negation and scaling are one-variable operations, as are $A$ and $\sigma$. Thus the [whole-plane reduction for continuous superposition](../../../../../whole-plane-reduction-for-continuous-superposition.md) gives a finite expression of the required kind for every continuous $f$ on the plane, without a boundedness assumption. For a complex-valued $f$, apply the argument to its real and imaginary parts and combine them using [addition](../../../../../addition.md) and the one-variable map $z\mapsto iz$. **All the constituent one-variable functions can be taken continuous.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
