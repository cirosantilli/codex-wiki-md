<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use periodic [plane waves](../../../../plane-wave.md) on the ring. For $n\in\mathbb Z$,

$$
\phi_n(x)=\frac{e^{inx/a}}{\sqrt{2\pi a}},\qquad H\phi_n=\frac{\hbar^2n^2}{2ma^2}\phi_n.
$$

They are [orthonormal](../../../../orthonormal-set.md) on one circumference and [complete](../../../../completeness.md) by [Fourier series](../../../../fourier-series-split.md). Thus $\boxed{E_k=\hbar^2k^2/(2ma^2)}$, with [degeneracy](../../../../degenerate-energy-levels.md) $\boxed{1\text{ for }k=0,\quad2\text{ for }k\geq1}$: the two signs of nonzero [angular momentum](../../../../angular-momentum.md) have the same energy. Equivalently one may use [normalized](../../../../normalization.md) sine and cosine [eigenfunctions](../../../../eigenfunction.md) for each positive $k$.

For the position measurement put $\theta=x/a$. Direct integration gives

$$
\boxed{\mathbb P(\tfrac12\pi a\leq x\leq\tfrac32\pi a)=\frac1\pi\int_{\pi/2}^{3\pi/2}\sin^2(\theta/2)\,d\theta=\frac12+\frac1\pi.}
$$

The energy measurement requires projection onto whole degenerate [eigenspaces](../../../../eigenspace.md), rather than just onto one traveling wave. The expansion coefficients are

$$
c_n=\langle\phi_n,\psi\rangle=\frac1{\pi\sqrt2}\int_0^{2\pi}\sin(\theta/2)e^{-in\theta}\,d\theta=\frac{2\sqrt2}{\pi(1-4n^2)}.
$$

For instance the imaginary integral vanishes by reflection about $\theta=\pi$, and the product-to-sum identity evaluates the real integral as $4/(1-4n^2)$. Consequently

$$
\boxed{p_0=\frac8{\pi^2},\qquad p_k=|c_k|^2+|c_{-k}|^2=\frac{16}{\pi^2(4k^2-1)^2}\quad(k\geq1).}
$$

Every numerator is positive and no integer $k$ makes a denominator zero, so every energy has nonzero [probability](../../../../probability.md). [Parseval's identity](../../../../parseval-identity.md) guarantees that these probabilities sum to one. The supplied state is a valid [normalized](../../../../normalization.md) periodic $L^2$ state; its derivative need not obey the operator-domain periodic condition for the spectral probabilities to be defined.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
