<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For distinct evaluation points $a_0,\ldots,a_{n-1}\in\mathbb F_q$ and $1\leq k\leq n$, the [Reed-Solomon code](../../../../../reed-solomon-error-correction.md) is

$$
\operatorname{RS}_k(a)=\{(f(a_0),\ldots,f(a_{n-1})):\ f\in\mathbb F_q[x],\ \deg f<k\}.
$$

This is a [linear code](../../../../../linear-code.md) of [dimension](../../../../../dimension-vector-space.md) $k$: evaluation is [linear](../../../../../linearity.md), and a nonzero [polynomial](../../../../../polynomial-split.md) of degree less than $k\leq n$ cannot vanish at all $n$ distinct points. The assertion of cyclicity concerns the primitive, unextended construction: set $n=q-1$ and $a_j=\omega^j$, where $\omega$ generates the [multiplicative group of a finite field](../../../../../multiplicative-group-of-a-finite-field.md) $\mathbb F_q^\times$. Arbitrary evaluation sets or arbitrary coordinate orders need not make a [Reed-Solomon code](../../../../../reed-solomon-error-correction.md) a [cyclic code](../../../../../cyclic-code.md).

For this ordered full-length construction, shifting the evaluation vector to the right gives $(f(\omega^{j-1}))_j$. This is the evaluation vector of $f(\omega^{-1}x)$, whose degree is still less than $k$, so it is a [cyclic code](../../../../../cyclic-code.md). Its [generator polynomial](../../../../../generator-polynomial-of-a-cyclic-code.md) follows from the [finite geometric series](../../../../../finite-geometric-series.md)

$$
\sum_{j=0}^{n-1}\omega^{jt}=\begin{cases}n,&n\mid t,\\0,&n\nmid t.\end{cases}
$$

Here the scalar $n=q-1$ is nonzero in $\mathbb F_q$. Write $f(x)=\sum_{a=0}^{k-1}m_ax^a$ and $c(x)=\sum_{j=0}^{n-1}f(\omega^j)x^j$. For $1\leq\ell\leq n-k$,

$$
c(\omega^\ell)=\sum_{a=0}^{k-1}m_a\sum_{j=0}^{n-1}\omega^{j(a+\ell)}=0,
$$

since $1\leq a+\ell\leq n-1$. Thus every word is divisible by $g(x)=\prod_{\ell=1}^{n-k}(x-\omega^\ell)$. This monic divisor of $x^n-1$ generates a [cyclic code](../../../../../cyclic-code.md) of [dimension](../../../../../dimension-vector-space.md) $n-(n-k)=k$, equal to the evaluation code by inclusion and dimension. Hence

$$
\boxed{\operatorname{RS}_k(1,\omega,\ldots,\omega^{n-1})=\langle g\rangle,\qquad g(x)=\prod_{\ell=1}^{n-k}(x-\omega^\ell),\quad n=q-1.}
$$

It is useful to allow a starting exponent $b$ for the consecutive [zeros of a cyclic code](../../../../../zero-of-a-cyclic-code.md). Define the [primitive cyclic Reed-Solomon code](../../../../../primitive-cyclic-reed-solomon-code.md)

$$
C_{k,b}=\left\langle\prod_{\ell=b}^{b+n-k-1}(x-\omega^\ell)\right\rangle.
$$

All exponents are understood modulo $n$. The same geometric-sum calculation shows that

$$
C_{k,b}=\{(a_j^{1-b}f(a_j))_{j=0}^{n-1}:\deg f<k\}.
$$

Indeed evaluating its word polynomial at $\omega^{b+\ell}$, $0\leq\ell<n-k$, gives sums with exponents $a+1+\ell$ between one and $n-1$. This is a [generalized Reed-Solomon code](../../../../../generalized-reed-solomon-code.md), with nonzero coordinate multipliers $a_j^{1-b}$; $C_{k,1}$ is the unweighted evaluation code. Directly, a right shift corresponds to replacing $f(x)$ by $\omega^{b-1}f(\omega^{-1}x)$, so these offset codes are also [cyclic codes](../../../../../cyclic-code.md).

