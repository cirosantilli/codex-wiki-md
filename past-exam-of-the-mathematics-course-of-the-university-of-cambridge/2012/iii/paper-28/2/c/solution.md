<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The polynomial is an [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md) at $5$, so it is irreducible and $[K:\mathbb Q]=3$. Its [polynomial discriminant](../../../../../../polynomial-discriminant.md) is

$$
\operatorname{disc}(f)=500-10800=-10300=-4\cdot5^2\cdot103.
$$

One must remove the index at $2$ before using this as the [field discriminant](../../../../../../field-discriminant.md). Put $\beta=(\alpha^2+\alpha)/2$. Direct reduction using $\alpha^3=5\alpha-20$ gives

$$
\alpha^2=2\beta-\alpha,\quad \alpha\beta=2\alpha+\beta-10,\quad \beta^2=3\beta-4\alpha-10.
$$

Thus $B=\mathbb Z+\mathbb Z\alpha+\mathbb Z\beta$ is a ring finite over $\mathbb Z$, so its elements are integral. Its basis has [discriminant of elements of a number field](../../../../../../discriminant-of-elements-of-a-number-field.md) $-2575=-5^2\cdot103$. The [discriminant-index formula for an integral lattice](../../../../../../discriminant-index-formula-for-an-integral-lattice.md) says $\operatorname{disc}(B)=[\mathcal O_K:B]^2\Delta_K$, so only $5$ could divide the remaining index.

We use these standard [different ideal](../../../../../../different-ideal.md) facts: the norm of the different is the absolute [field discriminant](../../../../../../field-discriminant.md); its localization is the local different; an unramified prime has different exponent zero, and a tamely ramified prime of [ramification index](../../../../../../ramification-index.md) $e$ has different exponent $e-1$. The [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md) at $5$ gives total ramification of degree three, which is tame because $5\nmid3$. Its contribution to $v_5(\Delta_K)$ is therefore two. This excludes a further index factor $5$, proving **$\mathcal O_K=B$ and $\boxed{\Delta_K=-2575}$.**

Since the index $[\mathcal O_K:\mathbb Z[\alpha]]=2$ is prime to $5$ and $103$, [Dedekind factorization theorem](../../../../../../dedekind-factorization-theorem.md) applies at both primes. Modulo $5$, $f=X^3$, giving a single prime $\mathfrak p=(5,\alpha)$ with [residue degree](../../../../../../residue-degree.md) one and [ramification index](../../../../../../ramification-index.md) three. Modulo $103$,

$$
f(X)=(X-6)^2(X+12).
$$

Thus $\mathfrak q=(103,\alpha-6)$ has [residue degree](../../../../../../residue-degree.md) one and [ramification index](../../../../../../ramification-index.md) two; the other prime over $103$ is unramified. Both ramified primes are tame. No other prime ramifies because none divides $\Delta_K$. **Consequently**

$$
\boxed{\mathfrak D_{K/\mathbb Q}=\mathfrak p^2\mathfrak q,\qquad N\mathfrak p=5,\quad N\mathfrak q=103.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
