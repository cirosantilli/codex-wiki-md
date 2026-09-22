<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Apply the [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md) to the [finite-field Kakeya set](../../../../../finite-field-kakeya-set.md) $A$. We will actually obtain the stronger estimate

$$
\boxed{|A|\geq\binom{p+n-1}{n}\geq\frac{p^n}{n!}.}
$$

Let $\mathcal P$ be the [vector space](../../../../../vector-space-split.md) over the [prime field](../../../../../prime-field.md) $\mathbb F_p$ of [multivariate polynomials](../../../../../multivariate-polynomial.md) in $n$ variables of [total degree of a polynomial](../../../../../total-degree-of-a-polynomial.md) at most $p-1$. By the [dimension of a bounded-total-degree polynomial space](../../../../../dimension-of-a-bounded-total-degree-polynomial-space.md), its [monomial](../../../../../monomial.md) basis consists of $x_1^{a_1}\cdots x_n^{a_n}$ with $a_i\geq0$ and $\sum_i a_i\leq p-1$. Adding a slack exponent gives $n+1$ nonnegative exponents summing to $p-1$; the [stars and bars](../../../../../stars-and-bars-combinatorics.md) count shows that

$$
\dim\mathcal P=\binom{p+n-1}{n}.
$$

If $|A|<\dim\mathcal P$, the evaluation [linear map](../../../../../linear-map.md) $\mathcal P\to\mathbb F_p^A$ has a nonzero element in its [kernel of a linear map](../../../../../kernel-of-a-linear-map.md). Thus there is a nonzero [polynomial](../../../../../polynomial-split.md) $P$ of [total degree of a polynomial](../../../../../total-degree-of-a-polynomial.md) $d\leq p-1$ vanishing at every point of $A$. Its degree cannot be zero, since $A$ contains a line and is nonempty. Write $P_d$ for its nonzero top [homogeneous polynomial](../../../../../homogeneous-polynomial.md) part.

For every nonzero $v\in\mathbb F_p^n$, the directional hypothesis supplies an [affine line in a vector space](../../../../../affine-line-in-a-vector-space.md)

$$
\{a_v+tv:t\in\mathbb F_p\}\subseteq A.
$$

Directions are one-dimensional [vector subspaces](../../../../../vector-subspace.md); rescaling a representative does not change this line. The univariate [polynomial](../../../../../polynomial-split.md) $P(a_v+tv)$ has degree at most $d<p$ and vanishes for all $p$ values of $t$. The [root bound for a polynomial](../../../../../lagrange-root-bound-over-a-field.md) makes it the zero [polynomial](../../../../../polynomial-split.md). Its coefficient of $t^d$ is exactly $P_d(v)$, so $P_d(v)=0$ for every nonzero $v$. Because $d>0$, $P_d(0)=0$ too.

To finish, we prove the relevant [polynomial nonvanishing below the field size](../../../../../polynomial-nonvanishing-below-the-field-size.md). A [polynomial](../../../../../polynomial-split.md) over $\mathbb F_p$ of degree at most $p-1$ in each variable cannot vanish on all of $\mathbb F_p^n$ unless it is zero. Induct on $n$. The one-variable case is the [root bound for a polynomial](../../../../../lagrange-root-bound-over-a-field.md). For more variables, write

$$
Q(x_1,\ldots,x_n)=\sum_{j=0}^{p-1}Q_j(x_1,\ldots,x_{n-1})x_n^j.
$$

Fixing the first $n-1$ coordinates gives a univariate [polynomial](../../../../../polynomial-split.md) with $p$ [roots of a polynomial](../../../../../root-of-a-polynomial.md), so all its coefficients are zero. Hence every $Q_j$ vanishes on $\mathbb F_p^{n-1}$, and the induction hypothesis makes every $Q_j$ zero. Applying this to $P_d$, whose [total degree of a polynomial](../../../../../total-degree-of-a-polynomial.md) is less than $p$, contradicts its choice as nonzero.

Therefore $|A|\geq\dim\mathcal P$. Finally,

$$
\binom{p+n-1}{n}=\frac{p(p+1)\cdots(p+n-1)}{n!}\geq\frac{p^n}{n!},
$$

which proves the requested lower bound. The crucial observation in the [finite-field Kakeya polynomial bound](../../../../../finite-field-kakeya-polynomial-bound.md) is that complete lines force the highest [homogeneous polynomial](../../../../../homogeneous-polynomial.md) part to vanish in every direction.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
