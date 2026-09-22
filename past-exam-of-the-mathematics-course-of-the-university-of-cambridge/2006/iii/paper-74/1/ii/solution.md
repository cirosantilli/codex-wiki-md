<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $N=\int_VP^2\,dV$, $D=\int_{\mathbb R^3}|\nabla P|^2\,dV$, $M=\int_{\mathbb R^3}|\mathbf B|^2\,dV$, and $q=\max_V|Q|$. The confined flow satisfies the [impermeability condition](../../../../../../no-penetration-boundary-condition.md) $\mathbf u\cdot\mathbf n=0$, so $Q=0$ at $r=a$. Multiplying the [radial magnetic induction scalar](../../../../../../radial-magnetic-induction-scalar.md) equation by $P$ and integrating, the [advection](../../../../../../advection.md) term vanishes by the [divergence theorem](../../../../../../divergence-theorem.md):

$$
\int_VP\,\mathbf u\cdot\nabla P\,dV=\frac12\int_{\partial V}P^2\mathbf u\cdot\mathbf n\,dS=0.
$$

The same [integration by parts](../../../../../../integration-by-parts.md), using $\nabla\cdot\mathbf B=0$, gives

$$
\int_VP\,\mathbf B\cdot\nabla Q\,dV
=\int_{\partial V}PQ\,\mathbf B\cdot\mathbf n\,dS-\int_VQ\,\mathbf B\cdot\nabla P\,dV
=-\int_VQ\,\mathbf B\cdot\nabla P\,dV.
$$

For diffusion, [Green's first identity](../../../../../../green-s-first-identity.md) in the sphere gives $\int_VP\Delta P=-\int_V|\nabla P|^2+\int_{\partial V}P\partial_rP$. In the exterior, $\Delta P=0$ and the normal on its inner boundary is $-\hat{\mathbf r}$, so

$$
\int_{\mathbb R^3\setminus V}|\nabla P|^2\,dV=-\int_{\partial V}P\partial_rP\,dS.
$$

The infinity term vanishes for the isolated decaying field. The [insulating boundary condition for the radial magnetic scalar](../../../../../../insulating-boundary-condition-for-the-radial-magnetic-scalar.md) permits matching the two traces, and therefore the exterior contribution is essential: it turns the diffusive term into $-\eta D$. Altogether,

$$
\frac12N'=-\int_VQ\,\mathbf B\cdot\nabla P\,dV-\eta D
\leq q\int_{\mathbb R^3}|\mathbf B\cdot\nabla P|\,dV-\eta D.
$$

Applying the pointwise [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and then its integral version,

$$
\int_{\mathbb R^3}|\mathbf B\cdot\nabla P|
\leq\int_{\mathbb R^3}|\mathbf B||\nabla P|
\leq\sqrt{MD},
\qquad
\frac12N'\leq q\sqrt{MD}-\eta D.
$$

Thus a nonzero field with stationary or growing $N$ must satisfy the [radial-flow dynamo energy bound](../../../../../../radial-flow-dynamo-energy-bound.md):

$$
\boxed{(\max_V|Q|)^2\geq\eta^2
\frac{\displaystyle\int_{\mathbb R^3}|\nabla P|^2\,dV}
{\displaystyle\int_{\mathbb R^3}|\mathbf B|^2\,dV}.}
$$

The temporal qualification matters. For general time-dependent [dynamo action](../../../../../../dynamo-action.md), nondecay does not make $N'\geq0$ at every instant; the boxed bound applies at nondecreasing instants, to a marginal or growing mode, or in an appropriate long-time sense. A uniform strict violation, $q\sqrt{M/D}\leq\eta-\varepsilon$ with $\varepsilon>0$, gives $N'\leq-2\varepsilon D$. The whole-space [Sobolev inequality](../../../../../../sobolev-inequality.md) and [Holder inequality](../../../../../../holder-inequality.md) give $N\leq |V|^{2/3}\|P\|_6^2\leq C_aD$, forcing exponential decay of $N$. Alternatively, for a bounded statistically steady field, time averaging the energy balance and applying [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) once more gives $q_*^2\geq\eta^2\langle D\rangle/\langle M\rangle$, where $q_*=\sup_tq(t)$. Sustained [dynamo action](../../../../../../dynamo-action.md) cannot have a uniform negative dissipation gap.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
