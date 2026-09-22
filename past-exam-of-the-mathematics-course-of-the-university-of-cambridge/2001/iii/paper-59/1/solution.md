<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [natural units](../../../../../natural-units.md) and the [Minkowski metric](../../../../../minkowski-metric.md) $g=\operatorname{diag}(1,-1,-1,-1)$. Multiplication of the block [gamma matrices](../../../../../gamma-matrices.md) gives

$$
(\gamma^0)^2=I_4,\qquad
\gamma^j\gamma^k=-\begin{pmatrix}\sigma_j\sigma_k&0\\0&\sigma_j\sigma_k\end{pmatrix},\qquad
\gamma^0\gamma^j=-\gamma^j\gamma^0.
$$

The [Pauli matrices](../../../../../pauli-matrices.md) obey $\sigma_j\sigma_k+\sigma_k\sigma_j=2\delta_{jk}I_2$, so the spatial anticommutators are $-2\delta_{jk}I_4$, the mixed ones are zero, and the temporal one is $2I_4$. Thus

$$
\boxed{\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}I_4.}
$$

Because [partial derivatives](../../../../../partial-derivative.md) commute, only the symmetric part of $\gamma^\mu\gamma^\nu$ survives in their contraction. Multiplying the [Dirac equation](../../../../../dirac-equation.md) on the left by its opposite-mass factor therefore gives the [flat-space Dirac factorization](../../../../../flat-space-dirac-factorization.md)

$$
(i\gamma^\mu\partial_\mu+m)(i\gamma^\nu\partial_\nu-m)\psi
=-(g^{\mu\nu}\partial_\mu\partial_\nu+m^2)\psi=0.
$$

Hence **every component satisfies $\boxed{(\Box+m^2)\psi=0}$**, the [Klein-Gordon equation](../../../../../klein-gordon-equation.md). This implication does not remove the first-order [spinor](../../../../../spinor.md) constraints imposed by the [Dirac equation](../../../../../dirac-equation.md).

