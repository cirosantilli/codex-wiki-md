<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [positive energy theorem](../../../../../positive-energy-theorem.md) concerns the total gravitational energy of isolated systems, rather than a pointwise gravitational energy density. Its standard asymptotically flat form is

$$
\boxed{E_{\rm ADM}\geq |\mathbf P_{\rm ADM}|.}
$$

Here are the hypotheses used in a spinorial proof. Take smooth, complete, three-dimensional [initial data in general relativity](../../../../../initial-data-in-general-relativity.md) $(\Sigma,h,k)$ with a [spin structure](../../../../../spin-structure.md), no inner boundary, and finitely many asymptotically Euclidean ends. Assume the usual differentiable falloff $h_{ij}-\delta_{ij}=O(r^{-1})$, $\partial h=O(r^{-2})$, $k_{ij}=O(r^{-2})$, with sufficiently decaying further derivatives and integrable matter densities. The [Hamiltonian constraint](../../../../../hamiltonian-constraint.md) and [momentum constraint](../../../../../momentum-constraint.md) must hold, and the matter must satisfy the [dominant energy condition](../../../../../dominant-energy-condition.md). These hypotheses exclude a naked singularity or an unaccounted boundary flux from the argument. An oriented three-manifold admits a [spin structure](../../../../../spin-structure.md); in higher dimensions the spinorial proof needs this as an additional assumption. Work in signature $(-+++)$ and units $G=c=1$.

Let $n$ be the future unit normal, choose $k_{ij}=-g(\nabla_i n,e_j)$, and define $\mu=T_{ab}n^an^b$ and $J_i=-T_{ab}n^ae_i^b$. With this convention the [Hamiltonian constraint](../../../../../hamiltonian-constraint.md) and [momentum constraint](../../../../../momentum-constraint.md) read

$$
R(h)+(\operatorname{tr}k)^2-|k|^2=16\pi\mu,
\qquad D^j(k_{ij}-h_{ij}\operatorname{tr}k)=8\pi J_i.
$$

The [dominant energy condition](../../../../../dominant-energy-condition.md) implies $\mu\geq |J|_h$. The asymptotic charges are the [ADM energy](../../../../../arnowitt-deser-misner-energy.md) and [ADM momentum](../../../../../adm-momentum.md),

$$
E=\frac1{16\pi}\lim_{r\to\infty}\int_{S_r}(\partial_jh_{ij}-\partial_ih_{jj})s^i\,dS,
\qquad P_i=\frac1{8\pi}\lim_{r\to\infty}\int_{S_r}(k_{ij}-h_{ij}\operatorname{tr}k)s^j\,dS.
$$

These are boundary charges; a sign condition on $\mu$ alone does not visibly determine their sign.

Choose [gamma matrices](../../../../../gamma-matrices.md) obeying $\{\gamma^a,\gamma^b\}=2g^{ab}$, with spatial matrices Hermitian and $\gamma^{\hat0}$ anti-Hermitian. The relevant derivative is the [Sen spinor connection](../../../../../sen-spinor-connection.md), not just the intrinsic [spin connection](../../../../../spin-connection.md):

$$
\nabla_i\epsilon=D_i^{(3)}\epsilon-\frac12k_{ij}\gamma^j\gamma^{\hat0}\epsilon,
\qquad \mathcal D\epsilon=\gamma^i\nabla_i\epsilon.
$$

The symmetric [extrinsic curvature](../../../../../extrinsic-curvature.md) makes $\mathcal D=\gamma^iD_i^{(3)}-\tfrac12(\operatorname{tr}k)\gamma^{\hat0}$. This is an [elliptic differential operator](../../../../../elliptic-differential-operator.md) with the ordinary spatial [Dirac operator](../../../../../dirac-operator.md) as principal part. Solve the [Witten spinor equation](../../../../../witten-spinor-equation.md) $\mathcal D\epsilon=0$, with $\epsilon\to\epsilon_\infty$ constant at the end under consideration and zero asymptotic constants at any other ends.

