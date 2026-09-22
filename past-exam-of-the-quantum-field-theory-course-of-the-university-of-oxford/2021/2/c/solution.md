<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take a spatial [Fourier transform](../../../../fourier-transform-split.md) of the [mode expansion of a Dirac field](../../../../mode-expansion-of-a-dirac-field.md):

$$
\widetilde\psi(t,\mathbf p)=\int d^3x\,e^{-i\mathbf p\cdot\mathbf x}\psi(t,\mathbf x)
=\frac1{\sqrt{2E}}\sum_r
\left[b_{-\mathbf p}^{r\dagger}v^r(-\mathbf p)e^{iEt}
+a_{\mathbf p}^ru^r(\mathbf p)e^{-iEt}\right].
$$

The [orthogonality](../../../../orthogonal-vectors.md) relations $u^{s\dagger}(\mathbf p)u^r(\mathbf p)=2E\delta^{sr}$ and $u^{s\dagger}(\mathbf p)v^r(-\mathbf p)=0$ isolate the [fermionic annihilation operator](../../../../fermionic-annihilation-operator.md). Projecting onto $v^s(-\mathbf p)$ instead isolates the [fermionic creation operator](../../../../fermionic-creation-operator.md):

$$
\boxed{\begin{aligned}
a_{\mathbf p}^s&=\frac{e^{iEt}}{\sqrt{2E}}u^{s\dagger}(\mathbf p)
\int d^3x\,e^{-i\mathbf p\cdot\mathbf x}\psi(t,\mathbf x),\\
b_{-\mathbf p}^{s\dagger}&=\frac{e^{-iEt}}{\sqrt{2E}}v^{s\dagger}(-\mathbf p)
\int d^3x\,e^{-i\mathbf p\cdot\mathbf x}\psi(t,\mathbf x).
\end{aligned}}
$$

The opposite time phases and reversed antiparticle [momentum](../../../../momentum-split.md) are essential. Both denominators are $\sqrt{2E}$, because the [Dirac spinors](../../../../dirac-spinor.md) have norm squared $2E$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
