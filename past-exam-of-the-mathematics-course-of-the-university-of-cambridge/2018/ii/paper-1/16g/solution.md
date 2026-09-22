<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

[Ordinal exponentiation](../../../../../ordinal-exponentiation.md) is defined by [transfinite recursion](../../../../../transfinite-recursion.md):

$$
\alpha^0=1,\qquad
\alpha^{\beta+1}=\alpha^\beta\alpha,\qquad
\alpha^\lambda=\sup_{\xi<\lambda}\alpha^\xi
$$

when $\lambda$ is a nonzero [limit ordinal](../../../../../limit-ordinal.md). If $\alpha\geq1$, each successor step and each supremum show that $\beta\mapsto\alpha^\beta$ is nondecreasing. If $\alpha\geq2$, [transfinite induction](../../../../../transfinite-induction.md) strengthens this to strict increase: $\alpha^\beta<\alpha^{\beta+1}$, and the value at a limit exceeds every earlier value.

Strict increase can disappear when the base changes. For example, with $\omega<\omega+1<\omega+2$,

$$
(\omega+1)^\omega=(\omega+2)^\omega=\omega^\omega,
$$

because for every positive finite $n$, both finite powers have leading term $\omega^n$, and taking the supremum gives $\omega^\omega$.

We next prove

$$
\boxed{\ \alpha^{\beta+\gamma}=\alpha^\beta\alpha^\gamma\ }.
$$

Apply [transfinite induction](../../../../../transfinite-induction.md) to $\gamma$. The zero and successor cases follow directly from the recursive definitions and the associativity of [ordinal multiplication](../../../../../ordinal-multiplication.md). At a limit $\lambda$, continuity of ordinal multiplication in its right argument gives

$$
\alpha^{\beta+\lambda}
=\sup_{\xi<\lambda}\alpha^{\beta+\xi}
=\sup_{\xi<\lambda}\alpha^\beta\alpha^\xi
=\alpha^\beta\alpha^\lambda.
$$

The superficially similar identity $(\alpha\beta)^\gamma=\alpha^\gamma\beta^\gamma$ is false: for $\alpha=\omega$, $\beta=2$, and $\gamma=2$,

$$
(\omega2)^2=\omega^2 2\ne\omega^2 4=\omega^2 2^2.
$$

Finally,

$$
\boxed{\ \alpha^{\omega_1}\geq\omega_1\iff\alpha\geq2\ },
\qquad
\boxed{\ \alpha^{\omega_1}\geq\omega_2\iff\alpha\geq\omega_2\ }.
$$

For the first equivalence, bases zero and one fail, while strict increase embeds every countable ordinal into the powers of any base $\alpha\geq2$. For the second, $\alpha\geq\omega_2$ immediately gives $\alpha^{\omega_1}\geq\alpha$. Conversely, if $\alpha<\omega_2$, then $|\alpha|\leq\aleph_1$. Every exponent below the [first uncountable ordinal](../../../../../first-uncountable-ordinal.md) $\omega_1$ is countable, so each $\alpha^\beta$ has cardinality at most $\aleph_1$; the supremum of $\aleph_1$ such ordinals still has cardinality at most $\aleph_1$ and is therefore below the [second uncountable ordinal](../../../../../second-uncountable-ordinal.md) $\omega_2$.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
