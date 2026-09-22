<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $e_1(x),\ldots,e_n(x)$ be the prescribed ordered orthonormal framing. The [unordered Stiefel bundle](../../../../../unordered-stiefel-bundle.md) is the quotient of the orthonormal $k$-frame bundle by the action of the [symmetric group](../../../../../symmetric-group.md) permuting its frame vectors. Inside it take only the unordered subsets of the distinguished framing:

$$
X_k=\{(x,\{e_{a_1}(x),\ldots,e_{a_k}(x)\}):\{a_1,\ldots,a_k\}\subseteq\{1,\ldots,n\}\}.
$$

Projection onto $x$ defines the [subset cover of a framed vector bundle](../../../../../subset-cover-of-a-framed-vector-bundle.md) $p_k:X_k\to X$. Each sheet is globally labeled by a $k$-element index subset, so

$$
X_k\cong X\times\binom{\{1,\ldots,n\}}k,
$$

and this is a $\binom nk$-sheeted cover. The whole unordered Stiefel fiber is generally continuous, not this finite cover; it is the specified framing that selects these sheets. Even if the given framing is only continuous, the product description gives the covering its smooth structure.

A covering is a local diffeomorphism, with $TX_k\cong p_k^*TX$, so its relative normal data has the canonical rank-zero [stable framing of a vector bundle](../../../../../stable-framing-of-a-vector-bundle.md). Its degree-zero [framed cobordism](../../../../../framed-cobordism.md) transfer defines

$$
\boxed{l_k(\eta)=(p_k)_!(1)\in\Omega_{fr}^0(X).}
$$

These are the [exotic subset-cover classes of a framed bundle](../../../../../exotic-subset-cover-class-of-a-framed-bundle.md). Set $l_0=1$, using the identity cover, and $l_k=0$ outside $0\le k\le n$.

For framed bundles $\eta,\zeta$ of ranks $n,m$, use the concatenated framing of their [direct sum](../../../../../direct-sum.md). A $k$-element subset uniquely contains $i$ vectors from the first frame and $j$ from the second, where $i+j=k$. This gives an isomorphism of framed covers over $X$,

$$
X_k(\eta\oplus\zeta)\cong
\coprod_{i+j=k}\bigl(X_i(\eta)\times_X X_j(\zeta)\bigr).
$$

Transfer is additive under disjoint union, since the tubular collapse is the sum of the collapses of the disjoint sheets. It is multiplicative under fiber product: external products of the two collapse and Thom constructions give the transfer of the product cover over $X\times X$, and pullback by the diagonal gives the fiber-product cover over $X$. Its product framing is exactly the canonical relative framing used here. Consequently

$$
\boxed{l_k(\eta\oplus\zeta)=\sum_{i+j=k}l_i(\eta)l_j(\zeta).}
$$

With the literal globally ordered framing in the question, these covers are all trivial and each sheet is the identity map with its canonical relative framing. Thus their classes simplify further to

$$
l_k(\eta)=\binom nk\,1,\qquad\sum_{k=0}^n l_k(\eta)t^k=(1+t)^n.
$$

The displayed sum formula then also follows from the binomial convolution. Nontrivial covering monodromy would require only an unordered frame reduction, rather than the global ordered frame assumed here. In particular no extra nonconstant characteristic classes are produced by this literal construction. The original PDF places these classes in degree zero; the converted TeX's degree $-1$ and omitted letter $l$ are transcription errors.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
