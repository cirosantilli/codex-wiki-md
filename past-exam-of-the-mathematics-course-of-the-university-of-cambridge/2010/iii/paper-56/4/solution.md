<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Killing spinor](../../../../../killing-spinor.md) is a nonzero spinor parameter for which the fermionic [supersymmetry](../../../../../supersymmetry-split.md) variations vanish on a bosonic background. In [minimal four-dimensional supergravity](../../../../../minimal-four-dimensional-supergravity.md) without a cosmological term this means

$$
\boxed{\nabla_\mu\epsilon=0.}
$$

It is an overdetermined equation and expresses an unbroken [supersymmetry](../../../../../supersymmetry-split.md) of the background. In the cosmological deformation the corresponding equation is $\mathcal D_\mu\epsilon=0$; in theories with additional bosonic fields their contributions also enter the [fermion](../../../../../fermion.md) variations.

For the undeformed theory the connection preserves both the spinor adjoint and gamma matrices. Consequently the [Dirac current](../../../../../dirac-current.md)

$$
K^\mu=\bar\epsilon\gamma^\mu\epsilon
$$

obeys $\nabla_\nu K_\mu=0$. In particular $\nabla_{(\nu}K_{\mu)}=0$, so **$K$ is a [Killing vector](../../../../../killing-vector-field.md)**, and in fact is parallel. For the real cosmological deformation, $\nabla_\mu\epsilon=-(m/2)\gamma_\mu\epsilon$ and $\nabla_\mu\bar\epsilon=(m/2)\bar\epsilon\gamma_\mu$ instead give $\nabla_\mu K_\nu=(m/2)\bar\epsilon[\gamma_\mu,\gamma_\nu]\epsilon$, whose symmetric part again vanishes.

The causal property uses an ordinary commuting spinor. Take an orthonormal frame with $(\gamma^0)^\dagger=-\gamma^0$, $(\gamma^i)^\dagger=\gamma^i$, and $\bar\epsilon=\epsilon^\dagger\gamma^0$. Then $K^0=-\epsilon^\dagger\epsilon$. Reverse its time orientation and write $V=-K$, so

$$
V^0=\epsilon^\dagger\epsilon,\qquad V^i=\epsilon^\dagger\alpha^i\epsilon,\qquad\alpha^i=-\gamma^0\gamma^i.
$$

The matrices $\alpha^i$ are Hermitian and obey $\{\alpha^i,\alpha^j\}=2\delta^{ij}$. For every spatial [unit vector](../../../../../unit-vector.md) $u$, $(u_i\alpha^i)^2=1$, whence $|u_iV^i|\le V^0$. Choose $u$ along the spatial part of $V$ to obtain

$$
\boxed{K_\mu K^\mu=V_\mu V^\mu=-(V^0)^2+|\mathbf V|^2\le0.}
$$

A nonzero [Killing spinor](../../../../../killing-spinor.md) cannot vanish at an isolated point: its defining connection equation transports its value along every curve. Thus on a connected background this is a nonzero, nowhere-spacelike [causal Dirac spinor current](../../../../../causal-dirac-spinor-current.md). The estimate does not need the Majorana condition, but it does need commuting components; Grassmann bilinears have no such ordinary positivity order.

For the [positive energy theorem](../../../../../positive-energy-theorem.md), take a complete asymptotically flat spacelike hypersurface with a [spin structure](../../../../../spin-structure.md) $\Sigma$, with suitable decay, Einstein constraint equations, and matter satisfying the [dominant energy condition](../../../../../dominant-energy-condition.md). Assume there are no inner boundaries, or that any inner-boundary contribution has the required nonnegative sign. The auxiliary commuting spinor approaches an arbitrary constant $\epsilon_\infty$ at spatial infinity. Define the real [Nester two-form](../../../../../nester-two-form.md)

$$
B^{\mu\nu}=\bar\epsilon\gamma^{\mu\nu\rho}\nabla_\rho\epsilon-\overline{\nabla_\rho\epsilon}\gamma^{\mu\nu\rho}\epsilon.
$$

