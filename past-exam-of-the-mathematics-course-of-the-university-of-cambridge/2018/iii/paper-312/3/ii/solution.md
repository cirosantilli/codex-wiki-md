<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Q^{ij}=\hat k^i\hat k^j-\delta^{ij}/3$. Rotations around $\hat{\mathbf k}$ and the vanishing trace imply that the angular integral in the [scalar neutrino anisotropic stress](../../../../../../scalar-neutrino-anisotropic-stress.md) has the form $A_\ell Q^{ij}$. Contract with $\hat k_i\hat k_j$ and use $\mu^2-1/3=(2/3)P_2(\mu)$. By the [Orthogonality of Legendre polynomials](../../../../../../orthogonality-of-legendre-polynomials.md),

$$
\frac23 A_\ell=\frac12\int_{-1}^{1}P_\ell(\mu)\left(\mu^2-\frac13\right)d\mu
=\frac23\frac{\delta_{\ell2}}5,
\qquad A_\ell=\frac{\delta_{\ell2}}5.
$$

Only the quadrupole in the [neutrino Boltzmann hierarchy](../../../../../../neutrino-boltzmann-hierarchy.md) contributes. Its phase factor is $(-i)^2=-1$, so the supplied stress definition becomes

$$
\Pi^{\hat i\hat j}(\eta,\mathbf x)
=\frac45\bar\rho_\nu\int\frac{d^3\mathbf k}{(2\pi)^{3/2}}\Theta_2(\eta,\mathbf k)Q^{ij}e^{i\mathbf k\cdot\mathbf x}.
$$

Comparing with the chosen normalization $-(4/3)\bar\rho_\nu\Pi Q^{ij}$ gives

$$
\boxed{\Pi(\eta,\mathbf k)=-\frac35\Theta_2(\eta,\mathbf k)}.
$$

The sign and factor here follow jointly from the stress convention and the unweighted [Legendre polynomial](../../../../../../legendre-polynomial.md) coefficients; they should not be transferred unchanged to a differently normalized hierarchy.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
