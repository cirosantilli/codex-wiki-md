<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a grid sequence define its [semidiscrete Fourier transform](../../../../semidiscrete-fourier-transform.md) in the dimensionless frequency variable $\theta\in[-\pi,\pi]$ by

$$
\widehat W(\theta)=\sum_{j\in\mathbb Z}W_je^{-ij\theta},\qquad
W_j=\frac1{2\pi}\int_{-\pi}^{\pi}\widehat W(\theta)e^{ij\theta}d\theta.
$$

For general square-summable data the transform is interpreted as an limit in the [L2 norm](../../../../l2-norm.md), rather than an [absolutely convergent](../../../../absolute-convergence.md) pointwise sum. The [Parseval identity](../../../../parseval-identity.md) in this normalization is

$$
\|W\|_{\ell_2}^2=\Delta x\sum_{j\in\mathbb Z}|W_j|^2
=\frac{\Delta x}{2\pi}\int_{-\pi}^{\pi}|\widehat W(\theta)|^2d\theta.
$$

The [Fourier symbols](../../../../fourier-symbol-of-a-difference-operator.md) of $D_x^0$ and $D_x^+D_x^-$ are $i\sin\theta/\Delta x$ and $-4\sin^2(\theta/2)/(\Delta x)^2$. Transforming the implicit equation gives

$$
\left(1+4a\mu\sin^2(\theta/2)+i\nu\sin\theta\right)\widehat U^{m+1}=\widehat U^m.
$$

Its [amplification factor](../../../../amplification-factor.md) is consequently

$$
G_I(\theta)=\frac1{1+4a\mu\sin^2(\theta/2)+i\nu\sin\theta}.
$$

The denominator has real part at least one because $a\geq0$. It never vanishes, so multiplication by $G_I$ defines a unique next value in the [l2 sequence space](../../../../l2-sequence-space.md), and

$$
|G_I(\theta)|^2=\frac1{(1+4a\mu\sin^2(\theta/2))^2+\nu^2\sin^2\theta}\leq1.
$$

The [Parseval identity](../../../../parseval-identity.md) now gives

$$
\boxed{\|U^{m+1}\|_{\ell_2}\leq\|U^m\|_{\ell_2}\leq\|U^0\|_{\ell_2}\quad\text{for every }m\geq0,\ \Delta x,\Delta t>0.}
$$

This is unconditional [practical stability of a finite difference scheme](../../../../practical-stability-of-a-finite-difference-scheme.md): in the course's terminology the numerical evolution does not increase this [norm](../../../../norm.md). Linearity gives the same estimate for perturbations of the initial data. This contraction convention is stronger than a finite-time mesh-uniform bound allowing physical exponential growth.[Archived Oxford NSDE I Lecture 12, PDF page 2, definition of practical stability as non-growth of the discrete norm](https://www.numerical.rl.ac.uk/media/people/tyrone-rees/nsde/notes/Lecture12.pdf)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical solutions of partial differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solutions of partial differential equations course of the University of Oxford](../../../../numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
