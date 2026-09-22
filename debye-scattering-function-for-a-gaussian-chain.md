# Debye scattering function for a Gaussian chain

↑ **Parent:** [Gaussian chain](gaussian-chain.md)

A continuum [Gaussian chain](gaussian-chain.md) has separation [characteristic function](characteristic-function.md) $e^{-a|s-t|}$, $a=k^2b^2/6$. Integrating over a contour of length $N$ gives the [polymer scattering function](polymer-scattering-function.md)

$$
g(k)=\frac2N\int_0^N(N-s)e^{-as}\,ds=N\mathcal D(x),\qquad x=aN=k^2R_g^2,
$$

where $R_g^2=Nb^2/6$ in this continuum convention and $\mathcal D(x)=2(e^{-x}-1+x)/x^2$, with continuous value $\mathcal D(0)=1$. Its limits are $\mathcal D(x)=1-x/3+x^2/12+\cdots$ and $\mathcal D(x)\sim2/x$ for large $x$.

For a discrete chain with $N$ sites, retain the self terms and let $z=e^{-k^2b^2/6}$. The exact finite expression is $g_N=1+(2/N)\sum_{\ell=1}^{N-1}(N-\ell)z^\ell=(1+z)/(1-z)-2z(1-z^N)/[N(1-z)^2]$, with $g_N(0)=N$. Taking $N\to\infty$ while $x=Nk^2b^2/6$ stays fixed gives $g_N/N\to\mathcal D(x)$. The continuum expression describes the coil scaling range, whereas the discrete expression tends to one as $kb\to\infty$.

## ↑ Ancestors (6)

1. [Gaussian chain](gaussian-chain.md)
2. [Biopolymer mechanics](biopolymer-mechanics.md)
3. [Mathematical biology](mathematical-biology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-75/3/solution.md)
