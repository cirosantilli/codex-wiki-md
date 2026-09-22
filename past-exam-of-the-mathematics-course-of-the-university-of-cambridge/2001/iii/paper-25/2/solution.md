<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The four [Pauli matrices](../../../../../pauli-matrices.md) form an orthogonal basis of $2\times2$ matrices for the [Hilbert-Schmidt inner product](../../../../../hilbert-schmidt-inner-product.md), since $\operatorname{Tr}(\sigma_\mu\sigma_\nu)=2\delta_{\mu\nu}$. A Hermitian [density matrix](../../../../../density-matrix.md) therefore has real coefficients in this basis, and its trace-one condition fixes the identity coefficient. Thus

$$
\boxed{\rho=\frac12(I+n_x\sigma_x+n_y\sigma_y+n_z\sigma_z),\qquad n_j=\operatorname{Tr}(\rho\sigma_j).}
$$

The multiplication rule for the [Pauli matrices](../../../../../pauli-matrices.md) $\sigma_i\sigma_j=\delta_{ij}I+i\epsilon_{ijk}\sigma_k$ implies $(n\cdot\sigma)^2=\|n\|^2I$. Its trace is zero, so for $n\ne0$ its eigenvalues are $\pm\|n\|$; for $n=0$ it vanishes. Hence

$$
\lambda_\pm(\rho)=\frac{1\pm\|n\|}{2}.
$$

Positivity is equivalent to $\|n\|\le1$. Conversely every real vector in this unit ball defines a positive trace-one matrix by the boxed formula. Therefore $\Phi(\rho)=n$ is a one-to-one correspondence with the [Bloch ball](../../../../../bloch-ball.md), with the displayed inverse. Each coordinate is linear in $\rho$, proving the affine property under any convex mixture.

A density matrix is pure precisely when its eigenvalues are $1,0$, equivalently when $\rho^2=\rho$. The eigenvalue formula makes this equivalent to $\|n\|=1$. Alternatively $\operatorname{Tr}\rho^2=(1+\|n\|^2)/2$. Thus **the pure states correspond exactly to the [Bloch sphere](../../../../../bloch-sphere.md)**.

For $n\ne0$, put $\widehat n=n/\|n\|$. The [spectral projectors](../../../../../spectral-projector.md) for the larger and smaller eigenvalues are

$$
P_+=\frac12(I+\widehat n\cdot\sigma),\qquad P_-=\frac12(I-\widehat n\cdot\sigma).
$$

They are orthogonal rank-one projections, have sum $I$, and give $\rho=\lambda_+P_++\lambda_-P_-$. For normalized eigenvectors in this nondegenerate case they equal $|\phi_1\rangle\langle\phi_1|$ and $|\phi_2\rangle\langle\phi_2|$. Their [Bloch vectors](../../../../../bloch-vector.md) are therefore **$\boxed{n_1=n/\|n\|,\quad n_2=-n/\|n\|}$**, the [antipodal eigenprojectors of a qubit density matrix](../../../../../antipodal-eigenprojectors-of-a-qubit-density-matrix.md).

At $n=0$, the state is $I/2$ and both eigenvalues coincide. There is no distinguished direction and the printed directional expression is undefined. Any orthonormal eigenbasis gives an antipodal pair of pure-state Bloch vectors, since its two projectors sum to $I$, but that pair can point in any direction. The nonzero-$n$ qualification is essential. The PDF denominators are $\|n\|$, not the converted TeX denominators involving $n_1,n_2$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