A [maximum distance separable code](../../../../../maximum-distance-separable-code.md), or [MDS code](../../../../../maximum-distance-separable-code.md), is a [linear code](../../../../../linear-code.md) attaining the [Singleton bound](../../../../../singleton-bound.md), with $d=n-k+1$. To see the bound, deleting any $d-1$ coordinates is injective on a code of [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md) $d$, since two words with the same puncture would differ in at most $d-1$ positions. Therefore $q^k\leq q^{n-d+1}$ and $d\leq n-k+1$. For a nonzero Reed-Solomon evaluation word, the [polynomial](../../../../../polynomial-split.md) has at most $k-1$ distinct [polynomial roots](../../../../../root-of-a-polynomial.md), so at least $n-k+1$ coordinates are nonzero. Nonzero coordinate multipliers do not change these zero positions. This proves $d\geq n-k+1$ for both [Reed-Solomon codes](../../../../../reed-solomon-error-correction.md) and [generalized Reed-Solomon codes](../../../../../generalized-reed-solomon-code.md). Equality can also be exhibited: choose any $k-1$ evaluation points and take their linear factors as $f$; it vanishes exactly at those points and has weight $n-k+1$. Thus

$$
\boxed{\operatorname{RS}_k\text{ and }C_{k,b}\text{ have parameters }[n,k,n-k+1]\text{ and are MDS codes}.}
$$

The [duality of primitive cyclic Reed-Solomon codes](../../../../../duality-of-primitive-cyclic-reed-solomon-codes.md) is especially transparent in the evaluation form. Assume first $1\leq k<n$. A vector of $C_{k,b}$ has coordinates $a_j^{1-b}f(a_j)$, $\deg f<k$; a vector of $C_{n-k,1-b}$ has coordinates $a_j^b h(a_j)$, $\deg h<n-k$. Their standard [dot product](../../../../../dot-product.md) is

$$
\sum_{j=0}^{n-1}a_j f(a_j)h(a_j)=0.
$$

Every monomial in $x f(x)h(x)$ has exponent at least one and at most $1+(k-1)+(n-k-1)=n-1$, and every such power sum vanishes. Thus $C_{n-k,1-b}\subseteq C_{k,b}^\perp$. Both sides have [dimension](../../../../../dimension-vector-space.md) $n-k$, giving

$$
\boxed{C_{k,b}^\perp=C_{n-k,1-b},\qquad g^\perp(x)=\prod_{\ell=1-b}^{k-b}(x-\omega^\ell).}
$$

In particular $C_{k,1}^\perp=C_{n-k,0}$ has generator $\prod_{\ell=0}^{k-1}(x-\omega^\ell)$. This agrees with the general [dual of a cyclic code](../../../../../dual-of-a-cyclic-code.md) rule: invert the roots belonging to the complementary factor $(x^n-1)/g$. The dual is a Reed-Solomon code in the consecutive-zero convention. With the strictly unweighted evaluation definition, its coordinates instead have the form $(a_jh(a_j))_j$, so it is a [generalized Reed-Solomon code](../../../../../generalized-reed-solomon-code.md); it need not equal the unweighted code of dimension $n-k$ on the same points. This convention distinction is essential. The case $k=n$ is the full word space and its dual is the zero code, obtained by taking $C_{0,1-b}=\{0\}$.

For [code encoding](../../../../../code-encoding.md), use the [finite-field discrete Fourier transform](../../../../../finite-field-discrete-fourier-transform.md) and its inverse:

$$
\widehat c_\ell=\sum_{j=0}^{n-1}c_j\omega^{j\ell},\qquad c_j=n^{-1}\sum_{\ell=0}^{n-1}\widehat c_\ell\omega^{-j\ell}.
$$

For a message $(m_0,\ldots,m_{k-1})$, put $\widehat c_{b-1-a}=n m_a$ for $0\leq a<k$, and set all other transform coordinates to zero. The [inverse discrete Fourier transform](../../../../../inverse-discrete-fourier-transform.md) returns

