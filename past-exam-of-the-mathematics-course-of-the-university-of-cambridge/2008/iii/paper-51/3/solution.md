<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [renormalizable quantum field theory](../../../../../renormalizable-quantum-field-theory.md) requires only finitely many independent field and parameter redefinitions to remove regulator dependence from its perturbative [correlation functions](../../../../../correlation-function.md), order by order. The allowed local [counterterms](../../../../../counterterm.md) must close within that finite set; it is not necessary that the unrenormalized integrals be finite.

In four spacetime dimensions the [kinetic term](../../../../../kinetic-term.md) fixes the [mass dimension](../../../../../mass-dimension.md) of $\phi$ to one. A coefficient multiplying $\phi^k$ therefore has dimension $4-k$. [Power counting](../../../../../power-counting-in-quantum-field-theory.md) excludes couplings of negative [mass dimension](../../../../../mass-dimension.md) for perturbative renormalizability. For a single scalar with a conventional nonderivative [polynomial](../../../../../polynomial-split.md) potential, the allowed form is

$$
\boxed{V(\phi)=v_0+h\phi+\frac12m^2\phi^2+\frac{\lambda_3}{3!}\phi^3+\frac{\lambda_4}{4!}\phi^4.}
$$

The constant controls vacuum energy and the linear term a possible tadpole. A field-reflection symmetry can remove the odd terms but is not necessary for renormalizability. Terms of degree above four generally require an infinite tower of [counterterms](../../../../../counterterm.md) when treated as fundamental interactions; they can instead be used in an [effective field theory](../../../../../effective-field-theory.md). Stability of the potential is a separate requirement, for example a positive quartic leading term, and should not be confused with the power-counting criterion.

For a graph with $E$ external scalar lines, $I$ internal lines, $L$ loops and $V_k$ vertices of degree $k$, the superficial [ultraviolet divergence](../../../../../ultraviolet-divergence.md) degree is $\omega=4L-2I$. The identities $L=I-\sum_kV_k+1$ and $2I+E=\sum_k kV_k$ give

$$
\omega=4-E+\sum_k(k-4)V_k.
$$

When every $k\le4$, only the finitely many low-point local divergences, including the [kinetic term](../../../../../kinetic-term.md), can require subtraction. Subdivergences are removed recursively by the same local [counterterms](../../../../../counterterm.md). A vertex with $k>4$ instead permits arbitrarily high divergence degrees as more such vertices are added. This explains the restriction rather than merely asserting it.

The bare [Lagrangian density](../../../../../lagrangian-density.md) is written in terms of regulator-dependent bare quantities, before taking the regulator away:

$$
\mathcal L_B=-\frac12(\partial\phi_B)^2-V_B(\phi_B),\qquad\phi_B=Z_\phi^{1/2}\phi,\qquad\mathcal L_B=\mathcal L_R+\mathcal L_{\mathrm{ct}}.
$$

The coefficients in $V_B$ are related to the [renormalized](../../../../../renormalization.md) parameters by regulator-dependent redefinitions. The [wave-function renormalization](../../../../../wave-function-renormalization.md) supplies a kinetic [counterterm](../../../../../counterterm.md). In [dimensional regularization](../../../../../dimensional-regularization.md) $d=4-\epsilon$, a quartic coupling has a bare relation of the form $\lambda_B=\mu^\epsilon[\lambda+\delta\lambda(\lambda,\epsilon)]$, with field factors incorporated according to the chosen definition. The bare parameters and bare [correlation functions](../../../../../correlation-function.md) are held fixed when changing the [renormalization scale](../../../../../renormalization-scale.md).

Even without a physical [mass](../../../../../mass.md), interacting loop subtractions require a reference scale $\mu$ to define the [renormalized](../../../../../renormalization.md) dimensionless coupling and field normalization. Finite logarithms then involve dimensionless combinations such as $\mu|x_r-x_s|$ or $p^2/\mu^2$. This scale is a subtraction convention, not a new physical [mass](../../../../../mass.md) parameter. Its explicit dependence is compensated by the [running coupling](../../../../../running-coupling.md) and field normalization.

Let $G_n=\langle\phi(x_1)\cdots\phi(x_n)\rangle$ at separated points. Its bare counterpart satisfies $G_{B,n}=Z_\phi^{n/2}G_n$. Define

$$
\beta(g)=\left.\mu\frac{dg}{d\mu}\right|_{\mathrm{bare}},\qquad\gamma(g)=\left.\frac12\mu\frac{d\log Z_\phi}{d\mu}\right|_{\mathrm{bare}}.
$$

Differentiating $G_{B,n}$ at fixed bare theory gives

