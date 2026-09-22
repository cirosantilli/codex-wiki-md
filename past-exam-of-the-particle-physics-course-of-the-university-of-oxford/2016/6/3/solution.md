<h1 id="6/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [Dirac representation of the gamma matrices](../../../../dirac-representation-of-the-gamma-matrices.md) and commuting external-wavefunction components, rather than anticommuting quantum fields. Let $A=\gamma^0\gamma^2$, $B=\gamma^2\gamma^0=-A$, and $\Gamma^\alpha=\gamma^\alpha(g_V-g_A\gamma^5)$. Since $(\gamma^2)^\dagger=-\gamma^2$ and $v=i\gamma^2u^*$,

$$
\bar v_A\Gamma^\alpha v_B=-u_A^TB\Gamma^\alpha\gamma^2u_B^*.
$$

Transpose this scalar and use $(\gamma^2)^T=\gamma^2$, $B^T=A$ and $\bar u_B=u_B^\dagger\gamma^0$:

$$
\bar v_A\Gamma^\alpha v_B=\bar u_B A(\Gamma^\alpha)^TB u_A.
$$

Here $A^2=1$ and $A(\gamma^5)^TA=\gamma^5$. The supplied identity therefore yields

$$
\begin{aligned}
A(\Gamma^\alpha)^TB&=A(g_V-g_A(\gamma^5)^T)(\gamma^\alpha)^TB\\
&=(g_V-g_A\gamma^5)\gamma^\alpha=\gamma^\alpha(g_V+g_A\gamma^5).
\end{aligned}
$$

Hence

$$
\boxed{\bar v_A(\mathbf p)\gamma^\alpha(g_V-g_A\gamma^5)v_B(\mathbf p')=\bar u_B(\mathbf p')\gamma^\alpha(g_V+g_A\gamma^5)u_A(\mathbf p)}.
$$

The external labels and [momenta](../../../../momentum-split.md) are exchanged; the scalar constants are transposed, not complex-conjugated. At the level of these numerical [fermion bilinears](../../../../fermion-bilinear.md), charge conjugation reverses the relative sign of the vector and axial terms, relating particle and [antiparticle](../../../../antiparticle.md) weak amplitudes. For $g_V=g_A$, the two displayed spinor chains have opposite [chiral projectors](../../../../chiral-projector.md). A physical charge-conjugation transformation of an operator current also includes the minus sign from reordering [Dirac fields](../../../../dirac-field.md). In particular this numerical identity does not imply equal electric charges for a particle and its [antiparticle](../../../../antiparticle.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [6](../../6.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
