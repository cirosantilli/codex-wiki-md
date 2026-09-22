<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We prove existence by the [direct method in the calculus of variations](../../../../direct-method-in-the-calculus-of-variations.md), making the step with [weakly compact sets](../../../../weakly-compact-set.md) explicit. For $X=W_0^{1,4}(\Omega)$ and $f\in L^{8/7}(\Omega)$, introduce the [functional](../../../../functional.md)

$$
E(u)=\frac14\|\nabla u\|_4^4+\frac18\|u\|_8^8-\int_\Omega fu\,dx.
$$

It is finite by part (b)(i). [Hölder's inequality](../../../../holder-s-inequality.md) and the [Sobolev embedding theorem](../../../../sobolev-embedding-theorem.md) give

$$
E(u)\geq\frac14\|u\|_X^4-C_8\|f\|_{8/7}\|u\|_X\longrightarrow+\infty
\quad\text{as }\|u\|_X\to\infty.
$$

Thus $E$ is a [coercive function](../../../../coercive-function.md), bounded below, and every [minimizing sequence](../../../../minimizing-sequence.md) is bounded in $X$.

The space $X$ is a [reflexive Banach space](../../../../reflexive-banach-space.md): it is isomorphic to a closed [linear subspace](../../../../vector-subspace.md) of the finite product of the [reflexive spaces](../../../../reflexive-space.md) $L^4(\Omega)$ recording the [function](../../../../function-split.md) and its [weak derivatives](../../../../weak-derivative.md). A bounded [sequence](../../../../sequence.md) in a [reflexive Banach space](../../../../reflexive-banach-space.md) has a [weakly convergent](../../../../weak-convergence.md) [subsequence](../../../../subsequence.md). Hence, after passing to a [subsequence](../../../../subsequence.md), a [minimizing sequence](../../../../minimizing-sequence.md) satisfies $u_j\rightharpoonup u_*$ in $X$. The continuous [linear maps](../../../../linear-map.md) $u\mapsto\nabla u$ into $L^4$ and $u\mapsto u$ into $L^8$ preserve [weak convergence](../../../../weak-convergence.md), so

$$
\nabla u_j\rightharpoonup\nabla u_*\text{ in }L^4,
\qquad u_j\rightharpoonup u_*\text{ in }L^8.
$$

The [norm](../../../../norm.md) in any [Banach space](../../../../banach-space-split.md) has [weak lower semicontinuity](../../../../weak-lower-semicontinuity.md), since it is the supremum of absolute values of bounded [linear functionals](../../../../linear-functional.md) of [dual norm](../../../../dual-norm.md) at most one, by the [Hahn-Banach theorem](../../../../hahn-banach-theorem.md). Therefore the two nonnegative [norm](../../../../norm.md) powers in $E$ have [weak lower semicontinuity](../../../../weak-lower-semicontinuity.md). Also $u\mapsto\int_\Omega fu\,dx$ belongs to $X^*$ and is continuous for [weak convergence](../../../../weak-convergence.md). It follows that

$$
E(u_*)\leq\liminf_j E(u_j)=\inf_{u\in X}E(u).
$$

For any $v\in X$, the real [function](../../../../function-split.md) $t\mapsto E(u_*+tv)$ has a minimum at $t=0$. Its [derivative](../../../../derivative.md) there is

$$
0=\left.\frac{d}{dt}E(u_*+tv)\right|_{t=0}
=\int_\Omega|\nabla u_*|^2\nabla u_*\cdot\nabla v\,dx
+\int_\Omega u_*^7v\,dx-\int_\Omega fv\,dx.
$$

This differentiation is justified directly by finite polynomial expansions: the fourth power of the [Euclidean norm](../../../../euclidean-norm.md) of $\nabla u_*+t\nabla v$ and the eighth power of $u_*+tv$ have integrable coefficients by [Hölder's inequality](../../../../holder-s-inequality.md). Thus $A(u_*)=0$, giving existence of a [weak solution](../../../../weak-solution.md).

If $u,w$ are two [weak solutions](../../../../weak-solution.md), testing the difference by $u-w$ and using part (b)(iii) gives

$$
0=\langle A(u)-A(w),u-w\rangle\geq\tfrac14\|u-w\|_X^4.
$$

Hence

$$
\boxed{\text{For every }f\in L^{8/7}(\Omega),\text{ there exists exactly one weak solution }u_*\in W_0^{1,4}(\Omega).}
$$

No sign assumption on $f$ or on the [weak solution](../../../../weak-solution.md) is required.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
