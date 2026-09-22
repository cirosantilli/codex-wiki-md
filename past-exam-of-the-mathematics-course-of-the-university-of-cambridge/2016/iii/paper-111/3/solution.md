<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the following normalization for [Fourier analysis on a finite group](../../../../../fourier-analysis-on-a-finite-group.md). Choose one [unitary irreducible representation](../../../../../unitary-irreducible-representation.md) $\rho:G\to U(d_\rho)$ from each equivalence class, including the [trivial representation](../../../../../trivial-representation.md). For a scalar function $f:G\to\mathbb C$, put

$$
\widehat f(\rho)=\mathbb E_x f(x)\rho(x),
\qquad
\langle f,g\rangle=\mathbb E_x\overline{f(x)}g(x).
$$

This convention uses $\rho(x)$, rather than $\rho(x)^*$, in the [Fourier transform on a finite group](../../../../../fourier-transform-on-a-finite-group.md); it makes the [normalized convolution on a finite group](../../../../../normalized-convolution-on-a-finite-group.md) preserve multiplication order.

The needed [representation theory](../../../../../representation-theory-split.md) consists of [Maschke's theorem](../../../../../maschke-s-theorem.md) and [unitarization of a finite-group representation](../../../../../unitarization-of-a-finite-group-representation.md), together with the [Schur orthogonality relations](../../../../../schur-orthogonality-relations.md):

$$
\mathbb E_x\rho(x)_{ij}\overline{\sigma(x)_{kl}}
=\begin{cases}d_\rho^{-1}\delta_{ik}\delta_{jl},&\rho=\sigma,\\0,&\rho\ne\sigma.\end{cases}
$$

The [regular representation](../../../../../regular-representation.md) contains $d_\rho$ copies of each $\rho$, so $\sum_\rho d_\rho^2=|G|$. Thus the scaled [matrix coefficients](../../../../../matrix-coefficient.md) $\sqrt{d_\rho}\rho(x)_{ij}$, and also their [complex conjugates](../../../../../complex-conjugate.md), form an [orthonormal basis](../../../../../orthonormal-basis.md) of all scalar functions on $G$. These facts imply [Fourier inversion on a finite group](../../../../../fourier-inversion-on-a-finite-group.md) and the [Parseval identity on a finite group](../../../../../parseval-identity-on-a-finite-group.md) in the forms

$$
f(x)=\sum_\rho d_\rho\operatorname{tr}\bigl(\widehat f(\rho)\rho(x)^*\bigr),
\qquad
\langle f,g\rangle
=\sum_\rho d_\rho\operatorname{tr}\bigl(\widehat f(\rho)^*\widehat g(\rho)\bigr),
$$

and hence

$$
\|f\|_2^2=\sum_\rho d_\rho\|\widehat f(\rho)\|_{\mathrm{HS}}^2.
$$

In particular, the transform is an isomorphism onto the direct sum of the [matrix algebras](../../../../../matrix-algebra.md) $M_{d_\rho}(\mathbb C)$, with the displayed weighted [Hilbert-Schmidt inner product](../../../../../hilbert-schmidt-inner-product.md).

Define the [normalized convolution on a finite group](../../../../../normalized-convolution-on-a-finite-group.md) by

$$
(f*g)(x)=\mathbb E_yf(y)g(y^{-1}x).
$$

Substituting $x=yz$ and using the [group representation](../../../../../group-representation.md) identity yields the [convolution theorem on a finite group](../../../../../convolution-theorem-on-a-finite-group.md)

$$
\widehat{f*g}(\rho)=\widehat f(\rho)\widehat g(\rho).
$$

Unlike [normalized convolution on a finite group](../../../../../normalized-convolution-on-a-finite-group.md) on an [abelian group](../../../../../abelian-group.md), this product need not commute. If $\widetilde f(x)=\overline{f(x^{-1})}$, then $\widehat{\widetilde f}(\rho)=\widehat f(\rho)^*$. For [left translation of a group function](../../../../../left-translation-of-a-group-function.md) and [right translation of a group function](../../../../../right-translation-of-a-group-function.md) $L_af(x)=f(a^{-1}x)$ and $R_af(x)=f(xa)$,

$$
\widehat{L_af}(\rho)=\rho(a)\widehat f(\rho),
\qquad
\widehat{R_af}(\rho)=\widehat f(\rho)\rho(a)^*.
$$

For an [abelian group](../../../../../abelian-group.md), every [irreducible representation](../../../../../irreducible-representation.md) is one-dimensional; this reduces to [Fourier analysis on a finite abelian group](../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md) with characters relabelled by their inverses. These formulas establish the basic scalar theory, with all normalizations and multiplication orders fixed.

Now suppose every nontrivial [irreducible representation](../../../../../irreducible-representation.md) has $d_\rho\geq m$. If $f$ is a [mean-zero function](../../../../../mean-zero-function.md), its component at the [trivial representation](../../../../../trivial-representation.md) is zero. The [Parseval identity on a finite group](../../../../../parseval-identity-on-a-finite-group.md) gives, for each other $\rho$,

$$
\|\widehat f(\rho)\|_{\mathrm{op}}
\leq\|\widehat f(\rho)\|_{\mathrm{HS}}
\leq\frac{\|f\|_2}{\sqrt{d_\rho}}
\leq\frac{\|f\|_2}{\sqrt m}.
$$

Using the [convolution theorem on a finite group](../../../../../convolution-theorem-on-a-finite-group.md), the [Hilbert-Schmidt norm](../../../../../hilbert-schmidt-norm.md) inequality $\|AB\|_{\mathrm{HS}}\leq\|A\|_{\mathrm{op}}\|B\|_{\mathrm{HS}}$, and the [Parseval identity on a finite group](../../../../../parseval-identity-on-a-finite-group.md) once more gives the [product mixing in a quasirandom group](../../../../../product-mixing-in-a-quasirandom-group.md) estimate

$$
\boxed{\|f*g\|_2\leq m^{-1/2}\|f\|_2\|g\|_2\quad\text{when }\mathbb E f=0.}
$$

Write $a,b,c$ for the [subset density](../../../../../density-of-a-finite-subset.md) values of $A,B,C$, respectively, and let $f=1_A-a$, $g=1_B-b$ be [balanced subset indicators](../../../../../balanced-indicator-function-of-a-finite-subset.md). Since both are [mean-zero functions](../../../../../mean-zero-function.md), $1_A*1_B=ab+f*g$. Their squared [norms](../../../../../norm.md) are $a(1-a)$ and $b(1-b)$. Also $\mathbb E(f*g)=0$, so the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) yields

$$
\begin{aligned}
\left|\mathbb E_z(1_A*1_B)(z)1_C(z)-abc\right|
&=\left|\mathbb E_z(f*g)(z)(1_C(z)-c)\right|\\
&\leq\sqrt{\frac{a(1-a)b(1-b)c(1-c)}m}
\leq\sqrt{\frac{abc}{m}}.
\end{aligned}
$$

If $abc>1/m$, the final bound is strictly smaller than $abc$. Thus the normalized number of pairs $(x,y)\in A\times B$ with $xy\in C$ is positive. Equivalently,

$$
\boxed{|A||B||C|>|G|^3/m\ \Longrightarrow\ AB\cap C\ne\varnothing.}
$$

This is the desired conclusion for a [quasirandom group](../../../../../quasirandom-group.md); the strict inequality ensures positivity rather than merely a nonnegative lower bound.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 111](../../paper-111-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
