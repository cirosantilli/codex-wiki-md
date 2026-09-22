<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

The set $K\cap P$ is compact because $K$ is closed and bounded, and the product

$$
G(x)=\prod_{j=1}^n x_j
$$

is continuous. By the [extreme value theorem](../../../../../extreme-value-theorem.md), $G$ has a maximizer. Since $K$ meets the interior of the [nonnegative orthant](../../../../../nonnegative-orthant.md) $P$, some feasible product is positive, so every maximizer lies in $\operatorname{Int}P$.

On $\operatorname{Int}P$, maximizing $G$ is equivalent to maximizing

$$
F(x)=\log G(x)=\sum_{j=1}^n\log x_j.
$$

The Hessian of $F$ is

$$
D^2F(x)=\operatorname{diag}\left(-\frac1{x_1^2},\ldots,-\frac1{x_n^2}\right),
$$

which is negative definite. Thus $F$ is a [strictly concave function](../../../../../strictly-concave-function.md), and it has at most one maximizer on the [convex set](../../../../../convex-set.md) $K\cap P$. Denote this unique point by $x^*$.

For any $x\in K\cap P$, the line segment

$$
x(t)=(1-t)x^*+tx,\qquad 0\leq t<1,
$$

lies in $K\cap\operatorname{Int}P$. Since $F(x(t))$ is maximal at $t=0$, its right derivative there is nonpositive:

$$
0\geq\left.\frac d{dt}F(x(t))\right|_{t=0}
=\sum_{j=1}^n\frac{x_j-x_j^*}{x_j^*}.
$$

Therefore

$$
\boxed{\sum_{j=1}^n\frac{x_j}{x_j^*}\leq n}.
$$

This is the supporting inequality for the [product maximizer on a compact convex subset of the positive orthant](../../../../../product-maximizer-on-a-compact-convex-subset-of-the-positive-orthant.md).

Suppose now that $K$ is invariant under cyclic coordinate permutation. That permutation preserves the product, so uniqueness forces it to fix $x^*$. Hence

$$
x^*=(r,\ldots,r)
$$

for some $r>0$. More explicitly,

$$
\boxed{
r=\max_{x\in K\cap P}\frac1n\sum_{j=1}^n x_j
}.
$$

Indeed, [cyclic symmetry averaging](../../../../../cyclic-symmetry-averaging.md) puts the diagonal point with coordinate equal to the mean of any $x\in K$ back in $K$, while the preceding inequality with $x_j^*=r$ gives $\sum_jx_j\leq nr$.

Finally, given $a=(a_1,\ldots,a_n)\in\operatorname{Int}P$, define

$$
K=\left\{x\in P:
\sum_{j=1}^n\frac{x_j}{a_j}\leq n
\right\}.
$$

This set is nonempty, closed, convex and bounded, and it contains $a$. By the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md),

$$
\frac{\prod_jx_j}{\prod_ja_j}
=\prod_{j=1}^n\frac{x_j}{a_j}
\leq
\left(\frac1n\sum_{j=1}^n\frac{x_j}{a_j}\right)^n
\leq1.
$$

Equality holds only when all $x_j/a_j$ are equal and their sum is $n$, namely only at $x=a$. Thus this $K$ has

$$
\boxed{x^*=a}.
$$

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
