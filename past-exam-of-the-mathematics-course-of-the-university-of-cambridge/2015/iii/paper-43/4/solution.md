<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use [gamma matrices](../../../../../gamma-matrices.md) satisfying the [Clifford algebra](../../../../../clifford-algebra.md) relation $\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}$, with $\gamma^{0\dagger}=\gamma^0$ and $\gamma^{i\dagger}=-\gamma^i$. The [Dirac adjoint](../../../../../dirac-adjoint.md) is $\bar\Psi=\Psi^\dagger\gamma^0$. Take the [Dirac action](../../../../../dirac-action.md)

$$
S_D=\int d^4x\,\bar\Psi(i\gamma^\mu\partial_\mu-m)\Psi.
$$

It differs from the manifestly Hermitian form with $(i/2)\bar\Psi\gamma^\mu\overleftrightarrow\partial_\mu\Psi$ only by a boundary term. Treat $\Psi$ and $\bar\Psi$ as independent variables when applying the [principle of stationary action](../../../../../principle-of-stationary-action.md). Varying $\bar\Psi$ gives

$$
\boxed{(i\gamma^\mu\partial_\mu-m)\Psi=0.}
$$

Varying $\Psi$ and integrating by parts gives the [adjoint Dirac equation](../../../../../adjoint-dirac-equation.md), $i(\partial_\mu\bar\Psi)\gamma^\mu+m\bar\Psi=0$. Multiplying the [Dirac equation](../../../../../dirac-equation.md) by $i\gamma^\nu\partial_\nu+m$ also gives $(\Box+m^2)\Psi=0$, so its dispersion relation is [Lorentz invariant](../../../../../lorentz-invariance.md).

For a [Lorentz transformation](../../../../../lorentz-transformation.md) $x'=\Lambda x$, the field transforms in the [Spinor representation of the Lorentz group](../../../../../spinor-representation-of-the-lorentz-group.md):

$$
\Psi'(x')=S(\Lambda)\Psi(x),\qquad S^{-1}\gamma^\mu S=\Lambda^\mu{}_{\nu}\gamma^\nu.
$$

Since $\partial'_\mu=(\Lambda^{-1})^\nu{}_{\mu}\partial_\nu$, this identity gives the [Lorentz covariance of the Dirac operator](../../../../../lorentz-covariance-of-the-dirac-operator.md):

$$
(i\gamma^\mu\partial'_\mu-m)\Psi'(x')=S(\Lambda)(i\gamma^\nu\partial_\nu-m)\Psi(x).
$$

Thus every solution is carried to another solution. The field is a spinor rather than a [four-vector](../../../../../four-vector.md); the transformation of the [gamma matrices](../../../../../gamma-matrices.md) supplies the necessary covariance. The [Dirac action](../../../../../dirac-action.md) is [Lorentz invariant](../../../../../lorentz-invariance.md) because its integrand is a scalar and $d^4x$ is invariant.

For electric charge $q$, use the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) $D_\mu=\partial_\mu+iqA_\mu$. The [minimal electromagnetic coupling of a Dirac field](../../../../../minimal-electromagnetic-coupling-of-a-dirac-field.md) is

$$
\mathcal L=\bar\Psi(i\gamma^\mu D_\mu-m)\Psi-\frac14F_{\mu\nu}F^{\mu\nu}=\bar\Psi(i\gamma^\mu\partial_\mu-m)\Psi-qA_\mu\bar\Psi\gamma^\mu\Psi-\frac14F_{\mu\nu}F^{\mu\nu}.
$$

The local [gauge transformations](../../../../../gauge-transformation.md) in this convention are

$$
\boxed{\Psi'=e^{-iq\alpha(x)}\Psi,\qquad\bar\Psi'=\bar\Psi e^{iq\alpha(x)},\qquad A'_\mu=A_\mu+\partial_\mu\alpha.}
$$

Direct substitution gives $D'_\mu\Psi'=e^{-iq\alpha}D_\mu\Psi$, which proves [gauge covariance of the charged Dirac equation](../../../../../gauge-covariance-of-the-charged-dirac-equation.md). The mass and kinetic terms are invariant, and $F'_{\mu\nu}=F_{\mu\nu}$, so the full action has [gauge invariance](../../../../../gauge-invariance.md). The [conserved current](../../../../../conserved-current.md) is $j^\mu=q\bar\Psi\gamma^\mu\Psi$. It transforms as a [four-vector](../../../../../four-vector.md) under [Lorentz transformations](../../../../../lorentz-transformation.md), and varying $A_\mu$ gives $\partial_\nu F^{\nu\mu}=j^\mu$.

To make the infinitesimal spinor transformation explicit, write $\Lambda^\mu{}_{\nu}=\delta^\mu{}_{\nu}+\omega^\mu{}_{\nu}$ with $\omega_{\mu\nu}=-\omega_{\nu\mu}$. Define

$$
\sigma^{\mu\nu}=\frac i2[\gamma^\mu,\gamma^\nu],\qquad S=1-\frac i4\omega_{\mu\nu}\sigma^{\mu\nu}+O(\omega^2).
$$

The [Lorentz generators from gamma-matrix commutators](../../../../../lorentz-generator-from-gamma-matrix-commutators.md) have precisely the needed algebra: $[\sigma^{\mu\nu},\gamma^\rho]=2i(\eta^{\nu\rho}\gamma^\mu-\eta^{\mu\rho}\gamma^\nu)$, which verifies $S^{-1}\gamma^\rho S=\gamma^\rho+\omega^\rho{}_{\nu}\gamma^\nu$ to first order. The [infinitesimal transformation of a Dirac field](../../../../../infinitesimal-transformation-of-a-dirac-field.md) is therefore

$$
\boxed{\Psi'(x')=\left(1-\frac i4\omega_{\mu\nu}\sigma^{\mu\nu}\right)\Psi(x)+O(\omega^2).}
$$

At the same coordinate argument, the orbital change must also be included:

$$
\boxed{\delta\Psi(x)=-\omega^\mu{}_{\nu}x^\nu\partial_\mu\Psi(x)-\frac i4\omega_{\mu\nu}\sigma^{\mu\nu}\Psi(x).}
$$

Both formulas describe the same transformation; their arguments differ.

Finally, the gamma adjoint identities imply $\sigma^{\mu\nu\dagger}=\gamma^0\sigma^{\mu\nu}\gamma^0$ and hence the [pseudo-unitarity of the spinor Lorentz representation](../../../../../pseudo-unitarity-of-the-spinor-lorentz-representation.md), $S^\dagger\gamma^0S=\gamma^0$. It follows that

$$
\bar\Psi'(x')=\bar\Psi(x)S^{-1},\qquad\boxed{\bar\Psi'(x')\Psi'(x')=\bar\Psi(x)\Psi(x).}
$$

Thus the [Dirac scalar bilinear](../../../../../dirac-scalar-bilinear.md) $\bar\Psi\Psi$ is a [Lorentz scalar](../../../../../lorentz-scalar.md). Infinitesimally the spin terms in $\delta(\bar\Psi\Psi)$ cancel; at fixed coordinates only the ordinary scalar orbital transformation remains.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
