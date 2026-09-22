<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First include the [trivial absolute value](../../../../../../trivial-absolute-value.md) if that convention is allowed. For a nontrivial [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md) on $\mathbb Q$, every integer has [absolute value on a field](../../../../../../absolute-value-algebra.md) at most one, and some nonzero integer has [absolute value on a field](../../../../../../absolute-value-algebra.md) less than one: otherwise every nonzero [rational number](../../../../../../rational-number.md), being a quotient of two integers, would have [absolute value on a field](../../../../../../absolute-value-algebra.md) one. Factoring that integer shows that some [prime number](../../../../../../prime-number.md) $p$ has $|p|<1$.

There cannot be two such [prime numbers](../../../../../../prime-number.md). If $|p|<1$ and $|q|<1$ for distinct [prime numbers](../../../../../../prime-number.md), choose integers $a,b$ with $ap+bq=1$. Then the [ultrametric inequality](../../../../../../ultrametric-inequality.md) gives

$$
1=|1|\leq\max(|a||p|,|b||q|)<1.
$$

Every other [prime number](../../../../../../prime-number.md) therefore has [absolute value on a field](../../../../../../absolute-value-algebra.md) one. Factoring numerator and denominator of a [rational number](../../../../../../rational-number.md) gives

$$
|x|=|p|^{v_p(x)}=|x|_p^c,\qquad
c=\frac{-\log |p|}{\log p}>0.
$$

Thus the nontrivial equivalence classes are precisely the [p-adic absolute values](../../../../../../p-adic-absolute-value.md), one for each [prime number](../../../../../../prime-number.md).

Now let $F$ be a [number field](../../../../../../number-field.md), with [ring of integers of a number field](../../../../../../ring-of-integers.md) $A$. If the restriction of an [absolute value on a field](../../../../../../absolute-value-algebra.md) to $\mathbb Q$ is trivial, a [monic polynomial](../../../../../../monic-polynomial.md) over $\mathbb Q$ satisfied by $x\in F$ forces $|x|\leq1$: if $|x|>1$, its leading term would strictly dominate the other terms. Applying the same argument to $x^{-1}$ forces $|x|=1$ for $x\ne0$. Thus a nontrivial [absolute value on a field](../../../../../../absolute-value-algebra.md) defined on $F$ has a nontrivial restriction, associated with some [prime number](../../../../../../prime-number.md) $p$.

Every $a\in A$ has $|a|\leq1$, by applying the same leading-term argument to its monic integral equation. Consequently

$$
\mathfrak p=\{a\in A:|a|<1\}
$$

is a proper [prime ideal](../../../../../../prime-ideal.md): it is an ideal by the [ultrametric inequality](../../../../../../ultrametric-inequality.md), and $|ab|<1$ with $|a|,|b|\leq1$ implies that at least one factor has [absolute value on a field](../../../../../../absolute-value-algebra.md) less than one. It is nonzero because it contains $p$.

The [localization](../../../../../../localization-of-a-ring.md) $A_{\mathfrak p}$ lies in the [valuation ring](../../../../../../valuation-ring.md) of the [absolute value on a field](../../../../../../absolute-value-algebra.md): a denominator outside $\mathfrak p$ has [absolute value on a field](../../../../../../absolute-value-algebra.md) one. Since $A$ is a [Dedekind domain](../../../../../../dedekind-domain.md), $A_{\mathfrak p}$ is a [discrete valuation ring](../../../../../../discrete-valuation-ring.md). Choose its [uniformizer](../../../../../../uniformizer.md) $\pi$. Each $x\in F^\times$ has a unique expression

$$
x=\pi^m u,\qquad m=v_{\mathfrak p}(x),\quad u\in A_{\mathfrak p}^{\times}.
$$

Both $u$ and $u^{-1}$ lie in the [valuation ring](../../../../../../valuation-ring.md), so $|u|=1$. Also $\pi$ belongs to its [maximal ideal](../../../../../../maximal-ideal.md), hence $|\pi|<1$. Therefore $|x|=|\pi|^{v_{\mathfrak p}(x)}$.

Conversely each nonzero [prime ideal](../../../../../../prime-ideal.md) of $A$ gives the [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md) $|x|=c^{v_{\mathfrak p}(x)}$ for any $0<c<1$, using the [discrete valuation](../../../../../../discrete-valuation.md) of $A_{\mathfrak p}$. All choices of $c$ are equivalent, and different [prime ideals](../../../../../../prime-ideal.md) are distinguished by the elements of $A$ having [absolute value on a field](../../../../../../absolute-value-algebra.md) less than one. We have proved [Non-Archimedean absolute values on a number field](../../../../../../non-archimedean-absolute-values-on-a-number-field.md):

$$
\boxed{\{\text{nontrivial equivalence classes on }F\}
\longleftrightarrow
\{\text{nonzero prime ideals of }\mathcal O_F\}.}
$$

The trivial class is additional when trivial [absolute values on a field](../../../../../../absolute-value-algebra.md) are admitted.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
