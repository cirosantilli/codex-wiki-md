<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use signature $(+---)$, the positive spatial metric $\gamma_{ij}$, and a future-directed unit normal $n_\mu=(N,0)$, so $n^\mu=N^{-1}(1,-N^i)$. This fixes the sign of the normal to agree with the specified $\Pi$. The negative normal covector printed in the source would instead give $-\Pi$; its orientation and the displayed derivative cannot both be retained. Use the operational negative-expansion convention for the [extrinsic curvature of a spatial hypersurface](../../../../../../extrinsic-curvature-of-a-spatial-hypersurface.md), $K_{ij}=-(\dot\gamma_{ij}-D_iN_j-D_jN_i)/(2N)$, which is the convention giving the requested expanding-universe sign. With this future normal and signature it equals $n_{i;j}$; the source's $-n_{i;j}$ identity instead uses its past-pointing normal.

For the [scalar-field matter projections](../../../../../../scalar-field-matter-projections.md), put $s_i=D_i\phi$ and $s^2=\gamma^{ij}s_is_j$. Decomposing the scalar gradient into normal and tangent parts gives $\partial_\mu\phi\partial^\mu\phi=\Pi^2-s^2$. Contracting the [Klein-Gordon scalar stress-energy tensor](../../../../../../klein-gordon-scalar-stress-energy-tensor.md) with the normal and the [spatial projection tensor](../../../../../../spatial-projection-tensor.md) therefore yields

$$
\boxed{\rho=\frac12\Pi^2+\frac12s^2+V,\qquad J_i=-\Pi s_i,\qquad
S_{ij}=s_is_j+\gamma_{ij}\left[\frac12(\Pi^2-s^2)-V\right].}
$$

In particular, the positive spatial metric raises the $i,j$ indices in $s^2$; raising them with the four-metric would reverse that spatial sign. These quantities are the [energy density](../../../../../../energy-density.md), momentum density and spatial stress in the normal frame.

For the homogeneous [Spatially flat FLRW metric](../../../../../../spatially-flat-flrw-metric.md), $N_i=0$, $\gamma_{ij}=a^2\delta_{ij}$ and $s_i=0$. Consequently $\Pi=\dot{\bar\phi}/\bar N$, $J_i=0$, $\bar\rho=\Pi^2/2+V$, $\bar P=\Pi^2/2-V$, and

$$
K_{ij}=-\frac{a\dot a}{\bar N}\delta_{ij},\qquad
\boxed{K^i{}_j=-H\delta^i{}_j,\quad K=-3H,\quad H=\frac{\dot a}{\bar Na}.}
$$

The intrinsic [Ricci scalar](../../../../../../ricci-scalar.md) is zero and $K^2-K_{ij}K^{ij}=9H^2-3H^2=6H^2$. The [Hamiltonian constraint](../../../../../../hamiltonian-constraint.md) thus gives **the scalar-field [Friedmann equation](../../../../../../friedmann-equations.md)**:

$$
\boxed{H^2=\frac{8\pi G}{3}\left(\frac{\dot{\bar\phi}^{2}}{2\bar N^2}+V(\bar\phi)\right).}
$$

The [momentum constraint](../../../../../../momentum-constraint.md) is identically satisfied, since its homogeneous spatial derivatives and $J_i$ vanish. The scalar equation reduces to $\bar N^{-1}\dot\Pi+3H\Pi+V_{,\phi}=0$. Substituting $\Pi$ and multiplying by $\bar N^2$ gives **the background [inflaton equation of motion](../../../../../../inflaton-equation-of-motion.md)**:

$$
\boxed{\ddot{\bar\phi}+\left(3H\bar N-\frac{\dot{\bar N}}{\bar N}\right)\dot{\bar\phi}+\bar N^2V_{,\phi}=0.}
$$

No derivation of the supplied gravitational constraints is needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
