# Domain with a nonzero idempotent maximal ideal

↑ **Parent:** [Idempotent ideal](idempotent-ideal.md)

Let

$$
R=\bigcup_{n\geq0}\mathbb Q[u_n],\qquad u_n=t^{1/2^n},\qquad u_n=u_{n+1}^2.
$$

This [ring](ring.md) consists of finite sums of rational multiples of nonnegative [dyadic rational](dyadic-rational.md) powers of $t$, interpreted as [functions](function-split.md) on $t>0$. Every pair of elements lies in one [polynomial ring](polynomial-ring.md) $\mathbb Q[u_n]$, so $R$ is an [integral domain](integral-domain.md). The constant term defines a [surjective](surjective-function.md) [ring homomorphism](ring-homomorphism.md) $R\to\mathbb Q$. Its [kernel of a ring homomorphism](kernel-of-a-ring-homomorphism.md) $\mathfrak m$ is nonzero and is a [maximal ideal](maximal-ideal.md), by the [maximal ideal quotient criterion](maximal-ideal-quotient-criterion.md).

Every $f\in\mathfrak m$ has the form $u_ng(u_n)$ for some $n$ and some [polynomial](polynomial-split.md) $g$. The identity

$$
f=u_{n+1}\bigl(u_{n+1}g(u_{n+1}^2)\bigr)
$$

expresses it as a product of two elements of $\mathfrak m$. Therefore $\mathfrak m=\mathfrak m^2$, and $\mathfrak m^n=\mathfrak m$ for all $n\geq1$. This shows that strict descent of [powers of an ideal](powers-of-an-ideal.md) can fail in an [integral domain](integral-domain.md), even for a nonzero [maximal ideal](maximal-ideal.md). By the [determinant trick](determinant-trick.md), such an [ideal](ideal.md) cannot be finitely generated, so this [ring](ring.md) is not a [Noetherian ring](noetherian-ring.md).

## ↑ Ancestors (9)

1. [Idempotent ideal](idempotent-ideal.md)
2. [Product of ideals](product-of-ideals.md)
3. [Ideal](ideal.md)
4. [Ring](ring.md)
5. [Commutative algebra](commutative-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-commutative-algebra-course-of-the-university-of-oxford/2017/2/d/solution.md)