$$
\boxed{\left(\mu\partial_\mu+\beta(g)\partial_g+n\gamma(g)\right)G_n=0.}
$$

This [Callan-Symanzik equation](../../../../../callan-symanzik-equation.md) expresses independence of the arbitrary subtraction scale. The [renormalization-group beta function](../../../../../beta-function-physics.md) describes the compensating coupling change; the [field-renormalization anomalous dimension](../../../../../field-renormalization-anomalous-dimension.md) describes the compensating rescaling of each insertion. Coincident composite insertions would require their own additional [renormalization](../../../../../renormalization.md), rather than automatically obeying this separated-point equation.

For the two-point function, set $z=p^2/\mu^2$ and $t=\tfrac12\log z$. We consider large positive spacelike $p^2$, with continuation to other momenta as required. The dimensionless [propagator](../../../../../propagator.md) factor obeys

$$
(-\partial_t+\beta\partial_g+2\gamma)d(e^{2t},g)=0.
$$

Define $\bar g(0)=g$ and $d\bar g/dt=\beta(\bar g)$. The [renormalization-group characteristic solution for a two-point function](../../../../../renormalization-group-characteristic-solution-for-a-two-point-function.md) is

$$
\boxed{d(e^{2t},g)=d(1,\bar g(t))\exp\left\{2\int_0^t\gamma(\bar g(s))\,ds\right\}.}
$$

To verify it, the running-coupling flow has $\beta(g)\partial_g\bar g(t)=\beta(\bar g(t))$. Also, $\beta(g)\partial_g\int_0^t\gamma(\bar g(s))ds=\gamma(\bar g(t))-\gamma(g)$. Applying $\partial_t-\beta(g)\partial_g$ to the displayed expression therefore gives $2\gamma(g)d$, exactly the required differential equation. The boundary value $d(1,g)$ records the [renormalization](../../../../../renormalization.md) condition. This shows how the ultraviolet behaviour is determined by the coupling trajectory and its accumulated [anomalous dimension](../../../../../anomalous-dimension.md): it can approach zero coupling, a nonzero fixed point, or a finite-scale singularity, depending on $\beta$.

For $\beta=-bg^3$ with $b>0$, direct integration gives

$$
\bar g(t)^2=\frac{g^2}{1+2bg^2t},\qquad2\int_0^t c\bar g(s)^2\,ds=\frac cb\log(1+2bg^2t).
$$

Consequently

$$
\boxed{d(z,g)=d\left(1,\frac{g}{\sqrt{1+bg^2\log z}}\right)\left(1+bg^2\log z\right)^{c/b}.}
$$

For a regular free-theory normalization $d(1,0)=1$, the leading large-$z$ form is $(1+bg^2\log z)^{c/b}$, times corrections from the small [running coupling](../../../../../running-coupling.md). This is [asymptotic freedom](../../../../../asymptotic-freedom.md) with a logarithmic, rather than a fixed-power, [propagator](../../../../../propagator.md) correction. The hypothetical beta and gamma functions are being used as given; this calculation does not assert that they are the actual beta and gamma functions of an arbitrary quartic scalar theory.

For the second beta function put $B=-b>0$, so $\beta(g)=Bg^3-ag^5$. Its positive nonzero fixed point and linearized slope are

$$
\boxed{g_*^2=\frac{B}{a}=-\frac ba,\qquad\beta^{\prime}(g_*)=-\frac{2B^2}{a}<0.}
$$

For $0<g<g_*$ the coupling increases with momentum, while for $g>g_*$ it decreases; each positive trajectory approaches $g_*$ in the ultraviolet. Negative initial couplings approach $-g_*$ by the odd symmetry of the beta function, with the same limiting squared coupling. The exactly zero trajectory remains zero. Thus the [nonzero ultraviolet fixed point of a cubic-quintic beta function](../../../../../nonzero-ultraviolet-fixed-point-of-a-cubic-quintic-beta-function.md) replaces asymptotic freedom by a finite-coupling ultraviolet limit, with $\bar g(t)-g_*=O(e^{-2B^2t/a})$. If the [anomalous dimension](../../../../../anomalous-dimension.md) is regular there, the [propagator](../../../../../propagator.md) factor has fixed-point behaviour $d(z,g)\sim A(g)z^{\gamma(g_*)}$ when its fixed-point boundary value is nonzero. If $\gamma(g)=cg^2$ is retained, the exponent is $\gamma(g_*)=-cb/a$. Trusting this perturbative truncation as a statement about the underlying theory requires $g_*$ to be sufficiently small; the flow result itself follows from the specified beta function.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
