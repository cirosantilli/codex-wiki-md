# Fourier transform of a periodic distribution

↑ **Parent:** [Fourier transform of a tempered distribution](fourier-transform-of-a-tempered-distribution.md)

For a $2\pi$ [periodic distribution](periodic-distribution.md) $u\in\mathcal S'(\mathbb R)$, choose a [smooth periodic partition of unity](smooth-periodic-partition-of-unity.md) $\Psi$, and define $c_n=(2\pi)^{-1}\langle u,\Psi e^{-inx}\rangle$. A finite [Schwartz seminorm](schwartz-seminorm.md) bound on the fixed [compact support](compact-support.md) gives $|c_n|\leq C(1+|n|)^N$. For a [Schwartz function](schwartz-function.md) $\phi$, the [Poisson summation formula](poisson-summation-formula.md) and [Fourier inversion](fourier-inversion-theorem.md) imply $P\widehat\phi(x)=\sum_n\phi(-n)e^{inx}$. Localizing the pairing for $u$ gives

$$
\langle\widehat u,\phi\rangle=\langle u,\Psi P\widehat\phi\rangle=2\pi\sum_n c_n\phi(n),
$$

proving the displayed [Fourier transform](fourier-transform-split.md) formula. The series converges in [tempered distributions](tempered-distribution.md) because its coefficients have [polynomial growth](polynomial-growth.md) while $\phi(n)$ decreases rapidly. Applying the [inverse Fourier transform](inverse-fourier-transform.md) gives $u=\sum_n c_ne^{inx}$ in [tempered distributions](tempered-distribution.md). These are the [smooth-window Fourier coefficients of a periodic distribution](smooth-window-fourier-coefficients-of-a-periodic-distribution.md), and the transform formula shows independence of $\Psi$.

## ↑ Ancestors (8)

1. [Fourier transform of a tempered distribution](fourier-transform-of-a-tempered-distribution.md)
2. [Tempered distribution](tempered-distribution.md)
3. [Schwartz space](schwartz-space.md)
4. [Fourier analysis](fourier-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-condensed-matter-physics-course-of-the-university-of-oxford/2019/1/c/solution.md)
- [Solution](past-exam-of-the-fourier-analysis-course-of-the-university-of-oxford/2023/3/a/iv/solution.md)
