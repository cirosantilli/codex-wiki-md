<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

At the usual two-derivative order, the [two-derivative global supersymmetric gauge action](../../../../../two-derivative-global-supersymmetric-gauge-action.md) is

$$
\begin{aligned}
S=\int d^4x\biggl\{&\int d^4\theta\,K(\Phi,\Phi^\dagger,V)\\
&+\left[\int d^2\theta\left(W(\Phi)+\frac14f_{ab}(\Phi)\mathcal W^{a\alpha}\mathcal W^b_\alpha\right)+\mathrm{h.c.}\right]
+2\sum_{a\text{ Abelian}}\xi_a\int d^4\theta\,V^a\biggr\}.
\end{aligned}
$$

Here $\mathcal W^a_\alpha$ is the [chiral field-strength superfield](../../../../../chiral-field-strength-superfield.md), distinguished from the [superpotential](../../../../../superpotential.md) $W$. The [Kähler potential](../../../../../kahler-potential.md) $K$ is a real gauge-invariant function, defined up to a [Kähler transformation](../../../../../kahler-transformation.md); $K_{i\bar j}$ supplies the scalar kinetic metric. The [superpotential](../../../../../superpotential.md) is a gauge-invariant [holomorphic function](../../../../../holomorphic-function.md) of the [chiral superfields](../../../../../chiral-superfield.md). The symmetric [gauge kinetic function](../../../../../gauge-kinetic-function.md) $f_{ab}$ is holomorphic and transforms so that its contraction with the field strengths is gauge invariant. Its real part supplies the gauge and gaugino kinetic coefficients and must be positive on physical configurations; its imaginary part supplies the topological angle. The final constants are [Fayet–Iliopoulos terms](../../../../../fayet-iliopoulos-term.md), normalized so that they contribute $\xi_aD^a$ when $V^a$ has highest component $\theta^2\bar\theta^2D^a/2$.

**For the simple non-Abelian gauge group specified in the question, $\xi=0$.** Invariance of a proposed $\xi_aD^a$ requires $\xi_af^a{}_{bc}=0$. A simple Lie algebra equals its commutator algebra, so no nonzero invariant covector exists. This proves that [Fayet–Iliopoulos terms require an Abelian gauge factor](../../../../../fayet-iliopoulos-terms-require-an-abelian-gauge-factor.md). The last term above describes the customary Abelian extension, not an additional arbitrary coupling of the simple group.

For a renormalizable theory, after choosing matter bases the functions reduce to

$$
\begin{aligned}
K&=\Phi_i^\dagger Z^i{}_j e^{2V}\Phi^j,\\
W&=c+a_i\Phi^i+\tfrac12m_{ij}\Phi^i\Phi^j+\tfrac16y_{ijk}\Phi^i\Phi^j\Phi^k,\\
f_{ab}&=Y\delta_{ab}.
\end{aligned}
$$

Only gauge-invariant monomials are included. A nonconstant $f$ would produce interactions of dimension greater than four. Here the gauge coupling is absorbed into the connection in $e^{2V}$, while $\operatorname{Re}Y=1/g_h^2$ in the holomorphic normalization. A constant $c$ has no dynamical effect in global supersymmetry. The original arbitrary functions remain useful for a nonrenormalizable two-derivative effective theory, but the following argument restricts to the requested renormalizable setting.

To analyze perturbative corrections, use a local [Wilsonian effective action](../../../../../wilsonian-effective-action.md) with a nonzero infrared cutoff and keep the same elementary fields. Introduce nondynamical background [chiral superfields](../../../../../chiral-superfield.md) $X,Y$ into its [F-term](../../../../../f-term.md) part:

$$
\int d^2\theta\left[XW_{\rm tree}(\Phi)+\frac14Y\mathcal W^{a\alpha}\mathcal W^a_\alpha\right]+\mathrm{h.c.},\qquad X=1\text{ at the end}.
$$

One may additionally promote each polynomial coefficient to its own chiral spurion to track flavor charges. Treating the couplings as fields ensures that a local chiral integral depends holomorphically on $\Phi,X,Y$: antichiral dependence would violate the chirality constraint unless accompanied by derivatives or rewritten as a [D-term](../../../../../d-term.md). This is the key use of [holomorphy](../../../../../holomorphic-function.md), rather than an assumption that all effective-action terms are holomorphic.

Give $\theta$ [R-charge](../../../../../r-charge.md) one, the matter fields charge zero, $X$ charge two and $Y$ charge zero. Then the chiral measure has charge minus two, $XW_{\rm tree}$ has charge two, and $\mathcal W_\alpha$ has charge one. These assignments define formal spurionic symmetries even if fixed numerical couplings do not enjoy the corresponding physical symmetry. An anomalous transformation is accompanied by the appropriate shift of the gauge-coupling spurion; nonperturbative dependence can record that anomaly.

