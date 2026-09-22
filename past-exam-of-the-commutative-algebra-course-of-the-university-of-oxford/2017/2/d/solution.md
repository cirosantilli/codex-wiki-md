<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**No.** A [domain with a nonzero idempotent maximal ideal](../../../../domain-with-a-nonzero-idempotent-maximal-ideal.md) is a counterexample. Consider

$$
R=\bigcup_{n\geq0}\mathbb Q[t^{1/2^n}],\qquad
u_n=t^{1/2^n},\qquad u_n=u_{n+1}^2.
$$

This can be realized concretely as a [ring of functions](../../../../ring-of-functions.md) on $t>0$: its elements are finite sums of rational multiples of nonnegative [dyadic rational](../../../../dyadic-rational.md) powers of $t$. Each stage $\mathbb Q[u_n]$ is a [polynomial ring](../../../../polynomial-ring.md), because a nonzero [polynomial](../../../../polynomial-split.md) cannot vanish for all $u_n>0$. Any two elements lie in one stage, which is an [integral domain](../../../../integral-domain.md), so their product is nonzero if both are nonzero. Thus $R$ is an [integral domain](../../../../integral-domain.md).

The constant term defines a [surjective](../../../../surjective-function.md) [ring homomorphism](../../../../ring-homomorphism.md) $\epsilon:R\to\mathbb Q$. It is well defined because replacing $u_n$ by $u_{n+1}^2$ preserves the constant term. Its [kernel of a ring homomorphism](../../../../kernel-of-a-ring-homomorphism.md)

$$
\mathfrak m=\{f\in R:\text{the constant term of }f\text{ is }0\}
$$

is a [maximal ideal](../../../../maximal-ideal.md), since $R/\mathfrak m\cong\mathbb Q$ is a [field](../../../../field.md), by the [maximal ideal quotient criterion](../../../../maximal-ideal-quotient-criterion.md). Also $u_0=t\in\mathfrak m$ is nonzero.

If $f\in\mathfrak m$, choose a stage in which $f=u_ng(u_n)$ for a [polynomial](../../../../polynomial-split.md) $g\in\mathbb Q[z]$. Then

$$
f=u_{n+1}\bigl(u_{n+1}g(u_{n+1}^2)\bigr).
$$

Both factors belong to $\mathfrak m$, so $f\in\mathfrak m^2$. The reverse inclusion holds for every [ideal](../../../../ideal.md), proving that $\mathfrak m$ is an [idempotent ideal](../../../../idempotent-ideal.md). Hence

$$
\boxed{0\ne\mathfrak m\text{ is maximal},\qquad\mathfrak m^n=\mathfrak m^{n+1}=\mathfrak m\quad(n\geq1).}
$$

The [Noetherian ring](../../../../noetherian-ring.md) hypothesis in [c](../c.md) is therefore essential even for a [maximal ideal](../../../../maximal-ideal.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
