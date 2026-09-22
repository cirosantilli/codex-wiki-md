<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We first extend the scalar [Hadamard three-circle theorem](../../../../../../hadamard-three-circle-theorem.md) to a [holomorphic](../../../../../../complex-differentiability-at-a-point.md) Banach-space-valued function $F$. Apply its inequality to $\ell(F(z))$ for every [bounded linear functional](../../../../../../continuous-linear-functional.md) $\ell$ of [norm](../../../../../../norm.md) at most one, and use the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) to recover the [norm](../../../../../../norm.md). For the radii $1/R,1,R$ this gives

$$
\|F(1)\|^2\le\sup_{|z|=R}\|F(z)\|\;\sup_{|z|=1/R}\|F(z)\|.
$$

Now take $F(z)=p(z)^{2^n}$. Even for noncommuting coefficients this is an algebra-valued [holomorphic](../../../../../../complex-differentiability-at-a-point.md) [polynomial](../../../../../../polynomial-split.md). Taking the $2^{-n}$th power gives

$$
\|p(1)^{2^n}\|^{2/2^n}\le
\max_{|z|=R}\|p(z)^{2^n}\|^{1/2^n}
\max_{|z|=1/R}\|p(z)^{2^n}\|^{1/2^n}.
$$

On each [boundary](../../../../../../boundary-of-a-set.md) circle the [continuous](../../../../../../continuous-function.md) functions $f_n(z)=\|p(z)^{2^n}\|^{1/2^n}$ decrease, by submultiplicativity, to $r_A(p(z))$ by the [spectral radius formula](../../../../../../spectral-radius-formula.md). Their maxima decrease to the [supremum](../../../../../../supremum.md) of this [pointwise limit](../../../../../../pointwise-limit.md). To justify that passage without assuming [continuity](../../../../../../continuous-function.md) of the [spectral radius](../../../../../../spectral-radius.md), take maximizing points along a convergent subsequence on the [compact](../../../../../../compact-space.md) circle. For any fixed $k$, all later $f_n$ are bounded by $f_k$; [continuity](../../../../../../continuous-function.md) of $f_k$ therefore bounds the limiting maxima by $f_k$ at the limiting point. Taking the infimum over $k$ gives the desired upper bound, while the reverse bound is immediate.

Passing to the limit proves the [spectral-radius three-circle inequality](../../../../../../spectral-radius-three-circle-inequality.md) at the geometric mean:

$$
\boxed{r_A(p(1))^2\le
\sup_{|z|=R}r_A(p(z))\;\sup_{|z|=1/R}r_A(p(z)).}
$$

For a nonunital algebra, use its [unitization of an algebra](../../../../../../unitization-of-an-algebra.md); the [spectral radius](../../../../../../spectral-radius.md) of an original algebra element is unchanged. Zero [boundary](../../../../../../boundary-of-a-set.md) suprema cause no difficulty in the decreasing-limit argument.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
