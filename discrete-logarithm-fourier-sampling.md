# Discrete-logarithm Fourier sampling

↑ **Parent:** [Hidden subgroup problem](hidden-subgroup-problem.md)

For a [generator of a group](generator-of-a-group.md) $g$ of order $M$ and $x=g^y$, the function $f(a,b)=g^ax^{-b}$ hides the [subgroup](subgroup.md) $\{(yb,b):b\in\mathbb Z_M\}$ of $\mathbb Z_M^2$. Each [fiber](fiber-of-a-function.md) is an affine [coset](coset.md) $\{(yb+k,b):b\in\mathbb Z_M\}$. Measuring the function register gives its normalized [coset state](coset-state.md). Applying the positive-exponent [quantum Fourier transform](quantum-fourier-transform.md) to both input registers gives amplitude

$$
\frac{e^{2\pi ikc_1/M}}{M\sqrt M}\sum_{b=0}^{M-1}e^{2\pi ib(yc_1+c_2)/M}.
$$

The [finite geometric series](finite-geometric-series.md) vanishes off $c_2=-yc_1$ and equals $M$ on that line. Thus each allowed output pair has [probability](probability.md) $1/M$, independently of the coset offset. If $\gcd(c_1,M)=1$, a [modular inverse](modular-multiplicative-inverse.md) recovers $y=-c_2c_1^{-1}$.

**Table of contents**

- [Linear congruence from a discrete-logarithm Fourier sample](linear-congruence-from-a-discrete-logarithm-fourier-sample.md)

## ↑ Ancestors (6)

1. [Hidden subgroup problem](hidden-subgroup-problem.md)
2. [Quantum Fourier transform](quantum-fourier-transform.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Modular exponentiation](modular-exponentiation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/1/b/iii/solution.md)
