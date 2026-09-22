<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the following simple-root [Hensel lemma](../../../../../hensel-s-lemma.md). Let $R$ be a [complete discrete valuation ring](../../../../../complete-discrete-valuation-ring.md), with maximal [ideal](../../../../../ideal.md) $\mathfrak m$, and let $f\in R[X]$. If $f(a_0)\in\mathfrak m$ and $f'(a_0)\in R^*$, there is a unique $a\in R$ with $a\equiv a_0\pmod{\mathfrak m}$ and $f(a)=0$.

For the proof, define [Newton's method](../../../../../newton-s-method-in-optimization.md) iterates $a_{r+1}=a_r-f(a_r)/f'(a_r)$. Each denominator stays a unit, because all iterates are congruent to $a_0$. Taylor's polynomial identity gives

$$
v(f(a_{r+1}))\geq2v(f(a_r)),\qquad
v(a_{r+1}-a_r)=v(f(a_r)).
$$

If an iterate is already a root, the process stops. Otherwise these [valuations](../../../../../valuation.md) tend to infinity, so the iterates form a [Cauchy sequence](../../../../../cauchy-sequence.md) in the complete ring. Its limit $a$ has the required residue and satisfies $f(a)=0$. If $a,b$ were two such roots, then

$$
f(a)-f(b)=(a-b)\big(f'(b)+(a-b)h(a,b)\big).
$$

The parenthesis is a unit, forcing $a=b$.

Now let $K/\mathbb Q_p$ be finite, with [residue field](../../../../../residue-field.md) $k=\mathbb F_q$. For every $m\geq1$ choose a monic irreducible polynomial $\bar f\in k[X]$ of degree $m$ and lift it to a monic $f\in\mathcal O_K[X]$. The lift is irreducible over $K$, since a factorization would reduce to a factorization of $\bar f$, by the monic form of [Gauss's lemma](../../../../../gauss-s-lemma-riemannian-geometry.md) over the [valuation](../../../../../valuation.md) ring. If $L=K(\alpha)$ for a root, its [residue field](../../../../../residue-field.md) contains $k(\bar\alpha)$ of degree $m$. The inequality $e(L/K)f(L/K)\leq[L:K]=m$ forces [residue degree](../../../../../residue-degree.md) $m$ and [ramification index](../../../../../ramification-index.md) one. Thus it is an [unramified extension](../../../../../unramified-extension.md) of degree $m$.

Conversely, in any [unramified extension](../../../../../unramified-extension.md) of degree $m$, choose a generator of its [residue field](../../../../../residue-field.md) and lift its separable minimal polynomial. Hensel's lemma supplies a root with that residue. Its degree is at least $m$ and hence it generates the extension. The same unique lifting of all residue conjugates shows that the extension is Galois and

$$
\boxed{\operatorname{Gal}(K_m/K)\cong\operatorname{Gal}(\mathbb F_{q^m}/\mathbb F_q)\cong C_m.}
$$

One can see uniqueness inside a fixed algebraic closure explicitly: the roots of $X^{q^m-1}-1$ lift all nonzero residue elements, and a lifted primitive residue element generates the extension. Hence

$$
\boxed{K_m=K(\mu_{q^m-1}),}
$$

with [arithmetic Frobenius](../../../../../frobenius-automorphism.md) acting by $\zeta\mapsto\zeta^q$. The case $q^m-1=1$ simply gives $K_1=K$. These are all finite [unramified extensions](../../../../../unramified-extension.md); $K_m\subseteq K_r$ exactly when $m\mid r$. Their union is the maximal [unramified extension](../../../../../unramified-extension.md), whose [Galois group](../../../../../galois-group.md) is $\widehat{\mathbb Z}$.

Finally prove norm-surjectivity on units using the [Herbrand quotient](../../../../../herbrand-quotient.md). For a [cyclic group](../../../../../cyclic-group.md) $G$ of order $m$, write

$$
h_G(M)=\frac{\#\widehat H^0(G,M)}{\#\widehat H^{-1}(G,M)}.
$$

The quotient is multiplicative on short exact sequences, equals one for finite modules, equals $m$ on the trivial module $\mathbb Z$, and equals one on induced regular modules. For a finite module, the equality follows directly from $|M^G||(\sigma-1)M|=|M|=|\ker N||NM|$.

Let $U_L=\mathcal O_L^*$. For sufficiently large $r$, the equivariant [p-adic logarithm](../../../../../p-adic-logarithm.md) identifies $U_L^r=1+\mathfrak p_L^r$ with $\mathfrak p_L^r$ additively. In the unramified case this is an induced regular lattice. Indeed choose a normal basis of the finite residue extension and lift its generating element. Its $m$ Galois conjugates reduce to a basis and hence form an $\mathcal O_K$-basis of $\mathcal O_L$; their coordinate determinant is a unit. Since a [uniformizer](../../../../../uniformizer.md) of $K$ is also one of $L$, multiplication by its $r$th power gives the same regular-module structure on $\mathfrak p_L^r$. For a regular module, invariants are norm images and a vector of coefficient sum zero is a cyclic difference, so both indicated [Tate cohomology](../../../../../tate-cohomology-of-a-finite-group.md) groups vanish. Consequently $h_G(U_L^r)=1$. The quotient $U_L/U_L^r$ is finite, so $h_G(U_L)=1$.

Apply multiplicativity to

$$
1\longrightarrow U_L\longrightarrow L^*\xrightarrow{v_L}\mathbb Z\longrightarrow0.
$$

It gives $h_G(L^*)=m$. [Hilbert 90](../../../../../hilbert-s-theorem-90.md) makes $\widehat H^{-1}(G,L^*)$ trivial, so $[K^*:N_{L/K}L^*]=m$. On the other hand

$$
v_K(N_{L/K}b)=m\,v_L(b),
$$

so the quotient maps onto $\mathbb Z/m\mathbb Z$. As its order is already $m$, its unit kernel is trivial. A norm which is a unit comes from a unit, by the same [valuation](../../../../../valuation.md) formula. Therefore

$$
\boxed{N_{L/K}(U_L)=U_K.}
$$

The standard normal-basis theorem for [finite fields](../../../../../finite-field.md) and the convergent logarithm/exponential on sufficiently deep principal units are the ingredients used in evaluating the [Herbrand quotient](../../../../../herbrand-quotient.md); the norm conclusion itself has been deduced here.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
