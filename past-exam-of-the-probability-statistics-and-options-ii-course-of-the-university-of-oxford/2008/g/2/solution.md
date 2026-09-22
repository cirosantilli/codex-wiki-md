<h1 id="g/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Assume the regular Sturm–Liouville setting: real coefficients with $p>0$, $w>0$ and sufficient [continuity](../../../../continuous-function.md) and [differentiability](../../../../differentiability.md) for the integrations below. Apply a multiplier to $J[y]-\lambda(\int_a^bwy^2-1)$. Its [first variation](../../../../first-variation.md) in the direction $\eta$ is

$$
2[p y'\eta]_a^b-2\int_a^b\big((p y')'+qy+\lambda wy\big)\eta\,dx.
$$

Variations vanishing at both endpoints and the supplied fundamental lemma give

$$
\boxed{-(p y')'-qy=\lambda wy.}
$$

At a free endpoint the value of $\eta$ is arbitrary, so the natural condition is $p y'=0$ there. At a fixed endpoint $\eta=0$, so no such [derivative](../../../../derivative.md) condition is imposed; the prescribed endpoint value is imposed instead. This distinction also allows one endpoint of each type.

For [eigenfunctions](../../../../eigenfunction.md) $u,v$ of distinct [eigenvalues](../../../../eigenvalue.md) $\lambda,\mu$ under the same homogeneous self-adjoint endpoint conditions, multiply their equations by $v,u$ and subtract. Integration gives

$$
(\lambda-\mu)\int_a^b wuv\,dx=[p(uv'-u'v)]_a^b=0.
$$

The boundary expression vanishes for both natural conditions and homogeneous fixed-value conditions. Thus $\boxed{\int_a^b wuv=0}$ for different [eigenvalues](../../../../eigenvalue.md).

In the specified fixed-endpoint case the eigenproblem is $-y''-y=\lambda y$, $y(0)=y(1)=0$. There are no nonzero solutions when $\lambda+1\le0$; the elementary exponential or affine solutions and the two endpoint conditions prove this. For $\lambda+1>0$, the first condition [leaves](../../../../leaf-of-a-graph.md) a sine and the second requires frequency $n\pi$. The normalized stationary functions and [eigenvalues](../../../../eigenvalue.md) are

$$
\boxed{y_n(x)=\pm\sqrt2\sin(n\pi x),\qquad\lambda_n=n^2\pi^2-1,\quad n\ge1.}
$$

Distinct sine modes are [orthogonal](../../../../orthogonal-vectors.md) by the [product-to-sum formula](../../../../product-to-sum-formula.md), or by the preceding [Green second identity](../../../../green-second-identity.md). Although they need not satisfy the natural [derivative](../../../../derivative.md) conditions, their fixed zero values also annihilate the boundary expression, so [orthogonality](../../../../orthogonal-vectors.md) is expected.

The [Wirtinger inequality](../../../../wirtinger-inequality.md) $\int_0^1y'^2\ge\pi^2\int_0^1y^2$ gives $J[y]\ge\pi^2-1$. For completeness it follows by writing $y=v\sin\pi x$ for a smooth function supported away from the endpoints and integrating the cross term: $\int(y'^2-\pi^2y^2)=\int\sin^2(\pi x)v'^2\ge0$. Approximation extends it to the Dirichlet Sobolev class. Equality is attained by the first sine mode; the eigenproblem or equality condition gives only its scalar multiples. Hence the two normalized minimizers are $\boxed{y=\pm\sqrt2\sin\pi x}$ and the [minimum](../../../../minimum-of-a-subset-of-a-total-order.md) is $\boxed{\pi^2-1=\lambda_1}$.

There is a wording distinction in the source: the two sign choices of the [minimum](../../../../minimum-of-a-subset-of-a-total-order.md) are not [orthogonal](../../../../orthogonal-vectors.md) to each other, since their [inner product](../../../../inner-product-split.md) is $-1$. [Orthogonality](../../../../orthogonal-vectors.md) applies to the stationary modes with different [eigenvalues](../../../../eigenvalue.md), not to both signs of the same minimizer.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [G](../../g.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
