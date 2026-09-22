<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $B=A^{\mathsf T}A$. Since $\det A>0$, $B$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md). The [spectral theorem](../../../../../spectral-theorem.md) gives a unique [principal square root of a positive semidefinite matrix](../../../../../principal-square-root-of-a-positive-semidefinite-matrix.md)

$$
U=B^{1/2},\qquad R=AU^{-1}.
$$

Then $R^{\mathsf T}R=U^{-1}BU^{-1}=I$ and $\det R=\det A/\det U=1$, so $R$ is a [rotation matrix](../../../../../rotation-matrix.md). Define $V=RUR^{\mathsf T}$. It is a [symmetric matrix](../../../../../symmetric-matrix.md), is positive definite, and satisfies $V^2=AA^{\mathsf T}$. Consequently the [polar decomposition in continuum mechanics](../../../../../polar-decomposition-in-continuum-mechanics.md) is

$$
\boxed{A=RU=VR,\quad U=(A^{\mathsf T}A)^{1/2},\quad V=(AA^{\mathsf T})^{1/2}.}
$$

Here $U$ and $V$ are the [right stretch tensor](../../../../../right-stretch-tensor.md) and [left stretch tensor](../../../../../left-stretch-tensor.md).

For the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md), use both [material isotropy](../../../../../material-isotropy.md) and [material frame indifference](../../../../../material-frame-indifference.md). Their respective transformation laws are

$$
\sigma(AQ)=\sigma(A),\qquad \sigma(QA)=Q\sigma(A)Q^{\mathsf T},\qquad Q\in SO(3).
$$

The first law and $A=VR$ give $\sigma(A)=\sigma(V)$. Combining the two laws gives $\sigma(QVQ^{\mathsf T})=Q\sigma(V)Q^{\mathsf T}$. In a [principal stretch](../../../../../principal-stretch.md) basis, $V=\operatorname{diag}(\lambda_1,\lambda_2,\lambda_3)$. Each half-turn about a coordinate axis leaves $V$ unchanged; its conjugation changes the signs of the corresponding off-diagonal [stress tensor](../../../../../cauchy-stress-tensor.md) entries. Those entries must therefore vanish. If two [principal stretches](../../../../../principal-stretch.md) coincide, rotations within their [eigenspace](../../../../../eigenspace.md) additionally force the [stress tensor](../../../../../cauchy-stress-tensor.md) to be scalar on that [eigenspace](../../../../../eigenspace.md). Thus **the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) and [left stretch tensor](../../../../../left-stretch-tensor.md) have common principal axes**, including at repeated [principal stretches](../../../../../principal-stretch.md). This proves [coaxiality of isotropic elastic stress](../../../../../coaxiality-of-isotropic-elastic-stress.md).

The precise symmetry conclusion is [equivariance of isotropic principal stresses](../../../../../equivariance-of-isotropic-principal-stresses.md). Every permutation of the [principal stretches](../../../../../principal-stretch.md) can be realized by a signed permutation [rotation matrix](../../../../../rotation-matrix.md), so

$$
\sigma_i(\lambda_{\pi(1)},\lambda_{\pi(2)},\lambda_{\pi(3)})
=\sigma_{\pi(i)}(\lambda_1,\lambda_2,\lambda_3)
$$

when the indexing is permuted consistently. Equivalently, permuting the arguments permutes the labelled [principal stresses](../../../../../principal-stress.md) in the same way. In particular, $\sigma_1$ is symmetric in $\lambda_2,\lambda_3$, and analogous statements hold for $\sigma_2,\sigma_3$.

For distinct [principal stretches](../../../../../principal-stretch.md), interpolate the three values $\sigma_i$ at the three points $\lambda_i$:

$$
\sigma=\beta_0I+\beta_1V+\beta_2V^2,\qquad
\sigma_i=\beta_0+\beta_1\lambda_i+\beta_2\lambda_i^2.
$$

Uniqueness of this interpolation implies that the scalar coefficients $\beta_j$ are symmetric functions of the unordered [principal stretches](../../../../../principal-stretch.md); they may be expressed through the elementary symmetric invariants. Smooth [isotropic](../../../../../isotropy.md) constitutive laws have the corresponding invariant representation across repeated stretches as well. The wording about symmetric functions must be understood in this collective sense: each labelled [principal stress](../../../../../principal-stress.md) need not be symmetric in all three arguments. For example, the objective [isotropic](../../../../../isotropy.md) law $\sigma=V^2$ has $\sigma_i=\lambda_i^2$, which disproves that stronger interpretation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
