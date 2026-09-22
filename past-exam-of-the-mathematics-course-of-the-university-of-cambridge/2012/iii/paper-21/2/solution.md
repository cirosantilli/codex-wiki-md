<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a complete discretely valued field with perfect [residue field](../../../../../residue-field.md) $k$, the [Witt residue sequence](../../../../../witt-residue-sequence.md) is the split exact sequence

$$
0\longrightarrow\operatorname{Br}(k)\longrightarrow\operatorname{Br}(K)
\xrightarrow{\partial_K}H^1(k,\mathbb Q/\mathbb Z)\longrightarrow0.
$$

The first map identifies the unramified Brauer classes. The residue map is canonical; a splitting is chosen by a [uniformizer](../../../../../uniformizer.md) $\pi$ and sends an unramified character $\chi$ to the cyclic Brauer class $(\chi,\pi)$. Changing $\pi$ may change this splitting by an unramified class. This is the version of Witt's theorem used here.

Now suppose $k=\mathbb F_q$. Fix arithmetic Frobenius $F_k:a\mapsto a^q$. Define the [local Brauer invariant](../../../../../local-brauer-invariant.md) by

$$
\boxed{\operatorname{inv}_K(\alpha)=\partial_K(\alpha)(F_k)\in\mathbb Q/\mathbb Z}.
$$

Here is an explicit cohomological construction. Set $E=K^{\mathrm{nr}}$ and $G=\operatorname{Gal}(E/K)\cong\widehat{\mathbb Z}$. The permitted vanishing $\operatorname{Br}(E)=0$, together with [Hilbert 90](../../../../../hilbert-s-theorem-90.md) and inflation, identifies $\operatorname{Br}(K)$ with $H^2(G,E^\times)$. Normalize the valuation $v(\pi)=1$. Its induced map sends a multiplicative two-cocycle $c$ to the integer-valued two-cocycle $v(c)$, giving

$$
\operatorname{Br}(K)\longrightarrow H^2(G,\mathbb Z)
\xrightarrow{\ \delta^{-1}\ }H^1(G,\mathbb Q/\mathbb Z)
\xrightarrow{\ \chi\mapsto\chi(F_k)\ }\mathbb Q/\mathbb Z.
$$

The middle isomorphism is the connecting map for $0\to\mathbb Z\to\mathbb Q\to\mathbb Q/\mathbb Z\to0$, since positive-degree continuous cohomology of the trivial module $\mathbb Q$ vanishes.

To see that the valuation map is an isomorphism, its module sequence splits using $\pi$, and the unit part has zero second cohomology. For each finite unramified cyclic extension $E_m/K$, cyclic cohomology identifies that unit contribution with $\mathcal O_K^\times/N_{E_m/K}\mathcal O_{E_m}^\times$. The norm on residue-field units is surjective. On the principal-unit quotient of level $r\ge1$, the norm is the residue trace, through $N(1+\pi^rb)\equiv1+\pi^r\operatorname{Tr}(\overline b)\pmod{\pi^{r+1}}$. The trace of a finite separable [field extension](../../../../../field-extension.md) is surjective; successive corrections and completeness therefore make the norm surjective on all units. Passing to the direct limit gives the asserted vanishing. Finally, a continuous character of $\widehat{\mathbb Z}$ is uniquely specified by its value on arithmetic Frobenius, and that value can be any element of $\mathbb Q/\mathbb Z$. **The invariant map is an isomorphism.**

In concrete terms, if $E_m/K$ is the [unramified extension](../../../../../unramified-extension.md) of degree $m$ and $\sigma$ lifts arithmetic Frobenius, the [cyclic algebra](../../../../../cyclic-algebra.md) with $ub=\sigma(b)u$ and $u^m=a$ has

$$
\operatorname{inv}_K(E_m/K,\sigma,a)=\frac{v_K(a)}m\pmod{\mathbb Z}.
$$

Indeed its standard two-cocycle has value $a$ when the powers of $\sigma$ wrap past $m$ and value one otherwise. Valuation turns this into the connecting cocycle for the character with Frobenius value $v_K(a)/m$. This also fixes the sign of the normalization.

For [restriction and corestriction of local Brauer invariants](../../../../../restriction-and-corestriction-of-local-brauer-invariants.md), let $l$ be the [residue field](../../../../../residue-field.md) of $L$, $e$ the [ramification index](../../../../../ramification-index.md) and $f=[l:k]$. A finite extension of [local fields](../../../../../local-field.md) has $[L:K]=ef$, $v_L|_K=e v_K$ and $v_K(N_{L/K}b)=f v_L(b)$. Every class of $\operatorname{Br}(K)$ is $(\chi,\pi_K)$, with $\chi$ unramified. After restriction to $L$, its character has Frobenius value $f\chi(F_k)$ and its parameter has valuation $e$. Thus

$$
\boxed{\operatorname{inv}_L(\operatorname{Res}_{L/K}\alpha)=[L:K]\operatorname{inv}_K(\alpha)}.
$$

For corestriction, write a class of $\operatorname{Br}(L)$ as $(\chi_l,\pi_L)$. Choose a character $\chi_k$ of the finite-field absolute group such that $\operatorname{Res}_{l/k}\chi_k=\chi_l$. This is possible because restriction is multiplication by $f$ on $\mathbb Q/\mathbb Z$, which is divisible. Inflate both characters to the [local fields](../../../../../local-field.md). The [norm projection formula for cyclic Brauer pairings](../../../../../norm-projection-formula-for-cyclic-brauer-pairings.md) gives

$$
\operatorname{Cor}_{L/K}(\chi_l,\pi_L)=(\chi_k,N_{L/K}\pi_L).
$$

This projection identity follows from the cohomological transfer and cup-product identity; on multiplicative degree-zero coefficients transfer is the [field norm](../../../../../field-norm.md), and the identity in higher degree follows by the cochain definition or dimension shifting. The norm parameter has $K$-valuation $f$, so its invariant is $f\chi_k(F_k)=\chi_l(F_l)$. Therefore

$$
\boxed{\operatorname{inv}_K(\operatorname{Cor}_{L/K}\beta)=\operatorname{inv}_L(\beta)}.
$$

This argument uses the character-and-norm description directly and does not cancel multiplication by $[L:K]$ in $\mathbb Q/\mathbb Z$, where such cancellation would be invalid. For purely inseparable steps in equal characteristic, [absolute Galois groups](../../../../../absolute-galois-group.md) identify, restriction uses inclusion of multiplicative coefficient modules, and Brauer corestriction uses the [field norm](../../../../../field-norm.md) on them. The same projection calculation applies. Factoring a general finite extension into separable and purely inseparable steps covers all finite extensions in the question.

Lastly, a class with invariant $a/b$ in lowest terms has [Brauer period](../../../../../period-of-a-brauer-class.md) $b$. The [unramified extension](../../../../../unramified-extension.md) of degree $b$ splits it, so its division-algebra degree divides $b$. Conversely a maximal subfield of the [division algebra](../../../../../division-algebra.md) splits it and has degree equal to that division-algebra degree; the restriction formula forces $b$ to divide that degree. These standard splitting-field properties are among the permitted inputs. Thus the [index of a central simple algebra](../../../../../index-of-a-central-simple-algebra.md) equals its period over a [local field](../../../../../local-field.md). The [central division algebras](../../../../../central-division-algebra.md) of degree $n$ are exactly those with invariants $a/n$ and $\gcd(a,n)=1$. The Brauer class determines its division representative uniquely, so there are

$$
\boxed{\varphi(n)}
$$

isomorphism classes, where $\varphi$ is the Euler totient function. This includes the single degree-one algebra $K$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
