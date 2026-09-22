<h1 id="24h/solution">Solution</h1>

↑ **Parent:** [24H](../24h.md)

For a [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) $D=\sum_pa_pp$ over an algebraically closed field, its [degree](../../../../../degree-of-a-divisor.md) is

$$
\deg D=\sum_pa_p.
$$

For a nonzero [rational function](../../../../../rational-function.md) $f$, its [principal divisor](../../../../../principal-divisor-on-an-algebraic-curve.md) is

$$
(f)=\operatorname{div}(f)=\sum_p\operatorname{ord}_p(f)p,
$$

where zeros have positive order and poles have negative order.

Now let $D=\sum_i a_ip_i$ have degree zero on the [projective line](../../../../../projective-line.md). Choose a homogeneous linear form $L_i(X_0,X_1)$ whose zero is $p_i$. Since $\sum_i a_i=0$, the expression

$$
f=\prod_iL_i^{a_i}
$$

is homogeneous of degree zero and therefore defines a rational function on $\mathbb P^1$. Each $L_i$ has one simple zero, and the cancellation of total degree removes any common scaling ambiguity, so

$$
(f)=\sum_i a_ip_i=D.
$$

Thus every degree-zero divisor on $\mathbb P^1$ is principal. If $E$ and $E'$ have the same degree, then $E-E'$ is principal, whence

$$
\boxed{E\sim E'}.
$$

This is the [divisor class on the projective line](../../../../../divisor-class-on-the-projective-line.md).

Write $p_\infty=[1:0]$. The coordinate $t=X_0/X_1$ has no critical zero or pole in the finite chart. Near infinity use $s=X_1/X_0=t^{-1}$; then

$$
dt=-s^{-2}ds.
$$

Hence the rational differential has one double pole at infinity and no other zero or pole:

$$
\boxed{(dt)=-2p_\infty},
$$

which represents the [canonical divisor of the projective line](../../../../../canonical-divisor-of-the-projective-line.md).

If $D\sim mK_{\mathbb P^1}$, then $D\sim-2mp_\infty$, and [linear equivalence of divisors](../../../../../linear-equivalence-of-divisors.md) gives $L(D)\cong L(-2mp_\infty)$. A function in the latter space has no finite poles, so it is a polynomial, and its degree is at most $-2m$. Therefore

$$
\boxed{\ell(D)=\max\{1-2m,0\}}.
$$

This calculation uses only the rational functions on $\mathbb P^1$, rather than the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md).

Finally, suppose distinct $p,q\in C$ satisfy $p-q=(f)$. The function $f$ has one simple pole and therefore defines a degree-one [finite morphism](../../../../../finite-morphism.md) $f:C\to\mathbb P^1$. A degree-one finite morphism between smooth projective curves is an [isomorphism](../../../../../isomorphism-of-algebraic-varieties.md). It would follow that $C\cong\mathbb P^1$ and hence that $C$ has [genus](../../../../../geometric-genus.md) zero, contrary to the hypothesis. Thus the [principal divisor with one simple zero and one simple pole](../../../../../principal-divisor-with-one-simple-zero-and-one-simple-pole.md) cannot occur on $C$:

$$
\boxed{p-q\text{ is not principal}.}
$$

## ↑ Ancestors (10)

1. [24H](../24h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
