<h1 id="23h/solution">Solution</h1>

↑ **Parent:** [23H](../23h.md)

A [divisor](../../../../../divisor.md) on a compact connected [Riemann surface](../../../../../riemann-surfaces.md) is a finite formal sum $D=\sum_pn_pp$ with integer coefficients; its degree is $\sum_pn_p$. A [canonical divisor](../../../../../canonical-divisor.md) is the divisor of zeros and poles of a nonzero meromorphic differential. Two divisors are linearly equivalent when their difference is the divisor of a nonzero [meromorphic function](../../../../../meromorphic-function.md). Such [principal divisors](../../../../../principal-divisor-on-an-algebraic-curve.md) have degree zero, but equal degree does not generally imply [linear equivalence of divisors](../../../../../linear-equivalence-of-divisors.md).

For example take distinct points $p,q$ on a genus-one surface. If $p-q$ were principal, its function would define a degree-one meromorphic map to the sphere, since it has just one [simple pole](../../../../../simple-pole.md). A degree-one map between compact [Riemann surfaces](../../../../../riemann-surfaces.md) is a biholomorphism, contradicting their different genera. Thus these degree-one divisors are not equivalent.

Define $L(D)=\{f\text{ meromorphic}: (f)+D\ge0\}\cup\{0\}$ and $\ell(D)=\dim_{\mathbb C}L(D)$. The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) states

$$
\ell(D)-\ell(K-D)=\deg D+1-g.
$$

Since all holomorphic functions on the compact surface are constant, $\ell(0)=1$. Setting $D=0$ gives $\ell(K)=g$. Multiplication by a fixed meromorphic differential identifies $L(K)$ with holomorphic differentials, so their dimension is $g$. Setting $D=K$ then gives

$$
\boxed{\dim H^0(S,\Omega^1)=g,\qquad\deg K=2g-2.}
$$

For $g=2$, choose a nonzero holomorphic differential, whose effective [canonical divisor](../../../../../canonical-divisor.md) has degree two. Since $\ell(K)=2$, $L(K)$ contains a nonconstant [meromorphic function](../../../../../meromorphic-function.md). Its pole divisor is bounded by that effective $K$, proving **existence of a nonconstant function with total pole multiplicity at most two**.

## ↑ Ancestors (10)

1. [23H](../23h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
