<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [integral extension](../../../../../integral-extension.md) $R\subseteq T$ means that every element $t\in T$ satisfies a [monic polynomial](../../../../../monic-polynomial.md) with coefficients in $R$:

$$
t^n+r_{n-1}t^{n-1}+\cdots+r_0=0.
$$

The [Krull dimension](../../../../../krull-dimension.md) is the supremum of the lengths of strict chains of primes:

$$
\boxed{\dim R=\sup\{n:\mathfrak p_0\subsetneq\mathfrak p_1\subsetneq\cdots\subsetneq\mathfrak p_n\}.}
$$

There need not be a finite bound on these lengths.

Here are the prime-ideal facts behind dimension preservation, with their relevant proofs. If a domain $B$ is integral over a subdomain $A$ and $B$ is a [field](../../../../../field.md), then $A$ is a [field](../../../../../field.md): for $0\neq a\in A$, a monic equation for $a^{-1}\in B$, multiplied by a suitable power of $a$, expresses $a^{-1}$ as an element of $A$. Conversely, an [integral domain](../../../../../integral-domain.md) integral over a [field](../../../../../field.md) is itself a [field](../../../../../field.md): a nonzero element has a polynomial equation with nonzero constant term after removing any factor of the indeterminate, and that equation expresses its inverse. Applied to quotients, these observations show that a prime in an [integral extension](../../../../../integral-extension.md) is maximal if and only if its contraction is maximal.

For the [Lying-over theorem](../../../../../lying-over-theorem.md), localize $R\subseteq T$ at $S=R\setminus\mathfrak p$. The inclusion remains injective and integral, and $S^{-1}T$ is nonzero. Any [maximal ideal](../../../../../maximal-ideal.md) of $S^{-1}T$ contracts to the unique [maximal ideal](../../../../../maximal-ideal.md) of $R_{\mathfrak p}$, by the [field](../../../../../field.md) criterion just proved. The [prime ideal correspondence for localization](../../../../../prime-ideal-correspondence-for-localization.md) then gives a prime of $T$ contracting to $\mathfrak p$.

For the [going-up theorem](../../../../../going-up-theorem.md), suppose $\mathfrak q$ lies over $\mathfrak p$ and $\mathfrak p\subseteq\mathfrak p'$. The quotient inclusion $R/\mathfrak p\subseteq T/\mathfrak q$ is integral. Apply [Lying-over theorem](../../../../../lying-over-theorem.md) to the prime $\mathfrak p'/\mathfrak p$; lifting back gives $\mathfrak q'\supseteq\mathfrak q$ contracting to $\mathfrak p'$.

For the [incomparability theorem for integral extensions](../../../../../incomparability-theorem-for-integral-extensions.md), suppose $\mathfrak q\subseteq\mathfrak q'$ contract to the same $\mathfrak p$. After localizing at $R\setminus\mathfrak p$, both are maximal [ideals](../../../../../ideal.md), because they lie over the [maximal ideal](../../../../../maximal-ideal.md) of $R_{\mathfrak p}$. Their inclusion is therefore equality. The bijection between primes under localization gives $\mathfrak q=\mathfrak q'$.

Now contract a strict chain of primes in $T$. [Incomparability theorem for integral extensions](../../../../../incomparability-theorem-for-integral-extensions.md) ensures that every contraction remains strict, so $\dim T\leq\dim R$. Conversely, [Lying-over theorem](../../../../../lying-over-theorem.md) lifts the first member of any finite chain in $R$, and repeated [going-up theorem](../../../../../going-up-theorem.md) lifts the remaining members; different contractions ensure a strict chain in $T$. Taking suprema, including the possibility of infinity, gives

$$
\boxed{\dim T=\dim R.}
$$

This proves that [integral extensions preserve Krull dimension](../../../../../integral-extensions-preserve-krull-dimension.md).

For the given quotient, put $B=k[Y][X]/(X^2+YX+Y^3)$. The relation is monic in $X$, so [monic polynomial](../../../../../monic-polynomial.md) division gives a unique representative $a(Y)+b(Y)X$. Thus $k[Y]\hookrightarrow B$ is injective and $B$ is free of rank two as a $k[Y]$-module. In particular, $B$ is integral over $k[Y]$. The one-variable polynomial [ring](../../../../../ring.md) has dimension one: its zero prime is strictly below $(Y)$, and every nonzero prime is maximal because $k[Y]$ is a principal [ideal](../../../../../ideal.md) domain. Hence

$$
\boxed{\dim k[X,Y]/(XY+X^2+Y^3)=1.}
$$

This is an instance of [dimension of a monic plane hypersurface](../../../../../dimension-of-a-monic-plane-hypersurface.md). No irreducibility or algebraic-closure assumption on $k$ is needed; monicity supplies the [integral extension](../../../../../integral-extension.md) in every characteristic.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
