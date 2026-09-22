<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Angle integration gives a dual representation in any lattice dimension. Discrete summation by parts rewrites the phase as

$$
\sum_{x,\mu}n_{x,\mu}(\theta_{x+\hat\mu}-\theta_x)
=-\sum_x\theta_x\sum_\mu(n_{x,\mu}-n_{x-\hat\mu,\mu}).
$$

Each normalized angle integral is a Kronecker delta. This proves the [integer-current representation of the Villain model](../../../../../../integer-current-representation-of-the-villain-model.md)

$$
Z_V=(2\pi\beta)^{-N_b/2}\sum_{\operatorname{div}n=0}\exp\left[-\frac1{2\beta}\sum_en_e^2\right].
$$

The PDF does not specify dimension or boundaries. The point-vortex [vortex Coulomb gas](../../../../../../vortex-coulomb-gas.md) interpretation below is two-dimensional. In three dimensions the defects are [vortex](../../../../../../phase-vortex.md) lines, and the dual constrained-current representation still holds but is not a gas of point charges with logarithmic interactions.

First take a connected simply connected planar lattice, with free outer angles, so no torus winding sectors are silently discarded. Assign an integer height $\ell$ to each dual face, fixing the exterior face height to zero. A divergence-free integer current is exactly the oriented height difference on the two faces adjoining its bond. To see existence, integrate the rotated current along a dual path: the change around a closed dual path is the total divergence inside, hence zero. Integer currents give integer heights, and fixing the exterior removes their constant-shift ambiguity. Therefore

$$
\sum_en_e^2=\sum_{\langle x,y\rangle_{\rm dual}}(\ell_x-\ell_y)^2=\ell^TL\ell,
$$

where $L$ is the positive dual [Graph Laplacian](../../../../../../laplacian-matrix.md) with the exterior height fixed. This gives the [dual integer-height representation of the planar Villain model](../../../../../../dual-integer-height-representation-of-the-planar-villain-model.md).

Apply the supplied [Poisson summation formula](../../../../../../poisson-summation-formula.md) separately to every interior height. For $N_f$ interior faces,

$$
Z_V=(2\pi\beta)^{-N_b/2}\sum_{q\in\mathbb Z^{N_f}}
\int_{\mathbb R^{N_f}}d\phi\,
\exp\left[-\frac1{2\beta}\phi^TL\phi+2\pi i q^T\phi\right].
$$

Complete the Gaussian square, or use its [characteristic function](../../../../../../characteristic-function.md), to evaluate the integral as

$$
\frac{(2\pi\beta)^{N_f/2}}{\sqrt{\det L}}\exp[-2\pi^2\beta q^TL^{-1}q].
$$

Thus the smooth fluctuations and integer defects separate:

$$
\boxed{Z_V=Z_{\rm sw}Z_{\rm v},\qquad
Z_{\rm v}=\sum_{q\in\mathbb Z^{N_f}}e^{-2\pi^2\beta q^TGq},\quad G=L^{-1}.}
$$

The Gaussian factor is $Z_{\rm sw}=(2\pi\beta)^{-(N_b-N_f)/2}/\sqrt{\det L}$. It really is the [spin wave](../../../../../../spin-wave.md) factor of the original lattice: the planar Euler identity gives $N_b-N_f=N_x-1$, and the [matrix-tree theorem](../../../../../../kirchhoff-s-theorem.md) identifies $\det L$ with the spanning-tree count of the original graph. Its reduced primal [Laplacian](../../../../../../laplacian.md) has the same determinant, so the noncompact Gaussian angle integral with one angle fixed has exactly this prefactor. The compact common-angle mode has been normalized to one. The remaining $q$ variables are integer [vortex](../../../../../../phase-vortex.md) windings on the faces, giving the [vortex Coulomb gas](../../../../../../vortex-coulomb-gas.md).

For periodic boundaries, $L$ has a zero mode, and there are also two noncontractible current sectors. Neutral charges use the inverse $G$ on the mean-zero subspace. An integer dual height may have twists $w_x,w_y\in\mathbb Z$ across periods $L_x,L_y$. Subtracting $w_xx/L_x+w_yy/L_y$ makes the remaining height periodic; the [gradient](../../../../../../gradient.md) energy gains $(L_yw_x^2/L_x+L_xw_y^2/L_y)/(2\beta)$. Its height [Poisson summation](../../../../../../poisson-summation-formula.md) supplies the phase $\exp[2\pi i(w_xP_x/L_x+w_yP_y/L_y)]$, where $P_x=\sum q_xx$ and $P_y=\sum q_xy$. A second [Poisson summation](../../../../../../poisson-summation-formula.md) in $w_x,w_y$ yields the positive [harmonic-sector factor in periodic Villain duality](../../../../../../harmonic-sector-factor-in-periodic-villain-duality.md)

$$
\mathcal W(q)=\sum_{W_x,W_y\in\mathbb Z}\exp\left[-2\pi^2\beta\left\{
\frac{L_x}{L_y}\left(W_x-\frac{P_x}{L_x}\right)^2+
\frac{L_y}{L_x}\left(W_y-\frac{P_y}{L_y}\right)^2\right\}\right].
$$

Up to charge-independent normalization, the exact periodic result is $Z_V=Z_{\rm sw}\sum_{\sum q=0}e^{-2\pi^2\beta q^TGq}\mathcal W(q)$. Smooth [spin waves](../../../../../../spin-wave.md) still factor out, but the finite-volume global winding sectors couple to [vortex](../../../../../../phase-vortex.md) dipole moments. The familiar neutral bulk formula suppresses this boundary information; it must not be asserted as an exact finite-torus formula without specifying those sectors.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
