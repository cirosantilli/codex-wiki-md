<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Put $T=R\circ J_Z:Z\to X^*$. Then $(Tz)(x)=x(z)$ and $\|Tz\|\leq\|z\|$. We must prove $T$ onto.

Take $f\in B_{X^*}$. Part (iv) supplies $\theta\in B_{Z^{**}}$ with $R\theta=f$. [Goldstine's theorem](../../../../goldstine-theorem.md) gives a net $z_\alpha\in B_Z$ with $J_Zz_\alpha\to\theta$ weak-star. By [continuity](../../../../continuous-function.md) of $R$, $Tz_\alpha\to f$ in $\sigma(X^*,X)$. Reflexivity of $X$ makes this the [weak topology](../../../../weak-topology-split.md) on $X^*$ by part (iii). Thus $B_{X^*}$ is contained in the weak [closure](../../../../closure-topology.md) of $T(B_Z)$.

The reverse containment holds because $T(B_Z)\subseteq B_{X^*}$, and the latter ball is weakly closed: it is the intersection of the closed evaluation constraints $|g(x)|\leq1$ for $x\in B_X$. The set $T(B_Z)$ is convex, so part (ii), now on the [Banach space](../../../../banach-space-split.md) $X^*$, gives

$$
\boxed{\overline{T(B_Z)}^{\|\cdot\|}=B_{X^*}.}
$$

Density of the ball gives exact surjectivity by a convergent correction argument. For nonzero $f\in X^*$, choose $z_1$ with $\|z_1\|\leq\|f\|$ and $\|f-Tz_1\|\leq\|f\|/2$. Inductively approximate the current residual $r_{n-1}$ by $Tz_n$ with $\|z_n\|\leq\|r_{n-1}\|$ and $\|r_{n-1}-Tz_n\|\leq\|r_{n-1}\|/2$. If a residual is zero, stop.

The residual [norms](../../../../norm.md) are bounded by $2^{-n}\|f\|$, while $\sum_n\|z_n\|\leq2\|f\|$. Completeness of $Z$ gives $z=\sum_nz_n\in Z$, and [continuity](../../../../continuous-function.md) of $T$ gives $Tz=f$. For $f=0$ use $z=0$. Therefore

$$
\boxed{\forall f\in X^*\ \exists z\in Z:\quad x(z)=f(x)\text{ for every }x\in X.}
$$

This is [evaluation onto the dual of a reflexive dual subspace](../../../../evaluation-onto-the-dual-of-a-reflexive-dual-subspace.md). The correction argument is needed: a dense image alone would not imply surjectivity.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the functional analysis course of the University of Oxford](../../../split.md)
5. [Functional analysis course of the University of Oxford](../../../../functional-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
