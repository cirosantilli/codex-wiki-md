<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Adopt the usual [orthogonal tight-binding approximation](../../../../orthogonal-tight-binding-approximation.md), so the three localized spatial states are orthonormal. Each site has two neighbors, with the same real hopping [matrix element](../../../../matrix-element.md). For coefficients $c_n$, the Schrödinger equation at site $n$ is

$$
(E-E_0)c_n=t(c_{n-1}+c_{n+1}),\qquad c_{n+3}=c_n.
$$

The constant-coefficient state has $c_1=c_2=c_3$, giving [energy](../../../../energy-split.md) $E_0+2t$. Its normalization therefore yields

$$
\boxed{|\psi_g\rangle=\frac{|1\rangle+|2\rangle+|3\rangle}{\sqrt3},\qquad E_g=E_0+2t.}
$$

To verify that it is the [ground state](../../../../ground-state.md), the three discrete ring momenta are $\theta=0,\pm2\pi/3$, with $c_n\propto e^{i\theta(n-1)}$ and energies $E_0+2t\cos\theta$. The other two states both have [energy](../../../../energy-split.md) $E_0-t$. Since $t<0$, $E_0+2t<E_0-t$ and the gap is $3|t|$. This is the [three-site tight-binding ring](../../../../three-site-tight-binding-ring.md) spectrum.

The spatial [ground state](../../../../ground-state.md) is unique and has equal probability $1/3$ on every site; its common overall phase is arbitrary. [Spin](../../../../spin.md) would supply a separate twofold degeneracy when no spin-dependent terms are included, but does not change the requested spatial state. If the localized functions were instead nonorthogonal raw atomic orbitals, their overlap matrix would be additional data needed for normalization and a [generalized eigenvalue problem](../../../../generalized-eigenvalue-problem.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
