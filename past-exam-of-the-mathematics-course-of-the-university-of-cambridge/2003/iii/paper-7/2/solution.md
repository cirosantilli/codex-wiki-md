<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [finite-field Kakeya set](../../../../../finite-field-kakeya-set.md), also called a finite-field Besicovitch set, is a subset containing a complete [affine line in a vector space](../../../../../affine-line-in-a-vector-space.md) $a+\mathbb F_pv$ in every nonzero direction $v$, with scalar multiples counted as the same direction. The line's translate may depend on the direction.

For odd $p$, take the union of the lines $y=mx-m^2/4$, $m\in\mathbb F_p$. Completing the square gives $x^2-y=(m/2-x)^2$. Thus that union is exactly $K_0=\{(x,y):x^2-y\text{ is a square, including zero}\}$. For each fixed $x$ there are $(p+1)/2$ such $y$, so $|K_0|=p(p+1)/2$. It contains every nonvertical slope. Add the vertical line $x=0$, whose overlap with $K_0$ has $(p+1)/2$ points. The [tangent-line finite-field Kakeya construction](../../../../../tangent-line-finite-field-kakeya-construction.md) consequently has

$$
\boxed{|K|=\frac{p^2+2p-1}{2}=\frac12p^2(1+o(1)).}
$$

The prime two is irrelevant to this asymptotic statement and can be handled by taking its whole plane.

For the high-dimensional lower bound, we give a direct [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md) proof, which yields a stronger estimate. Suppose a finite-field Kakeya set $K\subseteq\mathbb F_p^n$ has fewer than $\binom{p+n-1}{n}$ points. That binomial coefficient is the [dimension of a bounded-total-degree polynomial space](../../../../../dimension-of-a-bounded-total-degree-polynomial-space.md) of [polynomials](../../../../../polynomial-split.md) of total degree at most $p-1$. Evaluation at the points of $K$ imposes fewer linear conditions than this dimension. By the [rank-nullity theorem](../../../../../rank-nullity-theorem.md), there is a nonzero [polynomial](../../../../../polynomial-split.md) $P$ of total degree $d\leq p-1$ vanishing on $K$.

For every nonzero $v$ choose the line $a_v+tv\subseteq K$. The [polynomial](../../../../../polynomial-split.md) $P(a_v+tv)$ in $t$ has degree at most $d<p$ and vanishes at all $p$ field elements, so it vanishes identically. Its coefficient of $t^d$ is the leading [homogeneous polynomial](../../../../../homogeneous-polynomial.md) part $P_d(v)$. Thus $P_d(v)=0$ for every nonzero $v$. The case $d=0$ is already impossible for a nonzero constant vanishing on a nonempty set; for $d>0$, the absence of a constant term in this [homogeneous polynomial](../../../../../homogeneous-polynomial.md) also gives $P_d(0)=0$.

A [polynomial](../../../../../polynomial-split.md) of degree less than $p$ in each variable cannot vanish at every point of $\mathbb F_p^n$ unless it is zero. To see this, induct on $n$: fix the first $n-1$ variables, apply the one-variable root bound in the last variable, then apply the induction hypothesis to each resulting coefficient [polynomial](../../../../../polynomial-split.md). This forces $P_d=0$, contradicting the choice of the leading part. We have proved the [finite-field Kakeya polynomial bound](../../../../../finite-field-kakeya-polynomial-bound.md)

$$
|K|\geq\binom{p+n-1}{n}\geq\frac{p^n}{n!}.
$$

At $n=15$ this implies the required bound with an explicit absolute constant:

$$
\boxed{|K|\geq\frac{p^{15}}{15!}\geq\frac{p^9}{15!},\qquad c=1/15!.}
$$

The argument is valid in every prime characteristic and does not invoke the lower bound as an unproved theorem.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
