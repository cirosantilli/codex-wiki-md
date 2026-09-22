<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the physical [velocity potential](../../../../../../velocity-potential.md) by $\psi=\sqrt n\exp(im\phi/\hbar)$, so the [superfluid velocity](../../../../../../superfluid-velocity.md) is $\mathbf v=\nabla\phi$. The [condensate number current](../../../../../../condensate-number-current.md) is

$$
\mathbf j=\frac\hbar m\operatorname{Im}(\psi^*\nabla\psi)=n\nabla\phi.
$$

Multiplying the pumped [Gross–Pitaevskii equation](../../../../../../gross-pitaevskii-equation.md) by $\psi^*$ and subtracting its [complex conjugate](../../../../../../complex-conjugate.md) gives the density equation. Equivalently, substituting the amplitude and phase and equating imaginary parts yields

$$
\boxed{n_t+\nabla\cdot(n\nabla\phi)=\frac2\hbar(\gamma-\Gamma n)n}.
$$

Equating real parts gives the other [gain-loss Madelung equations](../../../../../../gain-loss-madelung-equations.md) relation,

$$
\boxed{m\phi_t+\frac m2|\nabla\phi|^2+V_0n
-\frac{\hbar^2}{2m}\frac{\nabla^2\sqrt n}{\sqrt n}=0}.
$$

The last term is the [quantum potential](../../../../../../quantum-potential.md), retained wherever $n>0$. Taking a [gradient](../../../../../../gradient.md) gives the equivalent velocity equation

$$
 m[\mathbf v_t+(\mathbf v\cdot\nabla)\mathbf v]
=-\nabla\left(V_0n-\frac{\hbar^2}{2m}\frac{\nabla^2\sqrt n}{\sqrt n}\right)
$$

in an irrotational region. In equilibrium $n_t=0$ and $\phi(\mathbf x,t)=\Phi(\mathbf x)-\mu t/m$, so

$$
\boxed{\nabla\cdot(n\nabla\Phi)=\frac{2n}{\hbar}(\gamma-\Gamma n)},\qquad
\mu=\frac m2|\nabla\Phi|^2+V_0n-
\frac{\hbar^2}{2m}\frac{\nabla^2\sqrt n}{\sqrt n}.
$$

This convention distinguishes the physical [velocity potential](../../../../../../velocity-potential.md) from the dimensionless [quantum phase](../../../../../../quantum-phase.md) $m\phi/\hbar$; using the latter instead would change the divergence prefactor.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
