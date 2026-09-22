# Fourier-cutoff recovery of expectations from a characteristic function

↑ **Parent:** [Uniqueness theorem for characteristic functions](uniqueness-theorem-for-characteristic-functions.md)

Let $f$ be compactly supported and continuous, let $g,\widehat g\in L^1(\mathbb R)$, and use $\widehat g(t)=\int g(x)e^{itx}\,dx$. If $g(0)\ne0$, then

$$
\mathbb E[f(Z)]
=\lim_{\varepsilon\downarrow0}
\frac1{2\pi g(0)}
\int_{\mathbb R}g(\varepsilon s)\widehat f(-s)\varphi_Z(s)\,ds.
$$

This follows by [Fubini's theorem](fubini-s-theorem.md), a change of variables, [Fourier inversion theorem](fourier-inversion-theorem.md), and [dominated convergence theorem](dominated-convergence-theorem.md). It gives a direct proof of the [uniqueness theorem for characteristic functions](uniqueness-theorem-for-characteristic-functions.md) because the right side depends only on $\varphi_Z$.

## ↑ Ancestors (7)

1. [Uniqueness theorem for characteristic functions](uniqueness-theorem-for-characteristic-functions.md)
2. [Characteristic function](characteristic-function.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/26k/b/solution.md)
