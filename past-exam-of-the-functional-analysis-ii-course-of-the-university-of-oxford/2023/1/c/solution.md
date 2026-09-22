<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each real $a$, define the [sublevel set](../../../../sublevel-set.md) $K_a=\{u\in K:F(u)\leq a\}$. Continuity of $F$ and closure of $K$ make $K_a$ a [closed set](../../../../closed-set.md) in $X$; the [convex function](../../../../convex-function.md) inequality makes it a [convex set](../../../../convex-set-split.md). The preceding result therefore makes every $K_a$ a [sequentially weakly closed set](../../../../sequentially-weakly-closed-set.md). Equivalently, $F$ has [weak lower semicontinuity](../../../../weak-lower-semicontinuity.md) along sequences in $K$.

Every $K_a$ is bounded. This is immediate if $K$ is bounded. Otherwise, an unbounded $K_a$ would contain $u_n$ with $\|u_n\|\geq n$, contradicting the assumed [coercive function](../../../../coercive-function.md) condition $F(u_n)\to\infty$.

Choose $z\in K$ and put $\ell=\inf_KF\in[-\infty,F(z)]$. Choose a [minimizing sequence](../../../../minimizing-sequence.md) $(u_n)$ entirely in $K_{F(z)}$, with $F(u_n)\to\ell$; when $\ell=-\infty$, require $F(u_n)\leq-n$ for sufficiently large $n$. It is bounded by the previous paragraph.

The [weak subsequence of a bounded Hilbert-space sequence](../../../../weak-subsequence-of-a-bounded-hilbert-space-sequence.md) theorem gives $u_{n_j}\rightharpoonup u_0$. This applies even if $X$ is not separable: the closed [linear span](../../../../linear-span.md) of the sequence is a [separable Hilbert space](../../../../separable-hilbert-space.md); successive extraction makes every coefficient in a countable [Hilbertian basis](../../../../hilbertian-basis.md) converge, the common [norm](../../../../norm.md) bound gives square-summable limiting coefficients by the [Bessel inequality](../../../../bessel-s-inequality.md), and approximation by finite [linear combinations](../../../../linear-combination.md) proves [weak convergence](../../../../weak-convergence.md). [Orthogonal decomposition](../../../../orthogonal-decomposition-by-a-closed-subspace.md) extends that conclusion to all test vectors in $X$. Since $K$ is a [sequentially weakly closed set](../../../../sequentially-weakly-closed-set.md), $u_0\in K$.

For any real $a>\ell$, a tail of $(u_{n_j})$ lies in $K_a$, so $u_0\in K_a$. If $\ell=-\infty$, this would give $F(u_0)\leq a$ for every real $a$, impossible because $F$ is real-valued. Thus $\ell$ is finite; letting $a\downarrow\ell$ gives $F(u_0)\leq\ell$, while the definition of [infimum](../../../../infimum.md) gives the reverse inequality. Therefore

$$
\boxed{u_0\in K,\qquad F(u_0)=\min_{u\in K}F(u).}
$$

This proves [minimum of a coercive convex functional on a Hilbert space](../../../../minimum-of-a-coercive-convex-functional-on-a-hilbert-space.md) by the [direct method in the calculus of variations](../../../../direct-method-in-the-calculus-of-variations.md), with bounded [sublevel sets](../../../../sublevel-set.md) supplying the required [weak sequential compactness in a Hilbert space](../../../../weak-sequential-compactness-in-a-hilbert-space.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the functional analysis II course of the University of Oxford](../../../split.md)
5. [Functional analysis II course of the University of Oxford](../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