For the [superpotential non-renormalization](../../../../../non-renormalization-theorem.md) argument, perturbation theory is insensitive to continuous shifts of the topological angle, which shifts the imaginary part of $Y$. A holomorphic coefficient invariant under every such shift is independent of $Y$ by the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md). This proves [perturbative gauge-coupling independence of the Wilsonian superpotential](../../../../../perturbative-gauge-coupling-independence-of-the-wilsonian-superpotential.md). At fixed infrared cutoff the perturbative expansion is regular near zero superpotential couplings. R-charge two therefore forces an allowed correction to be linear in $X$, rather than involving $X^2$, $\bar X$ or inverse powers of $X$. Flavor charges impose the corresponding monomial selection rules.

The remaining coefficient can be evaluated at zero gauge coupling. Free chiral propagators join a chiral and an antichiral endpoint. A single holomorphic superpotential vertex cannot close a loop; adding antichiral vertices violates holomorphy, while adding holomorphic vertices violates the linear spurion degree. Consequently the coefficient is its tree value. This proves, rather than merely quotes, the perturbative result

$$
\boxed{W_{\rm Wilsonian}^{\rm pert}=W_{\rm tree}.}
$$

The fixed-cutoff regularity matters: integrating out a whole massive multiplet can introduce inverse masses at tree level, and infrared-singular one-particle-irreducible expressions are not this local Wilsonian superpotential.

For the [gauge kinetic function](../../../../../gauge-kinetic-function.md), R-charge zero excludes regular positive powers of $X$ in its perturbative coefficient. Flavor spurions cannot repair this without forbidden antichiral or singular dependence. A topological-angle shift changes the tree gauge term only by its topological contribution, so the correction $f-Y$ is invariant under the shift. [Holomorphy](../../../../../holomorphic-function.md) then makes it independent of $Y$. An $L$-loop correction to the inverse gauge coupling carries the weak-coupling behavior $g_h^{2L-2}$: only one loop has the required coupling-independent behavior. Hence the [one-loop exactness of the holomorphic gauge kinetic function](../../../../../one-loop-exactness-of-the-holomorphic-gauge-kinetic-function.md) gives

$$
\boxed{f_{\rm pert}(\mu)=Y+\frac{b_0}{8\pi^2}\log\frac{\mu}{\mu_0},\qquad b_0=3C_2(G)-\sum_iT(R_i),}
$$

up to a one-loop matching constant. The coefficient follows from the usual one-loop field contributions: gauge bosons and an adjoint Weyl gaugino contribute $(11/3-2/3)C_2=3C_2$, while a chiral Weyl fermion and complex scalar contribute $-(2/3+1/3)T(R)=-T(R)$. Holomorphic logarithmic thresholds appear when massive fields are eliminated. This statement is about the holomorphic Wilsonian coupling, not a canonically normalized physical gauge coupling, whose running need not be one-loop exact.

The [Kähler potential](../../../../../kahler-potential.md) is integrated over all of [superspace](../../../../../superspace.md). It can depend on $X^\dagger X$, on both $Y$ and $Y^\dagger$, and on both matter chiralities. These neutral combinations allow ordinary loop corrections, such as a Yukawa-dependent correction to $\Phi^\dagger\Phi$, and no analogous argument forbids higher loops. Thus

$$
\boxed{K\text{ generally renormalizes at every loop order}.}
$$

Its [wave-function renormalization](../../../../../wave-function-renormalization.md) changes physical superpotential couplings after canonical normalization even though holomorphic vertex coefficients do not change. For a single field with kinetic coefficient $Z$, for instance, $m_c=m/Z$ and $y_c=y/Z^{3/2}$.

Finally consider [perturbative renormalization of a Fayet–Iliopoulos term](../../../../../perturbative-renormalization-of-a-fayet-iliopoulos-term.md) in an Abelian extension. A term $\int d^4\theta\,H(X,X^\dagger,Y,Y^\dagger)V$ must be invariant under $V\mapsto V+\Lambda+\Lambda^\dagger$ for arbitrary chiral $\Lambda$. Projection of the variation requires $\bar D^2H=D^2H=0$. An arbitrary algebraic function of background chiral spurions and their conjugates fails this requirement unless it is constant. Therefore a general coupling-dependent local FI counterterm is forbidden. The one-loop $D$ tadpole from charged scalars can still give

$$
\delta\xi\ \propto\ \left(\sum_iq_i\right)\int_{\mu<|p|<\Lambda_{\rm UV}}\frac{d^4p}{(2\pi)^4p^2}.
$$

It is independent of interaction couplings in the connection normalization used above and proportional to the trace of the Abelian charge generator. Higher-loop diagrams require interactions and cannot produce the permitted coupling-independent additive term. Thus **a traceless Abelian charge generator has no additive perturbative FI renormalization in this exactly supersymmetric setting**; otherwise a one-loop, regulator-dependent tadpole is possible. Vector-field normalization can change the reported canonical parameter, and soft breaking falls outside this proof. For the specified simple group, gauge invariance forbids $\xi$ before and after corrections.

These are perturbative statements. [Instantons](../../../../../instanton.md) or other nonperturbative effects may produce symmetry-allowed holomorphic terms, for example dependence on $e^{-8\pi^2Y}$, so neither the superpotential result nor the one-loop gauge result should be misread as forbidding all nonperturbative corrections.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
