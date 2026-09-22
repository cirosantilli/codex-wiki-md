# Fourier inversion theorem

↑ **Parent:** [Fourier analysis](fourier-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fourier_inversion_theorem)

The [Fourier inversion theorem](fourier-inversion-theorem.md) makes decomposition into [frequencies](frequency.md) reversible: a complete [Fourier transform](fourier-transform-split.md), including its [wave phases](phase-waves.md), determines the original [function](function-split.md) up to equality [almost everywhere](almost-everywhere.md). With the angular-frequency convention

$$
\widehat f(\xi)=\int_{\mathbb R^n}e^{-ix\cdot\xi}f(x)\,dx,
$$

if $f$ and $\widehat f$ belong to the [L1 space](l1-space.md), then

$$
f(x)=\frac1{(2\pi)^n}\int_{\mathbb R^n}e^{ix\cdot\xi}\widehat f(\xi)d\xi
$$

[almost everywhere](almost-everywhere.md). The right side is a continuous representative of $f$. If $f$ itself is continuous, equality holds everywhere, as explained by the [continuous version of Fourier inversion](continuous-version-of-fourier-inversion.md). The integrability hypotheses ensure that both displayed [integrals](integral-split.md) are ordinary absolutely convergent [integrals](integral-split.md). For arbitrary elements of the [L2 space](l2-space-is-a-hilbert-space.md), the [Plancherel theorem](plancherel-theorem.md) instead supplies inversion in the [L2 space](l2-space-is-a-hilbert-space.md) norm.

Each factor $e^{ix\cdot\xi}$ is a [Fourier mode](fourier-mode.md); the inverse [integral](integral-split.md) adds them with the complex weights $\widehat f(\xi)/(2\pi)^n$. The normalization is part of the recipe. In one dimension, writing ordinary [frequency](frequency.md) as $\nu=\xi/(2\pi)$ gives the equivalent pair

$$
F(\nu)=\int_{\mathbb R}f(t)e^{-2\pi i\nu t}\,dt,\qquad f(t)=\int_{\mathbb R}F(\nu)e^{2\pi i\nu t}\,d\nu,
$$

where $F(\nu)=\widehat f(2\pi\nu)$. Reversing both exponential signs gives another equivalent convention, but the forward and inverse formulas must use opposite signs consistently.

For example, the [Fourier transform of a Gaussian](fourier-transform-of-a-gaussian.md) gives

$$
f(x)=e^{-ax^2},\qquad \widehat f(\xi)=\sqrt{\frac\pi a}\,e^{-\xi^2/(4a)},\qquad a>0.
$$

[Fourier inversion](fourier-inversion-theorem.md) says that a weighted continuum of [oscillations](oscillation.md) reconstructs this smooth [Gaussian function](gaussian-function.md). Narrowing the original [Gaussian function](gaussian-function.md) by increasing $a$ broadens its [frequency spectrum](frequency-spectrum.md). This is a concrete demonstration that a sharply localized shape needs a wider range of [frequencies](frequency.md).

Inversion is what makes a [frequency](frequency.md) calculation useful: transform a [function](function-split.md), solve the simpler problem there, then return to the original variables. A brief proof outline is to multiply $\widehat f(\xi)$ by $e^{-\epsilon|\xi|^2}$, $\epsilon>0$. The inverse [integral](integral-split.md) becomes [convolution](convolution.md) with a normalized [Gaussian function](gaussian-function.md), an [approximate identity](approximate-identity.md). As $\epsilon$ tends to zero, [dominated convergence](dominated-convergence-theorem.md) gives the unregularized inverse [integral](integral-split.md), while the [approximate identity](approximate-identity.md) recovers $f$ [almost everywhere](almost-everywhere.md). Joseph Fourier's _Théorie analytique de la chaleur_ (1822), Chapter IX, article 417, contains a cosine double-integral representation antecedent to this modern formula; the hypotheses above are the modern statement.[Fourier 1822, Chapter IX, article 417: cosine integral representation](https://fr.wikisource.org/wiki/Th%C3%A9orie_analytique_de_la_chaleur/Chapitre_9)

**Table of contents**

- [Continuous version of Fourier inversion](continuous-version-of-fourier-inversion.md)
- [Fourier transform of a derivative](fourier-transform-of-a-derivative.md)
- [Inverse Fourier transforms of phase factors](inverse-fourier-transforms-of-phase-factors.md)
- [Translation property of the Fourier transform](translation-property-of-the-fourier-transform.md)

## ↑ Ancestors (5)

1. [Fourier analysis](fourier-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (40)

- [Filtered backprojection](filtered-backprojection.md)
- [Fourier analysis](fourier-analysis-split.md)
- [Fourier cosine transform](fourier-cosine-transform.md)
- [Fourier-cutoff recovery of expectations from a characteristic function](fourier-cutoff-recovery-of-expectations-from-a-characteristic-function.md)
- [Fourier inversion theorem](fourier-inversion-theorem.md)
- [Fourier representation of a smooth Selberg weight](fourier-representation-of-a-smooth-selberg-weight.md)
- [Inverse Fourier transform](inverse-fourier-transform.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-86/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/14d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-9/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/14e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-23/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-60/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-8/1/vii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/20f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/26k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/33c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/23i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-327/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-3/3a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/33e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/26g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-117/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1/1a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/14a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/27k/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/27k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/23f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-129/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/4/a/solution.md)
- [Pólya–Vinogradov inequality](polya-vinogradov-inequality.md)
- [Sampling expansion by periodic Fourier projection](sampling-expansion-by-periodic-fourier-projection.md)
- [Self-convolution of a bilateral exponential](self-convolution-of-a-bilateral-exponential.md)
