<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $Q$ be the [orthogonal matrix](../../../../orthogonal-matrix.md) taking old components to new ones, so $x'_i=Q_{ip}x_p$. With repeated indices summed, the [tensor component transformation law](../../../../tensor-component-transformation-law.md) is

$$
\boxed{t'_{ij}=Q_{ip}Q_{jq}t_{pq},\qquad u'_{ijkl}=Q_{ip}Q_{jq}Q_{kr}Q_{ls}u_{pqrs}.}
$$

An [isotropic tensor](../../../../isotropic-tensor.md) has the same components after every proper [rotation](../../../../rotation-mathematics.md). Since $Q_{ip}Q_{jp}=\delta_{ij}$, the [Kronecker delta](../../../../kronecker-delta.md) is invariant. Applying this identity to each factor shows that $a\delta_{ij}$ and every linear combination $b\delta_{ij}\delta_{kl}+c\delta_{ik}\delta_{jl}+d\delta_{il}\delta_{jk}$ are invariant as well.

To show that an [isotropic second-rank tensor](../../../../isotropic-second-rank-tensor.md) must be scalar, start with any matrix $t$, without assuming symmetry. Invariance under quarter-turns about axes 1 and 2 implies invariance under their squares, the half-turns

$$
Q_1^2=\operatorname{diag}(1,-1,-1),\qquad Q_2^2=\operatorname{diag}(-1,1,-1).
$$

The first forces $t_{12},t_{21},t_{13},t_{31}$ to vanish. The second also forces $t_{23},t_{32}$ to vanish. The matrix is therefore diagonal. A quarter-turn about axis 1 interchanges its 22 and 33 entries; one about axis 2 interchanges its 11 and 33 entries. All three must agree, giving $t=aI$.

A [rotation](../../../../rotation-mathematics.md) preserves the ball $V_R$, $|x|^2$ and the [volume element](../../../../volume-element.md). Changing integration variables by that rotation shows that $A$ and $B$ are [isotropic tensors](../../../../isotropic-tensor.md). Write $A_{ij}=a\delta_{ij}$. Taking its [tensor contraction](../../../../tensor-contraction.md) gives

$$
3a=A_{ii}=\int_{V_R}|x|^4dV=4\pi\int_0^Rr^6dr=\frac{4\pi R^7}{7},
$$

so $a=4\pi R^7/21$. Every permutation of the indices of $B$ leaves its integrand unchanged. Its complete symmetry therefore makes all three isotropic coefficients equal, say $d$:

$$
B_{ijkl}=d(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).
$$

Double contraction gives $15d=B_{iikk}=\int_{V_R}|x|^4dV=4\pi R^7/7$. Thus the [isotropic fourth moment of a ball](../../../../isotropic-fourth-moment-of-a-ball.md) and its radial contraction are

$$
\boxed{A_{ij}=\frac{4\pi R^7}{21}\delta_{ij},\qquad
B_{ijkl}=\frac{4\pi R^7}{105}(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).}
$$

Put $d=4\pi R^7/105$, so that $a=5d$. Contract $B$ with the prescribed [unit vector](../../../../unit-vector.md) twice:

$$
C_{ij}=A_{ij}+B_{ijkl}n_kn_l=d(6\delta_{ij}+2n_in_j).
$$

This has the [spectrum of a scalar matrix plus a rank-one projector](../../../../spectrum-of-a-scalar-matrix-plus-a-rank-one-projector.md). In the direction $n$, the [outer product](../../../../outer-product.md) $nn^T$ acts as the identity; on the plane perpendicular to $n$, it acts as zero. Therefore

$$
\boxed{Cn=\frac{32\pi R^7}{105}n,\qquad Cv=\frac{8\pi R^7}{35}v\quad\text{for }v\cdot n=0.}
$$

Any nonzero multiple of $n$ is a parallel [eigenvector](../../../../eigenvector.md), and any nonzero vector in the perpendicular plane is a transverse [eigenvector](../../../../eigenvector.md). The transverse [eigenvalue](../../../../eigenvalue.md) has multiplicity two; an [orthonormal basis](../../../../orthonormal-basis.md) of that plane completes a set of principal axes.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
