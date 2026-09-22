<h1 id="a1/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Project the first-order equation onto $\Psi_j^{(0)}$, with $j\ne i$. By [orthonormality](../../../../../../orthonormal-set.md) and the [Hermitian operator](../../../../../../hermitian-operator.md) property,

$$
\begin{aligned}
\langle\Psi_j^{(0)}|(\hat H^{(0)}-E_i^{(0)})|\Psi_i^{(1)}\rangle
&=(E_j^{(0)}-E_i^{(0)})c_{ij},\\
\langle\Psi_j^{(0)}|(\hat H^{(1)}-E_i^{(1)})|\Psi_i^{(0)}\rangle
&=H_{ji}.
\end{aligned}
$$

Consequently

$$
\boxed{c_{ij}=\frac{H_{ji}}{E_i^{(0)}-E_j^{(0)}}
=\frac{H_{ij}^*}{E_i^{(0)}-E_j^{(0)}}\qquad(j\ne i),}
$$

and

$$
\boxed{\Psi_i^{(1)}=\sum_{j\ne i}
\frac{\langle\Psi_j^{(0)}|\hat H^{(1)}|\Psi_i^{(0)}\rangle}
{E_i^{(0)}-E_j^{(0)}}\Psi_j^{(0)}.}
$$

The numerator order is important: the question defines $H_{ij}$ with $i$ on the bra, whereas projecting the correction onto state $j$ gives $H_{ji}$. The two coincide only when the relevant [matrix element](../../../../../../matrix-element.md) is real.

Excluding an $i$ component chooses $\langle\Psi_i^{(0)}|\Psi_i^{(1)}\rangle=0$, a permitted first-order phase and [wavefunction normalization](../../../../../../wavefunction-normalization.md) convention. A component parallel to $\Psi_i^{(0)}$ is not determined by the projected equation. Nondegeneracy ensures nonzero denominators; a small [energy](../../../../../../energy-split.md) gap can still make the perturbative expansion inaccurate unless $|\lambda H_{ji}|\ll|E_i^{(0)}-E_j^{(0)}|$.

## ↑ Ancestors (14)

1. [V](../v.md)
2. [B](../../b.md)
3. [A1](../../../a1.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the chemistry A course of the University of Cambridge](../../../../../split.md)
7. [Chemistry A course of the University of Cambridge](../../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
