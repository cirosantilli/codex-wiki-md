# Lacunary scaling-phase regularity counterexample

↑ **Parent:** [Periodic phase change of a scaling function](periodic-phase-change-of-a-scaling-function.md)

Let

$$
\theta(t)=\sum_{n\ge0}2^{-n}\sin(2^nt),\qquad a(t)=e^{i\theta(t)}.
$$

The [Fourier coefficients](fourier-coefficient.md) of $\theta$ are absolutely summable, so $a$ belongs to the [Wiener algebra](wiener-algebra.md), as does $a^{-1}$. The identity $\theta(2t)=\theta(t)+\theta(t+\pi)$ implies $a(2t)=a(t)a(t+\pi)$. Starting with a compactly supported [Daubechies wavelet](daubechies-wavelet.md) having $p\ge3$ [vanishing moments](vanishing-moment.md), the [periodic phase change of a scaling function](periodic-phase-change-of-a-scaling-function.md) gives $m(t)=a(t+\pi)m_0(t)$, while the canonical high-pass construction leaves $\widehat\psi(2t)=e^{-it}\overline{m_0(t+\pi)}\widehat\varphi_0(t)$ unchanged.

At a dyadic point $t_0=2\pi k/2^j$, the terms of the [difference quotient](difference-quotient.md) with $n\ge j$ and $2^n|h|\le1$ each contribute $1+O((2^nh)^2)$. Their number tends to infinity, their total error is bounded, and the remaining tail contributes a bounded amount. Hence $(\theta(t_0+h)-\theta(t_0))/h=\log_2(1/|h|)+O(1)$, so neither $\theta$ nor $a$ has a finite [derivative](derivative.md) there. These points are [dense](dense-set.md). Away from the isolated zero of $m_0$ near $\pi$, multiplication by its nonzero [smooth](smooth-function.md) value cannot remove this nondifferentiability. Thus the new [MRA low-pass filter](low-pass-filter-of-a-multiresolution-analysis.md) is not [differentiable](differentiable-function.md) throughout any neighborhood of $\pi$, despite integrability of the [scaling function](scaling-function.md) and unchanged [vanishing moments](vanishing-moment.md). Ordinary higher [derivatives](derivative.md) at $\pi$ cannot be inferred, although the corresponding [Peano zero](peano-zero.md) survives.

## ↑ Ancestors (9)

1. [Periodic phase change of a scaling function](periodic-phase-change-of-a-scaling-function.md)
2. [Scaling function](scaling-function.md)
3. [Multiresolution analysis](multiresolution-analysis.md)
4. [Wavelet](wavelet.md)
5. [Fourier analysis](fourier-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/1/d/solution.md)
