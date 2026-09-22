<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work with a supersymmetry-preserving regulator and a local [Wilsonian effective action](../../../../../wilsonian-effective-action.md) at a nonzero infrared cutoff, in holomorphic field variables. Its two-derivative terms have the form

$$
\int d^4\theta\,K(\Phi,\Phi^\dagger,V)+\left[\int d^2\theta\left\{W(\Phi)+\frac14f_{ab}(\Phi)\mathcal W^{a\alpha}\mathcal W^b_\alpha\right\}+\mathrm{h.c.}\right].
$$

Here $\mathcal W_\alpha$ is the gauge field-strength superfield, distinct from the [superpotential](../../../../../superpotential.md) $W$, and the [gauge kinetic function](../../../../../gauge-kinetic-function.md) $f_{ab}$ is symmetric and holomorphic. The perturbative [non-renormalization theorem](../../../../../non-renormalization-theorem.md) states

$$
\boxed{W_{\rm Wilsonian}^{\rm pert}=W_{\rm tree},\qquad f_{\rm Wilsonian}^{\rm pert}=f_{\rm tree}+f_{\rm one\ loop}.}
$$

The same elementary light fields are retained in the first equality. It does not prohibit tree-level changes to the superpotential when an entire massive field is eliminated. The [Kähler potential](../../../../../kahler-potential.md) may be renormalized at every loop order, nonperturbative effects are separate, and canonically normalized physical couplings need not satisfy these holomorphic statements.

First prove [superpotential non-renormalization](../../../../../non-renormalization-theorem.md). Promote every coupling in $W_{\rm tree}=\sum_A\lambda_A\mathcal O_A(\Phi)$ to a background [chiral superfield](../../../../../chiral-superfield.md), or [spurion](../../../../../spurion.md). A local [F-term](../../../../../f-term.md) must remain chiral for arbitrary backgrounds, so its coefficient is holomorphic in $\Phi$ and the $\lambda_A$, not in their complex conjugates. Give the matter superfields formal [R-charge](../../../../../r-charge.md) zero, $\theta$ charge one, and every $\lambda_A$ charge two. The superpotential then has charge two. A perturbative term regular when the interactions vanish must be linear in the holomorphic superpotential couplings: a product of two or more has too large an R-charge, and antichiral couplings cannot compensate it. Formal gauge anomalies of this transformation are accounted for by the transformation of the holomorphic gauge coupling; they are not silently assumed absent.

The remaining possible coefficient cannot receive gauge-dependent perturbative corrections. The [holomorphic gauge coupling](../../../../../holomorphic-gauge-coupling.md) may be written $S=g_h^{-2}-i\vartheta/(8\pi^2)$. Perturbation theory is insensitive to the topological angle, so any ordinary superpotential coefficient is invariant under $S\mapsto S+ic$, with real $c$. A holomorphic function with this continuous imaginary-shift invariance is constant in $S$ by the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md). This is [perturbative gauge-coupling independence of the Wilsonian superpotential](../../../../../perturbative-gauge-coupling-independence-of-the-wilsonian-superpotential.md).

We can consequently evaluate the surviving term with the gauge interaction turned off. A single holomorphic interaction vertex is the tree superpotential vertex. It cannot make a loop using free $\Phi$-$\Phi^\dagger$ propagators without additional vertices and antichiral couplings. Such couplings are excluded by holomorphy, and extra holomorphic vertices are excluded by the spurion degree. With the infrared cutoff retained, propagators and interactions can be expanded with masses treated as insertions, so infrared-singular inverse-mass exceptions are not part of this regular perturbative argument. The coefficient must therefore equal its tree value. This proves the [spurion selection rule for perturbative non-renormalization](../../../../../spurion-selection-rule-for-perturbative-non-renormalization.md) for arbitrary superpotential monomials.

Now prove [one-loop exactness of the holomorphic gauge kinetic function](../../../../../one-loop-exactness-of-the-holomorphic-gauge-kinetic-function.md). Add an independent constant background coupling $S$ to the gauge kinetic function. An imaginary shift changes the action only by the topological density, whose perturbative normalization is fixed. Thus the holomorphic perturbative coefficient transforms as

$$
f_{\rm pert}(S+ic)=f_{\rm pert}(S)+ic.
$$

Differentiating with respect to $c$ gives $\partial_Sf_{\rm pert}=1$. Therefore the correction $f_{\rm pert}-S$ is independent of $S$; nonlinear inverse powers of $\operatorname{Re}S$ cannot be holomorphic shift-invariant corrections. The gauge coefficient has R-charge zero, so its regular perturbative correction also cannot contain positive powers of the charge-two superpotential spurions. The anomalous shift of $S$ accounts for the allowed one-loop anomaly; it does not permit arbitrary higher-loop spurion dependence.

To connect this constraint to loop order, use gauge fields whose bare kinetic term has coefficient $1/g_h^2$. After factoring this tree normalization, an $L$-loop gauge-kinetic correction scales as $g_h^{2L-2}$. Equivalently, a gauge propagator contributes $S^{-1}$ and a pure-gauge vertex contributes $S$; with no superpotential interactions, closed matter lines give equal numbers of matter propagators and matter vertices. The connected graph identity $L=I-V+1$ then gives $S^{1-L}$ for the gauge coefficient. Tree order is linear in $S$, one loop is independent of $S$, and every higher loop has forbidden inverse-coupling dependence. Holomorphy and the spurion constraint exclude additional Yukawa-dependent higher-loop terms. Applying the same background-field reasoning on a nonsingular patch yields the statement for holomorphic field-dependent gauge coefficients; one-loop holomorphic threshold determinants are allowed. Thus the only perturbative correction to $f$ is the one-loop correction.

For one simple gauge factor with $\operatorname{tr}_R(T_aT_b)=T(R)\delta_{ab}$, the [one-loop beta function of a supersymmetric gauge theory](../../../../../one-loop-beta-function-of-a-supersymmetric-gauge-theory.md) has $b_0=3C_2(G)-\sum_iT(R_i)$. The vector and adjoint Weyl contributions give $(11/3-2/3)C_2(G)=3C_2(G)$, while one matter Weyl fermion and complex scalar contribute $-(2/3+1/3)T(R)=-T(R)$. Consequently, away from thresholds,

$$
\boxed{f(\mu)=f(M)+\frac{b_0}{8\pi^2}\log\frac\mu M,\qquad\mu\frac{df}{d\mu}=\frac{b_0}{8\pi^2}.}
$$

This sign makes the real inverse coupling decrease toward the infrared in an asymptotically free theory.

Finally, [holomorphic and canonically normalized superpotential couplings](../../../../../holomorphic-and-canonically-normalized-superpotential-couplings.md) are different. For example, if $K=Z\Phi^\dagger\Phi$, then $\Phi_c=Z^{1/2}\Phi$ changes $m\Phi^2/2+y\Phi^3/3$ to coefficients $m/Z$ and $y/Z^{3/2}$. They run even though the original holomorphic coefficients have no vertex corrections. Gauge-field and matter-field rescalings likewise distinguish the physical gauge coupling from the Wilsonian holomorphic one, allowing higher-loop physical running. Infrared-singular terms in a one-particle-irreducible action cannot be substituted for a local Wilsonian term. Nonperturbative terms such as $e^{-8\pi^2S}$ evade continuous topological-angle shift invariance and may generate superpotentials or gauge-kinetic effects when the symmetries and dynamics permit them. These qualifications are essential to the theorem's statement.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
