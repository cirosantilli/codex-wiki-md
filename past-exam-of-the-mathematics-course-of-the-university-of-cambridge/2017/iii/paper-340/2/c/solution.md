<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use localization and cancellation of the assumed [interval-adapted wavelet basis](../../../../../../interval-adapted-wavelet-basis.md): at scale $j$, every detail [wavelet](../../../../../../wavelet.md) has support diameter at most $B2^{-j}$, [L1 norm](../../../../../../l1-norm.md) at most $B'2^{-j/2}$, and annihilates [polynomials](../../../../../../polynomial-split.md) of degree less than $q$. These bounds also apply to the modified [boundary wavelets](../../../../../../boundary-wavelet.md); a restriction of an arbitrary whole-line [wavelet](../../../../../../wavelet.md) without the cancellation-preserving boundary construction would not suffice. The finitely many coarse [scaling functions](../../../../../../scaling-function.md) can be treated separately.

Write $\alpha=r+\beta$ with $0<\beta\le1$ as above. Because $\alpha<q$, we have $r<q$. Choose $x_0$ in the [support of a function](../../../../../../support.md) of $\psi_{j,n}$, and let $T_{x_0}$ be the degree-$r$ [Taylor polynomial](../../../../../../taylor-polynomial.md) of $f$. The [Hölder-Taylor remainder bound](../../../../../../holder-taylor-remainder-bound.md) gives

$$
|f(x)-T_{x_0}(x)|\le C_\alpha\|f\|_{C^\alpha}|x-x_0|^\alpha.
$$

For $r=0$ this is the [Hölder seminorm](../../../../../../holder-seminorm.md) bound. For $r\ge1$, the [integral](../../../../../../integral.md) [Taylor remainder](../../../../../../taylor-remainder.md) is bounded using $f^{(r)}(t)-f^{(r)}(x_0)$, whose magnitude is at most $[f^{(r)}]_{C^{0,\beta}}|t-x_0|^\beta$.

The [vanishing moments](../../../../../../vanishing-moment.md) remove $T_{x_0}$ from the [inner product](../../../../../../inner-product.md). Applying the remainder estimate and the [L1 norm](../../../../../../l1-norm.md) bound on the localized support yields the [wavelet coefficient decay for Hölder functions](../../../../../../wavelet-coefficient-decay-for-holder-functions.md)

$$
|\langle f,\psi_{j,n}\rangle|\le\sup_{\operatorname{supp}\psi_{j,n}}|f-T_{x_0}|\,\|\psi_{j,n}\|_1\le C_\alpha B^\alpha B'\|f\|_{C^\alpha}2^{-j\alpha}2^{-j/2}.
$$

Thus

$$
\boxed{|\langle f,\psi_{j,n}\rangle|\le C2^{-j(\alpha+1/2)}\|f\|_{C^\alpha}.}
$$

Here $C$ depends on the fixed [wavelet](../../../../../../wavelet.md) family, the exponent and boundary construction, but not on $f,j,n$. The proof uses the assumed regularity and moments; it does not identify the minimal [Daubechies wavelet](../../../../../../daubechies-wavelet.md) order with its [differentiability](../../../../../../differentiability.md) order, which need not coincide.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
