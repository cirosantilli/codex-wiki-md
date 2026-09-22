<h1 id="23f/solution">Solution</h1>

↑ **Parent:** [23F](../23f.md)

A [divisor on a complex manifold](../../../../../divisor-on-a-complex-manifold.md), specialized to a compact [Riemann surface](../../../../../riemann-surfaces.md), is a finite sum $D=\sum_p n_pp$ with integer coefficients, and $\deg D=\sum_pn_p$. Two divisors are linearly equivalent when $D'=D+(h)$ for a nonzero [meromorphic function](../../../../../meromorphic-function.md) $h$, whose [principal divisor on a complex manifold](../../../../../principal-divisor-on-a-complex-manifold.md) records zero orders minus pole orders. Define

$$
L(D)=\{0\}\cup\{f\text{ meromorphic}:(f)+D\ge0\},\qquad \ell(D)=\dim_{\mathbb C}L(D).
$$

Multiplication by $1/h$ gives an isomorphism $L(D)\to L(D')$, because $(f/h)+D'=(f)+D$. Its inverse is multiplication by $h$, proving $\ell(D')=\ell(D)$.

On the [Riemann sphere](../../../../../riemann-sphere.md) move $P$ to infinity by a Möbius coordinate. Meromorphic functions on the sphere are rational; those with no finite poles and a pole of order at most one at infinity are exactly $az+b$. Thus **$\ell(P)=2$**, without using Riemann–Roch.

The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) for a compact connected genus-$g$ surface is $\ell(D)-\ell(K-D)=\deg D+1-g$, where $K$ is a canonical divisor. Choose $D=(g+1)P$. Since the second dimension is nonnegative, $\ell(D)\ge2$. Constants span only one dimension, so a nonconstant $f$ exists whose only possible pole is at $P$ with order at most $g+1$. The degree of its holomorphic map to the sphere is the total pole order. Therefore

$$
\boxed{\deg(f:C\to S^2)\le g+1}.
$$

## ↑ Ancestors (10)

1. [23F](../23f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
