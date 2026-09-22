<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [natural units](../../../../../natural-units.md) and the [Minkowski metric](../../../../../minkowski-metric.md) $g=\operatorname{diag}(1,-1,-1,-1)$. The [Lorentz group](../../../../../lorentz-group.md) is

$$
G=O(1,3)=\{L\in GL(4,\mathbb R):L^TgL=g\}.
$$

Write a transformation near the identity as $L=I+\Omega+O(\Omega^2)$. The defining relation gives $\Omega^Tg+g\Omega=0$, so $\omega_{\mu\nu}=g_{\mu\rho}\Omega^\rho{}_\nu$ is antisymmetric. Choose

$$
(M^{\rho\sigma})^\mu{}_\nu
=g^{\rho\mu}\delta^\sigma_\nu-g^{\sigma\mu}\delta^\rho_\nu,
\qquad
\Omega=\frac12\omega_{\rho\sigma}M^{\rho\sigma}.
$$

There are $\binom42=\boxed{6}$ independent real parameters: three spatial rotations and three [Lorentz boosts](../../../../../lorentz-boost.md). Differentiating $(e^{t\Omega})^Tg e^{t\Omega}$ with respect to $t$ shows it is constant and equals $g$. Thus exponentiating these infinitesimal generators gives [Lorentz transformations](../../../../../lorentz-transformation.md) connected to the identity. The component they generate is the [Proper orthochronous Lorentz group](../../../../../proper-orthochronous-lorentz-group.md) $G_0=SO^+(1,3)$, characterized by $\det L=1$ and $L^0{}_0>0$.

The local exponential calculation alone establishes products of exponentials. The single-exponential assertion also holds here. Use the [Lorentz spinor double cover](../../../../../lorentz-spinor-double-cover.md) $SL(2,\mathbb C)\to SO^+(1,3)$, obtained by acting on $X=x^0I+x^a\sigma_a$ as $X\mapsto AXA^\dagger$. Its [determinant](../../../../../determinant.md) is the Minkowski norm. A lift $A$ with distinct eigenvalues $\lambda,\lambda^{-1}$ is diagonalizable and has a traceless logarithm with eigenvalues $z,-z$, where $e^z=\lambda$. With repeated eigenvalues, choose between $A$ and $-A$ so that the lift is $I+N$ with $N^2=0$; its traceless logarithm is $N$. Since the two signs have the same Lorentz image, exponentiating the differential of the covering map proves [every proper orthochronous Lorentz transformation is an exponential](../../../../../every-proper-orthochronous-lorentz-transformation-is-an-exponential.md):

$$
\boxed{L=\exp\left(\frac12\omega_{\rho\sigma}M^{\rho\sigma}\right).}
$$

It is not a global assertion about the disconnected improper components of $G$.

For [Dirac spinors](../../../../../dirac-spinor.md), choose [gamma matrices](../../../../../gamma-matrices.md) satisfying the [Clifford algebra](../../../../../clifford-algebra.md) $\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}I$ and set

$$
\Sigma^{\rho\sigma}=\frac14[\gamma^\rho,\gamma^\sigma],
\qquad S=\exp\left(\frac12\omega_{\rho\sigma}\Sigma^{\rho\sigma}\right).
$$

The Clifford relations give

$$
[\Sigma^{\rho\sigma},\gamma^\mu]
=g^{\sigma\mu}\gamma^\rho-g^{\rho\mu}\gamma^\sigma.
$$

They also give the stipulated Lorentz [commutator](../../../../../commutator.md) with every $M$ replaced by $\Sigma$: commute $\Sigma$ through the two gamma factors defining the other generator and collect the four terms. Consequently this is a representation of the [Lie algebra of the Lorentz group](../../../../../lie-algebra-of-the-lorentz-group.md), and exponentiation yields

$$
S^{-1}\gamma^\mu S=L^\mu{}_\nu\gamma^\nu,\qquad
\psi'(x')=S\psi(x),\quad x'=Lx.
$$

The [Dirac adjoint](../../../../../dirac-adjoint.md) $\bar\psi=\psi^\dagger\gamma^0$ transforms as $\bar\psi'=\bar\psi S^{-1}$, since $S^\dagger\gamma^0S=\gamma^0$.

There is a global qualification: a spatial rotation through $2\pi$ gives $S=-I$, while its Lorentz [matrix](../../../../../matrix.md) is $I$. Thus **[Dirac spinors](../../../../../dirac-spinor.md) form an ordinary representation of the double cover, and a double-valued representation of $G_0$**, rather than a single-valued linear representation of $G_0$ itself. [Fermion bilinears](../../../../../fermion-bilinear.md) are unaffected by this sign.

For a [scalar field](../../../../../scalar-field.md), $\phi'(x')=\phi(x)$ and its derivative transforms as a covector. A [Lagrangian density](../../../../../lagrangian-density.md) must have all Lorentz indices contracted into scalars using invariant tensors; arbitrary scalar potentials are allowed. For example the kinetic contraction and a potential $V(\phi)$ are invariant. Lorentz invariance by itself does not restrict the potential to quartic order: that restriction would be an additional four-dimensional power-counting requirement.

Define $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3$. It commutes with all $\Sigma^{\rho\sigma}$, so the [axial current](../../../../../axial-current.md) $j_5^\mu=\bar\psi\gamma^\mu\gamma^5\psi$ transforms as a vector under $G_0$. Hence **all three proposed contractions are invariant under $G_0$**. If invariance under parity or the full improper [Lorentz group](../../../../../lorentz-group.md) is also required, the distinction is:

$$
\begin{array}{c|c|c}
\text{operator}&G_0&\text{parity, for ordinary scalar }\phi\\ \hline
\partial_\mu\phi\,\partial^\mu\phi&\text{invariant}&\text{even}\\
\partial_\mu\phi\,j_5^\mu&\text{invariant}&\text{odd}\\
j_{5\mu}j_5^\mu&\text{invariant}&\text{even}.
\end{array}
$$

The [axial current](../../../../../axial-current.md) is a [pseudovector](../../../../../pseudovector.md): under an improper [Lorentz transformation](../../../../../lorentz-transformation.md) it has the extra [determinant](../../../../../determinant.md) sign. The mixed derivative–axial contraction is therefore a [pseudoscalar](../../../../../pseudoscalar.md), while the square of the [axial current](../../../../../axial-current.md) has two cancelling signs. If $\phi$ is itself a [pseudoscalar](../../../../../pseudoscalar.md), its derivative supplies the second sign and the mixed coupling becomes parity even. This is the [axial derivative coupling and parity](../../../../../axial-derivative-coupling-and-parity.md) distinction; parity invariance must not be silently assumed from proper Lorentz invariance.

In four dimensions, $[\phi]=1$, $[\psi]=3/2$ and $[\partial_\mu]=1$. The three operators have [mass dimensions](../../../../../mass-dimension.md) $4,5,6$, respectively. Thus the latter two require dimensionful couplings and are not power-counting renormalizable interactions, but this does not invalidate their Lorentz invariance or their use in an [effective field theory](../../../../../effective-field-theory.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
