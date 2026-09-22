<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An extension $A\subseteq B$ is an [integral extension](../../../../../integral-extension.md) when every $b\in B$ is an [integral element](../../../../../integral-element.md) over $A$, meaning that

$$
b^n+a_{n-1}b^{n-1}+\cdots+a_0=0\qquad(a_i\in A)
$$

for some monic polynomial. The [Krull dimension](../../../../../krull-dimension.md) of a [ring](../../../../../ring.md) is the supremum of the lengths $r$ of strict chains $\mathfrak p_0\subsetneq\cdots\subsetneq\mathfrak p_r$ of [prime ideals](../../../../../prime-ideal.md); the number counted is the number of inclusions.

We prove the prime-chain facts needed for [integral extensions preserve Krull dimension](../../../../../integral-extensions-preserve-krull-dimension.md). Taking quotients preserves an integral equation. Localizing both rings by the same multiplicative subset of $A$ also preserves integrality: for $b/s$, divide the equation for $b$ by $s^n$, so its new coefficients are $a_i/s^{n-i}$. Localizing just $B$ at all elements outside one of its primes would not be the same operation.

Two elementary field observations are useful. If a [field](../../../../../field.md) $C$ is integral over a subdomain $R$, then $R$ is a [field](../../../../../field.md), by the inverse argument given in Question 2. Conversely, if an [integral domain](../../../../../integral-domain.md) $C$ is integral over a [field](../../../../../field.md) $R$, every nonzero $c\in C$ has a monic equation with nonzero constant term: cancel a factor of $c$ from an equation if necessary. Dividing by $c$ and by that constant term expresses $c^{-1}$ as a polynomial in $c$. Thus $C$ is a [field](../../../../../field.md). In particular, the contraction of a [maximal ideal](../../../../../maximal-ideal.md) under an [integral extension](../../../../../integral-extension.md) is maximal.

For the [Lying-over theorem](../../../../../lying-over-theorem.md), fix $\mathfrak p\in\operatorname{Spec}A$ and localize by $S=A\setminus\mathfrak p$. The nonzero domain $S^{-1}B$ is integral over the local ring $A_{\mathfrak p}$. Choose a [maximal ideal](../../../../../maximal-ideal.md) $\mathfrak n$ of $S^{-1}B$. Its contraction is maximal in $A_{\mathfrak p}$, so it is the unique maximal ideal $\mathfrak pA_{\mathfrak p}$. The [prime ideal correspondence for localization](../../../../../prime-ideal-correspondence-for-localization.md) now pulls $\mathfrak n$ back to a [prime ideal](../../../../../prime-ideal.md) $\mathfrak q$ of $B$ with $\mathfrak q\cap A=\mathfrak p$.

For the [going-up theorem](../../../../../going-up-theorem.md), suppose $\mathfrak p\subseteq\mathfrak p'$ and $\mathfrak q\cap A=\mathfrak p$. The injection $A/\mathfrak p\hookrightarrow B/\mathfrak q$ is still integral. Apply the just-proved [Lying-over theorem](../../../../../lying-over-theorem.md) to $\mathfrak p'/\mathfrak p$. Pulling the resulting prime back gives $\mathfrak q'\supseteq\mathfrak q$ with $\mathfrak q'\cap A=\mathfrak p'$.

For the [incomparability theorem for integral extensions](../../../../../incomparability-theorem-for-integral-extensions.md), suppose $\mathfrak q\subseteq\mathfrak q'$ have the same contraction $\mathfrak p$. Write $R=A/\mathfrak p$ and $C=B/\mathfrak q$. The latter is a domain integral over $R$. Localizing both by $R\setminus\{0\}$ makes $S^{-1}C$ integral over the [fraction field](../../../../../field-of-fractions.md) of $R$, so $S^{-1}C$ is a [field](../../../../../field.md). The prime $\mathfrak q'/\mathfrak q$ is disjoint from $S$ and therefore localizes to a proper prime, which must be zero in this [field](../../../../../field.md). Since $C$ is a domain and all denominators are nonzero, an element of $C$ whose localization is zero was already zero. Hence $\mathfrak q'/\mathfrak q=0$, proving $\mathfrak q' =\mathfrak q$.

A strict prime chain in $B$ therefore contracts to a strict chain in $A$, giving $\dim B\leq\dim A$. Conversely, start over the bottom of any finite prime chain in $A$ using [Lying-over theorem](../../../../../lying-over-theorem.md), and successively use [going-up theorem](../../../../../going-up-theorem.md) to lift the entire chain. Distinct contractions ensure that the lifted inclusions are strict, giving the reverse inequality. Taking suprema, including when arbitrarily long chains exist, proves

$$
\boxed{\dim B=\dim A.}
$$

For an algebraic extension $K/\mathbb Q$, its ring $\mathcal O$ of algebraic integers is an [integral extension](../../../../../integral-extension.md) of $\mathbb Z$. The primes of $\mathbb Z$ are $(0)$ and the maximal ideals $(p)$, so the longest strict chains have length one; for example $(0)\subsetneq(2)$. The preceding argument yields

$$
\boxed{\dim\mathcal O=\dim\mathbb Z=1.}
$$

This [Krull dimension of rings of algebraic integers](../../../../../krull-dimension-of-rings-of-algebraic-integers.md) argument also covers infinite algebraic extensions. It uses integrality, not an assumption that $K$ is a [number field](../../../../../number-field.md) or that $\mathcal O$ is Noetherian.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
