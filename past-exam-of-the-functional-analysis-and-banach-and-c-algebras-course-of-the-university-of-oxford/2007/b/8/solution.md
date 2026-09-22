<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

A [state on a C-star algebra](../../../../state-on-a-c-star-algebra.md) is a [positive linear functional](../../../../positive-linear-functional.md) of [norm](../../../../norm.md) one. A [cyclic representation of a C-star algebra](../../../../cyclic-representation-of-a-c-star-algebra.md) is a representation of a [C-star algebra](../../../../c-star-algebra.md) $\pi:A\to B(H)$ with a vector $\xi$ whose orbit $\pi(A)\xi$ has dense linear span in $H$. On $c$, pointwise multiplication and coordinatewise [complex conjugation](../../../../complex-conjugation.md) preserve convergence; the constant sequence one is the unit. The [supremum norm](../../../../supremum-norm.md) is submultiplicative and obeys $\|\alpha^*\alpha\|_\infty=\|\alpha\|_\infty^2$. Completeness is given, so **$c$ is a commutative unital [C-star algebra](../../../../c-star-algebra.md)**.

If $F=\phi(\beta)$ is a state, testing its positivity on the coordinate projections gives $\beta_{j+1}\geq0$. To recover the independent coefficient at infinity, let $q_N$ have its first $N$ coordinates zero and all later ones one. This is a positive element of $c$, and $F(q_N)=\beta_1+\sum_{j>N}\beta_{j+1}\geq0$. Passing to the limit gives $\beta_1\geq0$. By the given isometry, $\|F\|=\|\beta\|_1=\sum_j\beta_j$, which is one. Conversely these nonnegative unit-sum coefficients make $F(\alpha^*\alpha)$ a sum of nonnegative weighted squares, and the isometry gives [norm](../../../../norm.md) one. Thus **the stated coefficient conditions are necessary and sufficient**.

For the specified state, all other coefficients are zero because they are nonnegative and the first three already sum to one. Its GNS null ideal is

$$
N_x=\{\alpha:x(\alpha^*\alpha)=0\}=\{\alpha:\alpha_\infty=\alpha_1=\alpha_2=0\}.
$$

Evaluation at infinity and the first two coordinates identifies $c/N_x$ with $\mathbb C^3$, with [inner product](../../../../inner-product-split.md) $\tfrac12u_\infty\overline{v_\infty}+\tfrac14u_1\overline{v_1}+\tfrac14u_2\overline{v_2}$. Left multiplication induces the diagonal representation; the class of the unit is $(1,1,1)$. In the equivalent standard [inner product](../../../../inner-product-split.md) the resulting GNS triple is

$$
\boxed{H_x=\mathbb C^3,\quad\pi_x(\alpha)=\operatorname{diag}(\alpha_\infty,\alpha_1,\alpha_2),\quad\xi_x=(1/\sqrt2,1/2,1/2).}
$$

Its coefficient is exactly $\tfrac12\alpha_\infty+\tfrac14\alpha_1+\tfrac14\alpha_2=F(\alpha)$. The three evaluations can be assigned arbitrary independent values by a convergent sequence, and all three entries of $\xi_x$ are nonzero. Therefore its orbit spans $\mathbb C^3$, verifying **cyclicity and the required state identity** directly.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