The central algebraic ingredient is the [Witten-Nester identity](../../../../../witten-nester-identity.md). Define $\bar\epsilon=-\epsilon^\dagger\gamma^{\hat0}$, the future-directed [Dirac current](../../../../../dirac-current.md) $K^a=\bar\epsilon\gamma^a\epsilon$, and the [Nester two-form](../../../../../nester-two-form.md)

$$
B^{ab}=\bar\epsilon\gamma^{abc}\nabla_c\epsilon-\overline{\nabla_c\epsilon}\gamma^{abc}\epsilon,
\qquad b^i=n_aB^{ai}.
$$

In an orthonormal frame $K^0=|\epsilon|^2$. Since $-\gamma^{\hat0}\gamma^i q_i$ is Hermitian with eigenvalues $\pm1$ for any unit spatial vector $q$, $|\mathbf K|\leq K^0$. Thus the [Dirac current](../../../../../dirac-current.md) is future causal. Differentiate the [Nester two-form](../../../../../nester-two-form.md) by the product rule. The antisymmetric second-derivative terms reduce using the [spinor curvature identity](../../../../../spinor-curvature-identity.md)

$$
[\nabla_a,\nabla_b]\epsilon=\frac14R_{ab cd}\gamma^{cd}\epsilon.
$$

The [Clifford algebra](../../../../../clifford-algebra.md) and the first [Bianchi identity](../../../../../bianchi-identity.md) turn the curvature contraction into the [Einstein tensor](../../../../../einstein-tensor.md). The spatial derivative terms give the difference of two squares. Projecting onto $\Sigma$ therefore gives

$$
D_i b^i=2\bigl(|\nabla_i\epsilon|^2-|\mathcal D\epsilon|^2\bigr)+G_{ab}n^aK^b
=2\bigl(|\nabla_i\epsilon|^2-|\mathcal D\epsilon|^2\bigr)+8\pi T_{ab}n^aK^b.
$$

The constraints are exactly the normal components of the [Einstein field equations](../../../../../einstein-field-equations.md) needed here. Moreover,

$$
T_{ab}n^aK^b=\mu K^0-J_iK^i\geq(\mu-|J|)K^0\geq0.
$$

For a solution of the [Witten spinor equation](../../../../../witten-spinor-equation.md), both terms left in this divergence are nonnegative.

There is an essential analytic step: an asymptotically constant [spinor field](../../../../../spinor-field.md) solving the [Witten spinor equation](../../../../../witten-spinor-equation.md) must actually exist. Extend the chosen constant smoothly from infinity to a field $\epsilon_0$. Then $\mathcal D\epsilon_0=O(r^{-2})$ is square-integrable. For compactly supported fields $\eta$, the same [Witten-Nester identity](../../../../../witten-nester-identity.md) has zero boundary flux and gives

$$
\|\mathcal D\eta\|_2^2=\|\nabla\eta\|_2^2+4\pi\int_\Sigma T_{ab}n^aK^b[\eta]\,dV\geq\|\nabla\eta\|_2^2.
$$

The asymptotically Euclidean [Hardy inequality in Euclidean space](../../../../../hardy-inequality-in-euclidean-space.md), local elliptic estimates and this identity supply the coercive estimate in the weighted first-order [Sobolev space](../../../../../sobolev-space-split.md) of decaying corrections. One way to see why a compact-region error cannot spoil coercivity is to assume the estimate fails and take a normalized sequence whose [Dirac operator](../../../../../dirac-operator.md) tends to zero. Local compactness and the estimate on the ends produce a decaying homogeneous solution. Integrating the identity with cutoffs shows that such a solution is parallel for the [Sen spinor connection](../../../../../sen-spinor-connection.md). A parallel field tending to zero at infinity is zero, contradicting its normalization. The end estimates exclude escape of the normalized sequence to infinity.