$$
\boxed{c_j=a_j^{1-b}\sum_{a=0}^{k-1}m_a a_j^a,\qquad a_j=\omega^j.}
$$

The $n-k$ zero transform coordinates are precisely the root checks defining $C_{k,b}$. This gives non-systematic encoding by evaluation. For [systematic polynomial encoding of a cyclic code](../../../../../systematic-polynomial-encoding-of-a-cyclic-code.md) with a message [polynomial](../../../../../polynomial-split.md) $M$ of degree less than $k$, put $r=n-k$ and calculate the remainder $R(x)$ of $x^rM(x)$ upon division by $g(x)$. Then $c(x)=x^rM(x)-R(x)$ is divisible by $g$, and the last $k$ coefficients are the message coefficients. Both methods use the same [generator polynomial](../../../../../generator-polynomial-of-a-cyclic-code.md) and the same ordered powers of $\omega$.

For [bounded-distance decoding](../../../../../bounded-distance-decoding.md), let $y=c+e$, put $r=n-k$, and assume at most $T=\lfloor r/2\rfloor$ symbol errors. The following description uses the [Reed-Solomon key equation](../../../../../reed-solomon-key-equation.md) and fixes the transform and locator conventions explicitly.


- Compute the [syndromes](../../../../../syndrome.md) $S_\ell=y(\omega^{b+\ell})=\widehat y_{b+\ell}$ for $0\leq\ell<r$. The corresponding codeword transform values vanish. An error of value $E_i$ at coordinate $j_i$ contributes $E_iX_i^{b+\ell}$, where $X_i=\omega^{j_i}$, so $S_\ell=\sum_iE_iX_i^{b+\ell}$.
- Form $S(z)=\sum_{\ell=0}^{r-1}S_\ell z^\ell$. Use the [Berlekamp-Massey algorithm](../../../../../berlekamp-massey-algorithm.md), or the polynomial [extended Euclidean algorithm](../../../../../extended-euclidean-algorithm.md) applied to $z^r$ and $S(z)$, to solve $\Lambda S\equiv\Omega\pmod{z^r}$ with $\Lambda(0)=1$, $\deg\Lambda=\nu\leq T$, and $\deg\Omega<\nu$. Choose the minimal-degree locator; zero syndrome gives $\Lambda=1$, $\Omega=0$. The [error locator polynomial](../../../../../error-locator-polynomial.md) is $\Lambda(z)=\prod_{i=1}^\nu(1-X_i z)$, and $\Omega$ is the [error evaluator polynomial](../../../../../error-evaluator-polynomial.md).
- Perform a [Chien search](../../../../../chien-search.md): test $\Lambda(\omega^{-j})$ for $0\leq j<n$. Its $\nu$ distinct zeros identify the erroneous coordinates. A mismatch between the degree and the number of distinct permitted roots is a decoding failure.
- Recover each error value by the [Forney algorithm](../../../../../forney-algorithm.md), with the present syndrome offset:


$$
\boxed{E_i=-X_i^{1-b}\frac{\Omega(X_i^{-1})}{\Lambda'(X_i^{-1})}.}
$$


- Set $e_{j_i}=E_i$, all other error coordinates to zero, and output $c=y-e$. Verify that all $r$ root checks vanish and that the correction has weight at most $T$. Recover the message from the unconstrained transform coordinates by $m_a=n^{-1}\widehat c_{b-1-a}$, or from the last $k$ coefficients if [systematic encoding](../../../../../systematic-encoding.md) was used.

The denominator in the [Forney algorithm](../../../../../forney-algorithm.md) is nonzero for distinct locations. The [minimum-distance error-detection and correction guarantee](../../../../../minimum-distance-error-detection-and-correction-guarantee.md) gives unique recovery because $d=n-k+1>2T$. If the required locator or a valid correction cannot be found, declare decoding failure. Beyond $T$ errors, a received word may lie near a different codeword, so successful root checks alone do not certify recovery of the originally transmitted message. **The guaranteed correction radius is $\lfloor(n-k)/2\rfloor$ symbol errors.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 87](../../paper-87-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
