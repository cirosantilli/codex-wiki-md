<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Linearize the averaged rule about the genuine positive-eigenvalue [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) $w_i=v_i/\sqrt\alpha$, where $v_i$ is a unit [eigenvector](../../../../../../eigenvector.md). The question's unit-length hint implicitly uses $\alpha=1$; for general $\alpha$ the scaling is required. Put $w=w_i+u$ and $u_i=v_i^Tu$. To first order,

$$
w^TCw=\frac{\lambda_i}{\alpha}+\frac{2\lambda_i}{\sqrt\alpha}u_i+O(\|u\|^2).
$$

Substituting into the mean learning equation and cancelling the equilibrium terms gives [stability and normalization of averaged Oja learning](../../../../../../stability-and-normalization-of-averaged-oja-learning.md):

$$
\boxed{\tau\dot u=(C-\lambda_iI)u-2\lambda_i u_iv_i+O(\|u\|^2).}
$$

In the eigenbasis, the radial and transverse perturbations satisfy

$$
\tau\dot u_i=-2\lambda_i u_i,\qquad
\tau\dot u_j=(\lambda_j-\lambda_i)u_j\quad(j\ne i).
$$

For $\lambda_i>0$, the radial direction contracts. Any nonmaximal eigenvector has a transverse direction with $\lambda_j>\lambda_i$ and is unstable. If $\lambda_1>\lambda_2$ and $\lambda_1>0$, both $\pm v_1/\sqrt\alpha$ have strictly negative linearized [eigenvalues](../../../../../../eigenvalue.md) and are [locally asymptotically stable](../../../../../../asymptotic-stability.md). Thus **only the maximal-eigenvalue directions can be stable**, with the usual simple-eigenvalue assumptions giving isolated attracting equilibria.

Convergence also needs an initial component along the top direction. For the full averaged equation, the coefficients $b_j=v_j^Tw$ obey

$$
\tau\dot b_j=[\lambda_j-\alpha(w^TCw)]b_j.
$$

For $b_1(0)\ne0$,

$$
\boxed{\frac{b_j(t)}{b_1(t)}=\frac{b_j(0)}{b_1(0)}
 e^{(\lambda_j-\lambda_1)t/\tau}.}
$$

With a strict top eigenvalue, all other ratios tend to zero. The norm equation from part a then drives the nonzero weight norm to $1/\sqrt\alpha$, so the weight converges to the top eigenvector with the sign of its initial top component. Random nonzero initialization has that component with probability one under a continuous distribution.

Several exceptions qualify the printed conclusion. A repeated largest eigenvalue gives neutral directions within the top eigenspace and convergence to a normalized vector in that space, not a unique eigenvector. An initial vector exactly orthogonal to the top eigenspace remains in that invariant subspace. The zero initialization stays zero. If $C=0$, every weight is stationary and no distinguished component can be learned. Nonzero nullspace equilibria are unstable when $C$ has a positive eigenvalue. Hence unconditional convergence from every initial weight, or uniqueness without a spectral gap, would be false.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
