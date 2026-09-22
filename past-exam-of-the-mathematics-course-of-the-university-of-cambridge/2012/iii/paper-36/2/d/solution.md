<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a [pathwise differentiable statistical functional](../../../../../../pathwise-differentiability-of-a-statistical-functional.md), an [influence-function representer](../../../../../../influence-function-representer.md) is a [mean-zero function](../../../../../../mean-zero-function.md) $\varphi\in L^2(P)$ such that every admissible [score function](../../../../../../informant-function.md) $g$ satisfies $D\psi_P(g)=P(\varphi g)$. The [efficient influence function](../../../../../../canonical-gradient.md), also called the [canonical gradient](../../../../../../canonical-gradient.md), is the unique such representer in the [statistical tangent space](../../../../../../statistical-tangent-space.md). Equivalently, it is the [orthogonal projection](../../../../../../orthogonal-projection.md) of any representer onto that [statistical tangent space](../../../../../../statistical-tangent-space.md). The [Pythagorean theorem in an inner-product space](../../../../../../pythagorean-theorem-in-an-inner-product-space.md) shows that it has the smallest squared [L2 norm](../../../../../../l2-norm.md) among all representers.

Here the [statistical tangent space](../../../../../../statistical-tangent-space.md) is all of $L^2_0(P_f)$. To verify the closure explicitly, take $h\in L^2_0(P_f)$, truncate it to $h_m=\max(-m,\min(h,m))$, and set $g_m=h_m-P_fh_m$. Then $g_m$ is bounded and centered, and $g_m\to h$ in $L^2(P_f)$, by [dominated convergence](../../../../../../dominated-convergence-theorem.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Part (c) supplies a representer already in this space. Hence

$$
\boxed{\varphi_f(u)=a(u)-\int_0^1 a(v)f(v)\,dv.}
$$

Its [variance](../../../../../../variance-split.md) is $P_fa^2-(P_fa)^2$.

**The closure must be taken in the density-weighted space $L^2(P_f)$.** An unweighted reading of $L^2[0,1]$ in the printed hint is false. For example, when $f(u)=2u$, the [function](../../../../../../function-split.md) $h(u)=u^{-3/4}-8/5$ has $P_fh=0$ and $P_fh^2=36/25$, so bounded centered truncations converge to it in $L^2(P_f)$; nevertheless $h\notin L^2([0,1],du)$. This illustrates [density of bounded centered scores](../../../../../../density-of-bounded-centered-scores.md) and fixes the measure in the closure statement.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
