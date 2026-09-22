<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a uniform material and an affine static base deformation, the [deformation gradient](../../../../../../deformation-gradient.md), [incremental elastic moduli](../../../../../../incremental-elastic-moduli.md) and reference [mass density](../../../../../../density.md) are constant. With zero incremental [body force](../../../../../../body-force.md), the equation reduces to $c_{\alpha i\beta j}v_{j,\beta\alpha}=\rho_0\ddot v_i$. Let $\nu$ be a unit material propagation direction, $m$ a constant polarization and $s=t-\nu_\alpha\xi_\alpha/c$. Direct differentiation of the [plane wave](../../../../../../plane-wave.md) gives

$$
v_i=m_if(s),\qquad \ddot v_i=m_if''(s),\qquad v_{j,\beta\alpha}=\frac{\nu_\alpha\nu_\beta}{c^2}m_jf''(s).
$$

Thus every twice differentiable profile $f$ satisfies the incremental equation if

$$
\boxed{Q_{ij}(\nu)m_j=\rho_0c^2m_i,\qquad Q_{ij}(\nu)=c_{\alpha i\beta j}\nu_\alpha\nu_\beta.}
$$

This is the [acoustic tensor](../../../../../../acoustic-tensor.md) [eigenvalue](../../../../../../eigenvalue.md) problem. The [acoustic tensor](../../../../../../acoustic-tensor.md) is a real [symmetric matrix](../../../../../../symmetric-matrix.md): interchange the index pairs in the [incremental elastic moduli](../../../../../../incremental-elastic-moduli.md) and then interchange the dummy material indices to obtain $Q_{ji}=Q_{ij}$. Its [eigenvectors](../../../../../../eigenvector.md) give the displacement polarizations. A positive [eigenvalue](../../../../../../eigenvalue.md) gives a real nonzero speed $c$; arbitrary-profile propagation imposes precisely this algebraic condition. Boundary conditions determine which combinations of these local [plane waves](../../../../../../plane-wave.md) are allowed in a finite body.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