Antisymmetry removes second derivatives except through the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md). Differentiation and the three-gamma [spinor curvature identity](../../../../../spinor-curvature-identity.md) used above give

$$
\nabla_\nu B^{\mu\nu}=2(\nabla_\nu\bar\epsilon)\gamma^{\mu\nu\rho}\nabla_\rho\epsilon+G^{\mu\nu}K_\nu.
$$

The first term comes from differentiating the two spinor factors. For the second term, replace $\nabla_\nu\nabla_\rho$ by half their [commutator](../../../../../commutator.md); its spin-curvature contraction is $G^{\mu\nu}\gamma_\nu/2$ from each conjugate term. This is the reason the [Einstein tensor](../../../../../einstein-tensor.md), and hence the matter energy density, enters the boundary-charge identity.

In an orthonormal frame adapted to the future normal of $\Sigma$, put $\chi_i=\nabla_i\epsilon$. Since $\gamma^0\gamma^{0ij}=-\gamma^{ij}$,

$$
2(\nabla_i\bar\epsilon)\gamma^{0ij}\nabla_j\epsilon=2\left(\sum_i|\chi_i|^2-\left|\sum_i\gamma^i\chi_i\right|^2\right).
$$

Here $\nabla_i$ is the spacetime [spin connection](../../../../../spin-connection.md) pulled back to $\Sigma$, including its [extrinsic curvature](../../../../../extrinsic-curvature.md). Choose the auxiliary spinor to solve the elliptic [Witten spinor equation](../../../../../witten-spinor-equation.md)

$$
\gamma^i\nabla_i\epsilon=0,\qquad\epsilon\longrightarrow\epsilon_\infty.
$$

The standard asymptotic-flatness and completeness hypotheses permit this boundary-value problem; the positivity identity also excludes a decaying homogeneous zero mode. It is this hypersurface equation that removes the negative square. A spacetime [Killing spinor](../../../../../killing-spinor.md) is not assumed for a general initial-data set.

Stokes' theorem and $G_{\mu\nu}=\kappa^2T_{\mu\nu}$ now give

$$
Q[\epsilon_\infty]=\frac1{\kappa^2}\int_{S_\infty}B^{0i}dS_i
=\frac2{\kappa^2}\int_\Sigma|\nabla_i\epsilon|^2dV+\int_\Sigma T_{\mu\nu}n^\mu V^\nu dV\ge0.
$$

The [dominant energy condition](../../../../../dominant-energy-condition.md) makes the second integrand nonnegative because $n$ and $V$ are future causal. Evaluating the two-form with the asymptotic [spin connection](../../../../../spin-connection.md) identifies its surface integral with the [ADM energy](../../../../../arnowitt-deser-misner-energy.md) and [momentum](../../../../../momentum.md):

$$
Q[\epsilon_\infty]=-P_\mu V_\infty^\mu
=\epsilon_\infty^\dagger\bigl(E\,1-P_i\alpha^i\bigr)\epsilon_\infty.
$$

For example its energy term uses $B^{0i}=\tfrac12(\partial_jh_{ij}-\partial_ih_{jj})|\epsilon_\infty|^2$ to first order in the asymptotic spatial [metric tensor](../../../../../metric-tensor.md) perturbation. With $\kappa^2=8\pi G$ this is exactly the ADM normalization. Since $P_i\alpha^i$ has [eigenvalues](../../../../../eigenvalue.md) $\pm|\mathbf P|$, positivity for every boundary spinor proves

$$
\boxed{E\ge|\mathbf P|\ge0.}
$$

[Killing spinors](../../../../../killing-spinor.md) describe saturation: their spatial derivative term vanishes, and the contracted matter term must also vanish for the corresponding charge to be zero. They characterize preserved [supersymmetry](../../../../../supersymmetry-split.md) rather than being prerequisites for positivity. Under the usual rigidity hypotheses, zero total four-momentum makes the nonnegative integral vanish for a full basis of asymptotic spinors; their parallel extensions force a vanishing [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) and give the Minkowski vacuum. A single [Killing spinor](../../../../../killing-spinor.md) with null current alone does not justify asserting that every component of the total [momentum](../../../../../momentum.md) vanishes.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
