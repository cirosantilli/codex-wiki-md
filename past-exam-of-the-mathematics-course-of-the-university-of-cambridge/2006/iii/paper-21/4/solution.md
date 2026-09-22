<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a complex bundle $E$, write $c_t(E)=\sum_{j\geq0}c_j^{MU}(E)t^j$, with $c_0(E)=1$ and $c_j(E)=0$ for $j>\operatorname{rank}_{\mathbb C}E$. The [Whitney sum formula for Chern classes](../../../../../whitney-sum-formula-for-chern-classes.md) in [complex cobordism](../../../../../complex-cobordism.md) is

$$
\boxed{c_t(\eta\oplus\xi)=c_t(\eta)c_t(\xi),\qquad
c_k(\eta\oplus\xi)=\sum_{a+b=k}c_a(\eta)c_b(\xi).}
$$

Products are in the complex-cobordism cohomology ring; these classes have even degrees $2j$. The [splitting principle for complex vector bundles](../../../../../splitting-principle-for-complex-vector-bundles.md) explains the formula: on a splitting space the [Chern classes](../../../../../chern-class.md) are elementary symmetric functions of the first [Chern classes](../../../../../chern-class.md) of the line summands, and joining the two lists multiplies their total Chern polynomials.

Use the line convention for the [projective bundle](../../../../../projective-bundle.md):

$$
\mathbb{CP}(\eta)=\{(x,\ell):x\in X,\ \ell\subset\eta_x\text{ is a complex line}\}.
$$

Its [relative tautological line bundle](../../../../../relative-tautological-line-bundle.md) is

$$
\eta(1)=\{((x,\ell),v):v\in\ell\}\longrightarrow\mathbb{CP}(\eta).
$$

It is a complex rank-one subbundle of $p^*\eta$. Choose a [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) and let $E=\eta(1)^\perp$, of rank $n-1$, so $p^*\eta=\eta(1)\oplus E$.

Throughout, $x=c_1^{MU}(\eta(1))$, the tautological line's class, as specified before the final equation. Put $a_k=p^*c_k^{MU}(\eta)$ and $b_k=c_k^{MU}(E)$, with $a_0=b_0=1$. Since $c_t(\eta(1))=1+xt$, Whitney multiplication gives

$$
\sum_{k=0}^{n}a_kt^k=(1+xt)\sum_{k=0}^{n-1}b_kt^k.
$$

Comparison of coefficients gives $a_k=b_k+xb_{k-1}$, hence recursively $b_k=a_k-xb_{k-1}$. Therefore the [Chern classes of a tautological-line complement](../../../../../chern-classes-of-a-tautological-line-complement.md) are

$$
\boxed{c_k^{MU}(\eta(1)^\perp)
=\sum_{j=0}^{k}(-1)^j x^j\,p^*c_{k-j}^{MU}(\eta)
\quad(0\leq k\leq n-1),}
$$

and the classes for $k\geq n$ vanish by the rank.

At degree $n$ the same recursion has $b_n=0$, giving

$$
0=a_n-xa_{n-1}+x^2a_{n-2}-\cdots+(-1)^nx^n.
$$

Multiplying by $(-1)^n$ proves the [projective bundle relation in complex cobordism](../../../../../projective-bundle-relation-in-complex-cobordism.md)

$$
\boxed{x^n-p^*c_1^{MU}(\eta)x^{n-1}
+p^*c_2^{MU}(\eta)x^{n-2}-\cdots+(-1)^np^*c_n^{MU}(\eta)=0.}
$$

These alternating signs come from the inverse formal power series $(1+xt)^{-1}$. They do not require identifying the [First Chern class](../../../../../first-chern-class.md) of a dual line with $-x$, which is generally incorrect in [complex cobordism](../../../../../complex-cobordism.md).

The final sentence's designation $x=c_1(\eta)$ must mean the earlier $c_1(\eta(1))$. If instead one substitutes $p^*c_1(\eta)$ literally, the claimed relation is false even in ordinary cohomology. For example, take $\eta=L\oplus L$ over $\mathbb{CP}^2$, with $a=c_1(L)$ a generator. Its [projective bundle](../../../../../projective-bundle.md) is $\mathbb{CP}^2\times\mathbb{CP}^1$, and $p^*a^2\ne0$. With the incorrect substitution $x=2p^*a$, the rank-two polynomial evaluates to

$$
(2p^*a)^2-(2p^*a)(2p^*a)+p^*a^2=p^*a^2\ne0.
$$

The tautological-line interpretation above is the one consistent with the bundle decomposition and the stated relation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
