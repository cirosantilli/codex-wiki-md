<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Use the unitary normalization of the [Fourier transform](../../../../../fourier-transform.md),

$$
\mathcal Ff(\xi)=(2\pi)^{-n/2}\int_{\mathbb R^n}e^{-ix\cdot\xi}f(x)\,dx,\qquad
\mathcal Gg(x)=(2\pi)^{-n/2}\int_{\mathbb R^n}e^{ix\cdot\xi}g(\xi)\,d\xi.
$$

The [Schwartz space](../../../../../schwartz-space.md) $\mathcal S(\mathbb R^n)$ consists of [smooth function](../../../../../smooth-function.md)s for which every [Schwartz seminorm](../../../../../schwartz-seminorm.md) $\sup_x|x^\alpha\partial^\beta f(x)|$ is finite. Such functions and all their [derivatives](../../../../../derivative.md) are integrable. Differentiating under the integral and integrating by parts give

$$
\partial_\xi^\alpha\mathcal Ff=(-i)^{|\alpha|}\mathcal F(x^\alpha f),\qquad
\xi^\beta\mathcal Ff=(-i)^{|\beta|}\mathcal F(\partial^\beta f).
$$

Consequently

$$
\sup_\xi|\xi^\beta\partial_\xi^\alpha\mathcal Ff(\xi)|
\leq(2\pi)^{-n/2}\|\partial^\beta(x^\alpha f)\|_1.
$$

Expand the [derivative](../../../../../derivative.md) by the product rule and insert the integrable weight $(1+|x|)^{-n-1}$; the right side is bounded by finitely many Schwartz seminorms of $f$. This proves continuity $\mathcal F:\mathcal S\to\mathcal S$. The identical argument with the opposite sign proves continuity of $\mathcal G$.