More constructively, on this completed correction space solve

$$
\int_\Sigma\langle\mathcal D\eta,\mathcal D\chi\rangle\,dV
=-\int_\Sigma\langle\mathcal D\epsilon_0,\mathcal D\chi\rangle\,dV
$$

for every compactly supported $\chi$, using the [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md). Set $\epsilon=\epsilon_0+\eta$. Since $\mathcal D$ is formally skew-adjoint in the positive spatial spinor inner product, the residual $\xi=\mathcal D\epsilon$ is a square-integrable weak solution of $\mathcal D\xi=0$. Elliptic regularity makes it smooth. Cutoff integration of the identity excludes a nonzero square-integrable homogeneous solution: it would be parallel, whereas a nonzero parallel field has nonzero limiting norm on an asymptotically Euclidean end and cannot be square-integrable. Hence $\xi=0$. Weighted elliptic estimates then give the required asymptotic decay of $\eta$. This supplies [elliptic existence of a Witten spinor](../../../../../elliptic-existence-of-a-witten-spinor.md), rather than assuming it from the sign of a formal integral.

Finally integrate the [Witten-Nester identity](../../../../../witten-nester-identity.md) over $\Sigma$. The [ADM boundary term of the Nester two-form](../../../../../adm-boundary-term-of-the-nester-two-form.md) is

$$
\lim_{r\to\infty}\int_{S_r}b^is_i\,dS=8\pi(EK^0_\infty-P_iK^i_\infty).
$$

To identify this boundary term, expand the asymptotic [spin connection](../../../../../spin-connection.md) to first order in $h-\delta$. Its flux is half of $(\partial_jh_{ij}-\partial_ih_{jj})s^iK^0_\infty$; the [extrinsic curvature](../../../../../extrinsic-curvature.md) contribution is $-(k_{ij}-h_{ij}\operatorname{tr}k)s^jK^i_\infty$. Their coefficients give precisely the two charges displayed above. The derivative of the decaying spinor correction has zero leading integrated flux by antisymmetry, and the higher-order terms vanish with the falloff. Thus

$$
EK^0_\infty-P_iK^i_\infty
=\frac1{4\pi}\int_\Sigma|\nabla\epsilon|^2\,dV+
\int_\Sigma T_{ab}n^aK^b\,dV\geq0.
$$

Choose a normalized asymptotic [spinor field](../../../../../spinor-field.md) that is an eigenvector with eigenvalue $+1$ of $-\gamma^{\hat0}\gamma^i q_i$. Then $K^0_\infty=1$ and $\mathbf K_\infty=q$. Choosing $q=\mathbf P/|\mathbf P|$ proves $E\geq|\mathbf P|$; if $\mathbf P=0$, any such choice gives $E\geq0$. This is positivity in every asymptotic frame, not only the zero-momentum case.

The zero-energy rigidity also follows from the vanishing integrals. If $E=0$, then $\mathbf P=0$ and the construction for a basis of asymptotic spinors produces a basis of parallel fields. Their [spinor curvature identity](../../../../../spinor-curvature-identity.md) forces the spatially pulled-back spacetime curvature to vanish; the nonnegative matter terms vanish too. The resulting [Gauss–Codazzi equations](../../../../../gauss-codazzi-equations.md) are those of a hypersurface in [Minkowski spacetime](../../../../../minkowski-spacetime.md), and its vacuum development is flat. Completeness and the ordinary Euclidean asymptotic end rule out a nontrivial flat quotient. The initial hypersurface need not have $k=0$: a curved spacelike slice of [Minkowski spacetime](../../../../../minkowski-spacetime.md) also has zero [ADM energy](../../../../../arnowitt-deser-misner-energy.md). **The proof works by converting an asymptotic energy charge into a nonnegative bulk integral, with the spinor equation and its existence supplying the crucial bridge.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
