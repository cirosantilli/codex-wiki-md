# Logarithmic cusp with slow trigonometric approximation

↑ **Parent:** [Inverse theorem for trigonometric approximation](inverse-theorem-for-trigonometric-approximation.md)

Define $h(x)=|x|\log(e\pi/|x|)$ on $[-\pi,\pi]$, set $h(0)=0$, and extend periodically. Concavity and monotonicity on $[0,\pi]$ give $\omega(h,\delta)=\delta\log(e\pi/\delta)$ for $0<\delta\le\pi$. Its cosine [Fourier coefficients](fourier-coefficient.md) are

$$
a_j=-\frac{2}{\pi j^2}\int_0^{j\pi}\frac{1-\cos u}{u}\,du
=-\frac{2\log j}{\pi j^2}+O(j^{-2}),\qquad j\ge1.
$$

One [integration by parts](integration-by-parts.md) gives the formula; the remaining integral is $\log j+O(1)$ by the [Dirichlet test](dirichlet-test.md). All these coefficients are nonpositive. The [de la Vallée Poussin sum](de-la-vallee-poussin-sum.md) $V_n=2\sigma_{2n}-\sigma_n$ reproduces degree-at-most-$n$ [trigonometric polynomials](trigonometric-polynomial.md) and has [operator norm](operator-norm.md) at most three. Hence $L_n(f)=f(0)-V_nf(0)$ has norm at most four and annihilates those polynomials. Its weights on coefficients are zero up to $n$, nonnegative thereafter, and one from $2n$ onwards, so $|L_n(h)|\ge\sum_{j\ge2n}|a_j|\gtrsim\log n/n$. Thus $E_n(h)\ge|L_n(h)|/4\gtrsim\log n/n$; the [first Jackson theorem for periodic approximation](first-jackson-theorem-for-periodic-approximation.md) proves the matching upper bound. This cusp and the [critical Weierstrass modulus](critical-weierstrass-modulus.md) have the same first-modulus order but different best-approximation rates.

## ↑ Ancestors (6)

1. [Inverse theorem for trigonometric approximation](inverse-theorem-for-trigonometric-approximation.md)
2. [Uniform approximation](uniform-approximation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69/6/c/solution.md)
