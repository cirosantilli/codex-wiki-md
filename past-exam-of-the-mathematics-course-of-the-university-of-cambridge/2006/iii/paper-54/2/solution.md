<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $\eta_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$, $\sigma^\mu=(I,\boldsymbol\sigma)$ and $\bar\sigma^\mu=(I,-\boldsymbol\sigma)$, where $\boldsymbol\sigma$ are the [Pauli matrices](../../../../../pauli-matrices.md). The translation and [Lorentz generators](../../../../../lorentz-generator.md) obey the [Poincare algebra](../../../../../poincare-algebra.md)

$$
\begin{aligned}
[P_\mu,P_\nu]&=0,\\
[M_{\mu\nu},P_\rho]&=i(\eta_{\nu\rho}P_\mu-\eta_{\mu\rho}P_\nu),\\
[M_{\mu\nu},M_{\rho\sigma}]&=i(\eta_{\nu\rho}M_{\mu\sigma}-\eta_{\mu\rho}M_{\nu\sigma}-\eta_{\nu\sigma}M_{\mu\rho}+\eta_{\mu\sigma}M_{\nu\rho}).
\end{aligned}
$$

One can derive the additional relations by realizing the [supercharges](../../../../../supersymmetry-generator.md) as differential operators on [superspace](../../../../../superspace.md). With [left Grassmann derivatives](../../../../../left-grassmann-derivative.md) and $P_\mu=i\partial_\mu$, take

$$
Q_\alpha=\partial_{\theta^\alpha}-i\sigma^\mu_{\alpha\dot\beta}\bar\theta^{\dot\beta}\partial_\mu,
\qquad
\bar Q_{\dot\beta}=-\partial_{\bar\theta^{\dot\beta}}+i\theta^\alpha\sigma^\mu_{\alpha\dot\beta}\partial_\mu.
$$

Using $\{\partial_{\theta^\alpha},\theta^\beta\}=\delta_\alpha{}^\beta$, the two mixed derivative-coordinate terms each give $i\sigma^\mu_{\alpha\dot\beta}\partial_\mu$. The remaining terms cancel by Grassmann anticommutation. Equal-chirality terms cancel in the same way. Hence

$$
\boxed{\{Q_\alpha,\bar Q_{\dot\beta}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu,\qquad\{Q_\alpha,Q_\beta\}=\{\bar Q_{\dot\alpha},\bar Q_{\dot\beta}\}=0.}
$$

All coefficients are independent of $x$, so direct differentiation gives $[P_\mu,Q_\alpha]=[P_\mu,\bar Q_{\dot\alpha}]=0$. This also shows that [supercharges commute with translations](../../../../../supercharges-commute-with-translations.md) and preserve the four-momentum of a state.

For the [Lorentz generators](../../../../../lorentz-generator.md), define the left-handed spinor matrices

$$
S_{\mu\nu}=\frac{i}{4}(\sigma_\mu\bar\sigma_\nu-\sigma_\nu\bar\sigma_\mu).
$$

The identity $\sigma^\mu\bar\sigma^\nu+\sigma^\nu\bar\sigma^\mu=2\eta^{\mu\nu}I$ gives their Lorentz commutation relations. Acting on the spinor superspace coordinates and their dual derivatives then gives, in a column-component convention,

$$
\boxed{[M_{\mu\nu},Q_\alpha]=-(S_{\mu\nu})_\alpha{}^\beta Q_\beta,\qquad
[M_{\mu\nu},\bar Q_{\dot\alpha}]=(S_{\mu\nu}^{*})_{\dot\alpha}{}^{\dot\beta}\bar Q_{\dot\beta}.}
$$

Here dotted index values are identified with the conjugate undotted values, and $\bar Q_{\dot\alpha}=Q_\alpha^\dagger$. The second formula also follows directly by taking the adjoint of the first, using Hermitian $M_{\mu\nu}$. For example, $S_{12}=\sigma^3/2$, so $[J_3,Q_1]=-Q_1/2$ and $[J_3,Q_2]=Q_2/2$ for $J_3=M_{12}$. This explicit component convention avoids reversing signs by mixing state matrices with operator-component matrices. Covariance of the mixed [anticommutator](../../../../../anticommutator.md) follows by applying these matrices to $\sigma^\rho P_\rho$.

These are the minimal [Super-Poincaré algebra](../../../../../super-poincare-algebra.md) relations. In the ordinary particle algebra a possible scalar term in $\{Q_\alpha,Q_\beta\}$ would be proportional to $\epsilon_{\alpha\beta}$, but an anticommutator is symmetric in its two labels; with only one supersymmetry such a central term vanishes. Extended algebras can instead use an antisymmetric internal index tensor. Tensor charges associated with extended objects are not part of this minimal particle algebra.

For a positive-energy [massless supermultiplet](../../../../../massless-supermultiplet.md), choose $p^\mu=(E,0,0,E)$ with $E>0$, so $p_\mu=(E,0,0,-E)$ and

$$
\{Q_\alpha,Q_\beta^\dagger\}=2\sigma^\mu_{\alpha\dot\beta}p_\mu
=\begin{pmatrix}0&0\\0&4E\end{pmatrix}.
$$

Positivity of the Hilbert-space norm implies that both $Q_1$ and $Q_1^\dagger$ annihilate every state: their squared norms sum to zero. Set

$$
a=\frac{Q_2}{\sqrt{4E}},\qquad a^\dagger=\frac{Q_2^\dagger}{\sqrt{4E}},\qquad
\{a,a^\dagger\}=1,\quad a^2=(a^\dagger)^2=0.
$$

For momentum along the positive third axis, [helicity](../../../../../helicity.md) is $h=J_3$. The Lorentz commutators give $[h,a]=a/2$ and $[h,a^\dagger]=-a^\dagger/2$. Choose a highest-helicity [Clifford vacuum](../../../../../clifford-vacuum.md) $|\lambda\rangle$ with $a|\lambda\rangle=0$. Its partner $a^\dagger|\lambda\rangle$ has unit norm if the first state does and has helicity $\lambda-1/2$. No further state is generated because $(a^\dagger)^2=0$. Therefore

$$
\boxed{\text{an irreducible finite-helicity massless }\mathcal N=1\text{ multiplet has helicities }(\lambda,\lambda-\tfrac12).}
$$

The two states have opposite [fermion parity](../../../../../fermion-parity.md). A [CPT completion of a supermultiplet](../../../../../cpt-completion-of-a-supermultiplet.md) adds helicities $(-\lambda,-\lambda+1/2)$ and conjugate internal charges when necessary. Taking $\lambda=1/2$ produces a complex scalar and a [Weyl spinor](../../../../../weyl-spinor.md) after CPT completion; taking $\lambda=1$ produces the massless [vector multiplet](../../../../../supersymmetric-vector-multiplet.md). This construction assumes ordinary finite-helicity particle representations, rather than continuous-spin representations.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
