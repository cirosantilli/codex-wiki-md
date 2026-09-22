<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

For a [Cartesian second-rank tensor](../../../../../cartesian-second-rank-tensor.md), write

$$
P_{ij}=\frac12(P_{ij}+P_{ji})+\frac12(P_{ij}-P_{ji}).
$$

The first term is a [symmetric second-rank tensor](../../../../../symmetric-second-rank-tensor.md) and the second is an [antisymmetric second-rank tensor](../../../../../antisymmetric-second-rank-tensor.md). Taking the [trace](../../../../../matrix-trace.md) of the symmetric term and subtracting it gives the [scalar, symmetric-traceless and axial tensor decomposition](../../../../../scalar-symmetric-traceless-and-axial-tensor-decomposition.md):

$$
\boxed{P=\frac13P_{kk},\qquad S_{ij}=\frac12(P_{ij}+P_{ji})-\frac13P_{kk}\delta_{ij},\qquad A_k=\frac12\epsilon_{kij}P_{ij}.}
$$

Here $S_{ij}=S_{ji}$ and $S_{ii}=0$. To check reconstruction of the antisymmetric part, contract the [Levi-Civita symbols](../../../../../levi-civita-symbol.md):

$$
\epsilon_{ijk}A_k=\frac12\epsilon_{ijk}\epsilon_{klm}P_{lm}=\frac12(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})P_{lm}=\frac12(P_{ij}-P_{ji}).
$$

Thus $P_{ij}=P\delta_{ij}+S_{ij}+\epsilon_{ijk}A_k$, and the displayed contractions also prove uniqueness. The vector associated with the antisymmetric part is an [axial vector](../../../../../pseudovector.md) under reflections, and an ordinary vector under proper rotations.

For the specified [isotropic tensor](../../../../../isotropic-tensor.md) law, contract the [Kronecker deltas](../../../../../kronecker-delta.md) first:

$$
P_{ij}=\alpha\delta_{ij}T_{kk}+\beta T_{ij}+\gamma T_{ji}.
$$

Write $T_{ij}=T\delta_{ij}+W_{ij}+\epsilon_{ijk}V_k$, where $T=T_{kk}/3$ and $W$ is symmetric and traceless. Transposition preserves its scalar and symmetric-traceless parts and reverses its antisymmetric part. Therefore

$$
P_{ij}=(3\alpha+\beta+\gamma)T\delta_{ij}+(\beta+\gamma)W_{ij}+(\beta-\gamma)\epsilon_{ijk}V_k.
$$

Uniqueness of the decomposition gives the [isotropic elasticity on tensor components](../../../../../isotropic-elasticity-on-tensor-components.md) relations. Provided their respective coefficients are nonzero, the requested inverses are

$$
\boxed{T=\frac{P}{3\alpha+\beta+\gamma},\qquad W_{ij}=\frac{S_{ij}}{\beta+\gamma},\qquad V_k=\frac{A_k}{\beta-\gamma}.}
$$

If one coefficient vanishes, that strain component has zero stress response: the corresponding stress component must be zero for a solution to exist, and that strain component is not uniquely recoverable. Isotropy by itself does not guarantee invertibility.

If $T_{ij}$ is symmetric then $V=0$, hence $A=0$ and the stress is symmetric. Equivalently, direct transposition gives $P_{ij}-P_{ji}=(\beta-\gamma)(T_{ij}-T_{ji})=0$. Restricting to this symmetric-strain case gives

$$
\boxed{P_{ij}=\lambda\delta_{ij}T_{kk}+\mu T_{ij},\qquad\lambda=\alpha,\quad\mu=\beta+\gamma.}
$$

This final two-parameter expression uses the symmetry assumption from the preceding request. For a general nonsymmetric array, the transpose term cannot be absorbed into the same coefficient: it acts with $\beta+\gamma$ on the symmetric-traceless part and with $\beta-\gamma$ on the antisymmetric part. The stated coefficient $\mu$ is the coefficient of $T_{ij}$ itself; if one instead writes the conventional elastic law with $2\mu$ multiplying the strain, that shear-modulus convention is half this coefficient.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