For [surjectivity](../../../../../surjective-function.md) and [injectivity](../../../../../injective-function.md) an inversion proof is needed. If $f\in\mathcal S$, multiply $\mathcal Ff(\xi)$ by $e^{-\varepsilon|\xi|^2/2}$. [Fubini's theorem](../../../../../fubini-s-theorem.md) and the elementary [Gaussian integral](../../../../../gaussian-integral.md) give

$$
\mathcal G\bigl(e^{-\varepsilon|\xi|^2/2}\mathcal Ff\bigr)(x)
=\int_{\mathbb R^n}f(y)\rho_\varepsilon(x-y)\,dy,
\qquad
\rho_\varepsilon(x)=(2\pi\varepsilon)^{-n/2}e^{-|x|^2/(2\varepsilon)}.
$$

The Gaussian has total integral one and its mass outside any fixed ball tends to zero. The right side therefore tends to $f(x)$, by uniform continuity of $f$. On the left, $\mathcal Ff\in\mathcal S\subset L^1$, so dominated convergence gives $\mathcal G\mathcal Ff(x)$. This proves $\mathcal G\mathcal F=I$. Reversing the signs in the same calculation proves $\mathcal F\mathcal G=I$. Thus

$$
\boxed{\mathcal F:\mathcal S(\mathbb R^n)\longrightarrow\mathcal S(\mathbb R^n)\text{ is a continuous bijection, with inverse }\mathcal G.}
$$

Its inverse is continuous by the seminorm estimate already proved. This establishes the requested bijection without assuming [Fourier inversion](../../../../../fourier-inversion-theorem.md) as an unexplained theorem.

Inversion gives $\mathcal F^2f(x)=f(-x)$ and the [Parseval identity](../../../../../parseval-identity.md). Indeed, inserting the integral for $\mathcal Ff$ into $\int\mathcal Ff\,\overline{\mathcal Fg}$ and using $f,\mathcal Fg\in L^1$ gives $\int f\overline g$. Density of [Schwartz functions](../../../../../schwartz-function.md) in $L^2$ extends $\mathcal F$ to a [unitary operator](../../../../../unitary-operator.md) on $L^2$, the [Plancherel theorem](../../../../../plancherel-theorem.md). Translation of $f$ becomes multiplication by a phase, modulation becomes frequency translation, and

$$
\mathcal F(f*g)=(2\pi)^{n/2}(\mathcal Ff)(\mathcal Fg),\qquad
\mathcal F(\partial_jf)=i\xi_j\mathcal Ff.
$$

These formulas explain why the [Fourier transform](../../../../../fourier-transform.md) diagonalizes constant-coefficient differential operators. By transpose it also defines a bijection of the [tempered distributions](../../../../../tempered-distribution.md): with the complex-linear distributional pairing, $\langle\mathcal FT,\phi\rangle=\langle T,\mathcal F\phi\rangle$, since the Fourier [kernel](../../../../../kernel-of-a-linear-map.md) is symmetric in its variables.

The connection with [creation and annihilation operators](../../../../../creation-and-annihilation-operators.md) is especially transparent for the [harmonic oscillator](../../../../../simple-harmonic-motion.md). On the common invariant dense domain $\mathcal S$, set

$$
a_j=\frac{x_j+\partial_j}{\sqrt2},\qquad
 a_j^\dagger=\frac{x_j-\partial_j}{\sqrt2}.
$$

[Integration by parts](../../../../../integration-by-parts.md) shows that these are formal Hilbert-space adjoints. They are closable unbounded operators; [commutators](../../../../../commutator.md) below are computed on $\mathcal S$, avoiding undefined products on arbitrary $L^2$ [vectors](../../../../../vector.md). The identity $[\partial_j,x_k]=\delta_{jk}I$ gives the [canonical commutation relations](../../../../../canonical-commutation-relation.md)

$$
[a_j,a_k^\dagger]=\delta_{jk}I,\qquad[a_j,a_k]=[a_j^\dagger,a_k^\dagger]=0.
$$

It also gives

$$
H=-\Delta+|x|^2=2\sum_j a_j^\dagger a_j+nI.
$$

The normalized vacuum $h_0(x)=\pi^{-n/4}e^{-|x|^2/2}$ satisfies $a_jh_0=0$. Define the [Hermite functions](../../../../../hermite-function.md)

$$
h_\alpha=\frac{(a_1^\dagger)^{\alpha_1}\cdots(a_n^\dagger)^{\alpha_n}}{\sqrt{\alpha_1!\cdots\alpha_n!}}h_0.
$$

Moving [annihilation operators](../../../../../annihilation-operator.md) past [creation operators](../../../../../creation-operator.md) with the commutation relations proves

$$
a_jh_\alpha=\sqrt{\alpha_j}\,h_{\alpha-e_j},\qquad
 a_j^\dagger h_\alpha=\sqrt{\alpha_j+1}\,h_{\alpha+e_j},\qquad
Hh_\alpha=(2|\alpha|+n)h_\alpha.
$$

These same relations show that the [Hermite functions](../../../../../hermite-function.md) are [orthonormal](../../../../../orthonormal-set.md): unequal occupations are orthogonal [eigenvectors](../../../../../eigenvector.md) of one of the commuting symmetric [number operators](../../../../../number-operator.md) $a_j^\dagger a_j$, and the ladder relations recursively give [norm](../../../../../norm.md) one.

For completeness, let $g\in L^2$ be orthogonal to every $h_\alpha$. The Hermite [polynomials](../../../../../polynomial-split.md) have nonzero leading monomials and triangular lower-degree terms, so these orthogonality relations say that all [polynomial](../../../../../polynomial-split.md) moments of $h(x)=g(x)e^{-|x|^2/2}\in L^1$ vanish. Its Fourier integral extends to an [entire function](../../../../../entire-function.md) of $\zeta\in\mathbb C^n$:

$$
F(\zeta)=\int g(x)e^{-|x|^2/2}e^{-ix\cdot\zeta}\,dx.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), with the Gaussian absorbing every exponential linear weight and every [polynomial](../../../../../polynomial-split.md), justifies differentiation uniformly on compact sets of $\zeta$. Every Taylor coefficient at zero is a vanishing moment, so the [entire function](../../../../../entire-function.md) is zero. Fourier uniqueness on $L^1$ follows here without circularity: if an $L^1$ function has zero [Fourier transform](../../../../../fourier-transform.md), convolving it with $\rho_\varepsilon$ gives zero by the [Gaussian integral](../../../../../gaussian-integral.md) and Fubini, and the approximate-identity limit in $L^1$ gives the original function zero. Thus $h=0$ and $g=0$. The [Hermite functions](../../../../../hermite-function.md) form an [orthonormal basis](../../../../../orthonormal-basis.md) of $L^2$.

Finally, the elementary [Gaussian integral](../../../../../gaussian-integral.md) gives $\mathcal Fh_0=h_0$. The [derivative](../../../../../derivative.md) and multiplication identities above imply

$$
\mathcal F a_j=i a_j\mathcal F,\qquad
\mathcal F a_j^\dagger=-i a_j^\dagger\mathcal F,
$$

where the operators on the right act on the frequency variable. Hence

$$
\boxed{\mathcal Fh_\alpha=(-i)^{|\alpha|}h_\alpha.}
$$

Thus creation and annihilation organize both the oscillator's spectral decomposition and the four possible Fourier [eigenvalues](../../../../../eigenvalue.md). On [Schwartz functions](../../../../../schwartz-function.md) the oscillator powers control weighted [derivatives](../../../../../derivative.md), and Hermite coefficients decay faster than every power of $1+|\alpha|$; conversely this rapid coefficient decay implies all Schwartz seminorms are finite. The Fourier phases preserve this decay, providing another explanation of the Fourier automorphism of [Schwartz space](../../../../../schwartz-space.md).

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
