<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In the printed phased [Bell basis](../../../../../bell-basis.md), the actions on its four kets are

$$
\begin{array}{c|ccc}
 &\sigma_A^x&\sigma_A^y&\sigma_A^z\\\hline
|1\rangle&i|2\rangle&-i|3\rangle&i|4\rangle\\
|2\rangle&-i|1\rangle&-i|4\rangle&-i|3\rangle\\
|3\rangle&-i|4\rangle&i|1\rangle&i|2\rangle\\
|4\rangle&i|3\rangle&i|2\rangle&-i|1\rangle
\end{array}
$$

Each [matrix](../../../../../matrix.md) is purely imaginary and antisymmetric. Let $T$ have these four basis kets as columns in the computational basis. The [infinitesimal generators](../../../../../infinitesimal-generator-stochastic-processes.md) of the standard rotation $U_A=\exp[-i\theta\,\mathbf n\cdot\boldsymbol\sigma_A/2]$ are

$$
G_a=-\frac i2T^\dagger(\sigma_a\otimes I)T.
$$

Using the displayed actions gives the phase-convention-specific identities

$$
\boxed{G_x=-L_x^-,\qquad G_y=L_y^-,\qquad G_z=-L_z^-.}
$$

They are real [antisymmetric matrices](../../../../../skew-symmetric-matrix.md). A finite $SU(2)$ rotation on $A$ therefore acts on the magic-basis coefficient vector as $b\mapsto Ob$, with $O\in SO(4)$. Consequently

$$
q'=(Ob)^{\mathsf T}(Ob)=b^{\mathsf T}O^{\mathsf T}Ob=b^{\mathsf T}b=q.
$$

It preserves [concurrence](../../../../../concurrence.md) and hence **preserves the reduced [eigenvalues](../../../../../eigenvalue.md) and [entanglement entropy](../../../../../entanglement-entropy.md)**. A general $U(2)$ operation adds a common [phase](../../../../../phase-waves.md) to $b$; that changes $q$ by a [phase](../../../../../phase-waves.md) of twice the angle but leaves $|q|$ unchanged. The real-rotation description of local transformations is a characteristic property of the [magic basis](../../../../../magic-basis.md).[After Eq.(6), real magic-basis matrices and independent local transformations](../../../../../entanglement-of-a-pair-of-quantum-bits-by-scott-hill-and-william-k-wootters.md)

As an independent direct check, a local unitary sends $\rho_A$ to $U_A\rho_AU_A^\dagger$, which is a unitary similarity transformation and cannot change its [spectrum](../../../../../spectrum-functional-analysis.md). This [local-unitary invariance of entanglement entropy](../../../../../local-unitary-invariance-of-entanglement-entropy.md) also explains why merely rotating one subsystem cannot create [entanglement](../../../../../entangled-state.md).

## ↑ Ancestors (15)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