For [Lorentz covariance](../../../../../lorentz-covariance.md), transform coordinates by $x'=Lx$ and the [Dirac spinor](../../../../../dirac-spinor.md) by $\psi'(x')=S(L)\psi(x)$. The [chain rule](../../../../../chain-rule.md) gives $\partial'_\mu=(L^{-1})^\nu{}_{\mu}\partial_\nu$. Consequently

$$
\begin{aligned}
S^{-1}(i\gamma^\mu\partial'_\mu-m)\psi'(x')
&=\left[iS^{-1}\gamma^\mu S(L^{-1})^\nu{}_{\mu}\partial_\nu-m\right]\psi(x)\\
&=(i\gamma^\rho\partial_\rho-m)\psi(x)=0.
\end{aligned}
$$

The cancellation uses $L^\mu{}_{\rho}(L^{-1})^\nu{}_{\mu}=\delta^\nu{}_{\rho}$. Thus the [Lorentz transformation](../../../../../lorentz-transformation.md) maps every solution to another, establishing the [Lorentz covariance of the Dirac operator](../../../../../lorentz-covariance-of-the-dirac-operator.md).

The infinitesimal identity follows directly from the [Clifford algebra](../../../../../clifford-algebra.md). Moving $\gamma^\rho$ past the two factors gives

$$
[\gamma^\mu\gamma^\nu,\gamma^\rho]
=2g^{\nu\rho}\gamma^\mu-2g^{\mu\rho}\gamma^\nu.
$$

Subtracting the same identity with $\mu,\nu$ interchanged proves the [spinor Lorentz generator commutator](../../../../../spinor-lorentz-generator-commutator.md)

$$
[\sigma^{\mu\nu},\gamma^\rho]=2i(g^{\nu\rho}\gamma^\mu-g^{\mu\rho}\gamma^\nu).
$$

Contracting with the antisymmetric tensor $\omega_{\mu\nu}$ yields

$$
\frac{i}{4}[\sigma^{\mu\nu}\omega_{\mu\nu},\gamma^\rho]
=-\frac12\left(g^{\nu\rho}\omega_{\mu\nu}\gamma^\mu-g^{\mu\rho}\omega_{\mu\nu}\gamma^\nu\right)
=\boxed{\omega^\rho{}_{\nu}\gamma^\nu}.
$$

It also verifies $S^{-1}\gamma^\rho S=\gamma^\rho+\omega^\rho{}_{\nu}\gamma^\nu+O(\omega^2)$ for the infinitesimal [Spinor representation of the Lorentz group](../../../../../spinor-representation-of-the-lorentz-group.md).

For a positive-energy [four-momentum](../../../../../four-momentum.md), put $\psi=u(p)e^{-ip\cdot x}$, $E=\sqrt{\mathbf p^2+m^2}>0$. The [Dirac equation](../../../../../dirac-equation.md) becomes $(\not p-m)u=0$, where the [Feynman slash notation](../../../../../feynman-slash-notation.md) uses $\not p=\gamma^\mu p_\mu=E\gamma^0-\boldsymbol\gamma\cdot\mathbf p$. Splitting $u=(\xi,\eta)^T$ gives

$$
(E-m)\xi-(\boldsymbol\sigma\cdot\mathbf p)\eta=0,\qquad
(\boldsymbol\sigma\cdot\mathbf p)\xi-(E+m)\eta=0.
$$

The second equation sets $\eta=(\boldsymbol\sigma\cdot\mathbf p)\xi/(E+m)$, and the first is then the [mass shell](../../../../../mass-shell.md), since $(\boldsymbol\sigma\cdot\mathbf p)^2=\mathbf p^2I_2$. Choosing two orthonormal two-spinors $\chi_s$ gives the [Dirac plane waves in the standard representation](../../../../../dirac-plane-waves-in-the-standard-representation.md):

$$
\boxed{\psi_s^{(+)}(x)=u_s(p)e^{-ip\cdot x},\qquad
u_s(p)=\sqrt{E+m}\begin{pmatrix}\chi_s\\\dfrac{\boldsymbol\sigma\cdot\mathbf p}{E+m}\chi_s\end{pmatrix},\quad s=1,2.}
$$

The negative-frequency solutions are independently

$$
\boxed{\psi_s^{(-)}(x)=v_s(p)e^{ip\cdot x},\qquad
v_s(p)=\sqrt{E+m}\begin{pmatrix}\dfrac{\boldsymbol\sigma\cdot\mathbf p}{E+m}\eta_s\\\eta_s\end{pmatrix},\qquad(\not p+m)v_s=0,}
$$

with orthonormal $\eta_s$. They are the [antiparticle](../../../../../antiparticle.md) modes after field quantization. The normalization gives $u_r^\dagger u_s=v_r^\dagger v_s=2E\delta_{rs}$ and $\overline u_ru_s=2m\delta_{rs}$, $\overline v_rv_s=-2m\delta_{rs}$, using the [Dirac adjoint](../../../../../dirac-adjoint.md) $\overline u=u^\dagger\gamma^0$.

For a spatial rotation, $\sigma^{ij}=\epsilon_{ijk}\operatorname{diag}(\sigma_k,\sigma_k)$. Hence the intrinsic rotation generators are

$$
J_k=\frac12\begin{pmatrix}\sigma_k&0\\0&\sigma_k\end{pmatrix},\qquad
[J_i,J_j]=i\epsilon_{ijk}J_k,\qquad \sum_kJ_k^2=\frac34I_4.
$$

For a massive particle in its rest frame, the two independent [spinors](../../../../../spinor.md) therefore carry the two-dimensional [spin one-half](../../../../../spin-one-half.md) representation, with $J_3$ [eigenvalues](../../../../../eigenvalue.md) $\pm1/2$ and Casimir $s(s+1)=3/4$. A $2\pi$ rotation acts as $-I$, the [spinor sign under a full spatial rotation](../../../../../spinor-sign-under-a-full-spatial-rotation.md). Thus **the particle has [spin](../../../../../spin.md) $\boxed{s=1/2}$**; four [spinor](../../../../../spinor.md) components encode particle and antiparticle sectors, not four [spin](../../../../../spin.md) states of one particle. In the [massless limit](../../../../../massless-limit.md) the corresponding physical labels are [helicities](../../../../../helicity.md) $\pm1/2$ rather than a rest-frame [spin](../../../../../spin.md) basis.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
