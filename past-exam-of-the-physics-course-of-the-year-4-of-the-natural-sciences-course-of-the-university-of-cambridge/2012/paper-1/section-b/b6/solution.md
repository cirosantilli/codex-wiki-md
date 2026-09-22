<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

For the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator-split.md), using $[\hat x,\hat p]=i\hbar$, direct multiplication gives

$$
\hat a^\dagger\hat a=\frac{\hat p^2}{2m\hbar\omega}+\frac{m\omega\hat x^2}{2\hbar}-\frac12,
\qquad
\boxed{\hat H=(\hat a^\dagger\hat a+\tfrac12)\hbar\omega.}
$$

The [commutators](../../../../../commutator.md) are

$$
\boxed{[\hat a,\hat a^\dagger]=1,\quad
[\hat H,\hat a]=-\hbar\omega\hat a,\quad
[\hat H,\hat a^\dagger]=\hbar\omega\hat a^\dagger.}
$$

Thus each ladder operation shifts [energy](../../../../../energy-split.md) by one quantum. The [ladder operator](../../../../../ladder-operator.md) norms $\|a|n\rangle\|^2=n$ and $\|a^\dagger|n\rangle\|^2=n+1$, with conventional [phases](../../../../../phase-waves.md), give

$$
\boxed{\hat a|n\rangle=\sqrt n\,|n-1\rangle,\qquad
\hat a^\dagger|n\rangle=\sqrt{n+1}\,|n+1\rangle.}
$$

Let $\ell=\sqrt{\hbar/(m\omega)}$. In position space $\hat p=-i\hbar\partial_x$, so $a\psi_0=0$ becomes $(x+\ell^2\partial_x)\psi_0=0$. Normalizing and then applying $a^\dagger$ gives

$$
\boxed{\psi_0=(\pi\ell^2)^{-1/4}e^{-x^2/(2\ell^2)},\qquad
\psi_1=\sqrt2\frac{x}{\ell}\psi_0.}
$$

Their overlap vanishes because $\psi_0^*\psi_1$ is odd on the full real line; the [Gaussian](../../../../../normal-distribution.md) second moment verifies $\int|\psi_1|^2dx=1$.

<a id="section-b/b6/image-oscillator-ground-and-first-states"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1-gp2012-oscillator.png)

**[Figure 5](#section-b/b6/image-oscillator-ground-and-first-states). Oscillator ground and first states**. Original normalized oscillator wavefunctions show even ground-state parity, odd first-excited parity and one interior node in the excited state.

## ↑ Ancestors (13)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
