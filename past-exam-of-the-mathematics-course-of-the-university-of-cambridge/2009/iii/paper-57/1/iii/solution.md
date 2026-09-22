<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $a_\mu=n^\nu\nabla_\nu n_\mu$ be the [normal acceleration](../../../../../../normal-acceleration.md). It is tangential by normalization. Resolving the derivative's first index into normal and tangential parts gives

$$
\nabla_\mu n_\nu=K_{\mu\nu}-n_\mu a_\nu,\qquad\nabla_\mu n^\mu=K.
$$

The [extrinsic curvature](../../../../../../extrinsic-curvature.md) is symmetric because the normal is hypersurface orthogonal: locally $n_\mu=-N\partial_\mu t$, and the antisymmetric derivative of $n$ vanishes after projecting both indices tangentially.

Apply the supplied Ricci commutator to $n^\nu$ and project its free index. With the positive-expansion convention it gives

$$
\begin{aligned}
P^\mu{}_\alpha R_{\mu\lambda}n^\lambda
&=P^\mu{}_\alpha[\nabla_\nu(K_\mu{}^\nu-n_\mu a^\nu)-\nabla_\mu K]\\
&=P^\mu{}_\alpha\nabla_\nu K^\nu{}_\mu-K_{\alpha\nu}a^\nu-D_\alpha K.
\end{aligned}
$$

To identify the first two terms, expand the fully projected divergence:

$$
D_\beta K^\beta{}_\alpha
=P^\mu{}_\alpha P^\rho{}_\lambda\nabla_\rho K^\lambda{}_\mu
=P^\mu{}_\alpha\nabla_\lambda K^\lambda{}_\mu
+n^\rho n_\lambda P^\mu{}_\alpha\nabla_\rho K^\lambda{}_\mu.
$$

Tangency gives $n_\lambda K^\lambda{}_\mu=0$. Differentiating it shows that the last term is $-P^\mu{}_\alpha K^\lambda{}_\mu n^\rho\nabla_\rho n_\lambda=-K_{\alpha\lambda}a^\lambda$. Substituting into the commutator proves the [contracted Codazzi equation with positive expansion](../../../../../../contracted-codazzi-equation-with-positive-expansion.md):

$$
\boxed{D_\beta K^\beta{}_\alpha-D_\alpha K=P^\mu{}_\alpha R_{\mu\nu}n^\nu.}
$$

No assumption of geodesic normals was needed; the acceleration terms cancel rather than being discarded.

The metric-trace term in the [Einstein field equations](../../../../../../einstein-field-equations.md) drops out of a tangential-normal projection, since $P^\mu{}_\alpha g_{\mu\nu}n^\nu=0$. Define the normal-frame momentum density $j_\alpha=-P^\mu{}_\alpha T_{\mu\nu}n^\nu$. The equation becomes

$$
D_\beta K^\beta{}_\alpha-D_\alpha K=-8\pi G j_\alpha.
$$

Thus **Codazzi supplies the [momentum constraint](../../../../../../momentum-constraint.md)** on each spatial slice. In flat homogeneous FRW, $K^i{}_j=H\delta^i{}_j$ and $H$ has no spatial gradient, so its left side vanishes. A comoving homogeneous [perfect fluid](../../../../../../perfect-fluid.md) likewise has $j_i=0$. The background satisfies the constraint automatically; the Friedmann expansion law is instead obtained from the normal-normal constraint.

Suitable scalar variables are lapse and shift potentials $A,B$, spatial curvature and scalar shear potentials $\psi,E$, and a matter momentum potential $J$ with $j_i=\partial_iJ$. For example, choose

$$
ds^2=a^2\left[-(1+2A)d\tau^2+2\partial_iB\,d\tau dx^i+((1-2\psi)\delta_{ij}+2\partial_i\partial_jE)dx^idx^j\right].
$$

A [density contrast](../../../../../../density-contrast.md) and pressure perturbation can be added for the remaining scalar matter equations. With this positive-shift convention, the linear extrinsic-curvature perturbation is

$$
\delta K^i{}_j=\frac1a[-(\psi'+\mathcal HA)\delta^i{}_j+\partial^i\partial_j(E'-B)].
$$

Its scalar shear cancels out of the momentum-constraint combination, leaving

$$
\boxed{\frac2a\partial_i(\psi'+\mathcal HA)=-8\pi G\partial_iJ.}
$$

These are the [scalar momentum constraint with positive extrinsic curvature](../../../../../../scalar-momentum-constraint-with-positive-extrinsic-curvature.md) variables; a specified gauge can then remove two of the four scalar metric potentials.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
