<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For this question use the [Levi-Civita connection](../../../levi-civita-connection.md), its [metric compatibility](../../../metric-compatibility.md) and the usual [curvature](../../../curvature.md) symmetries. In the index ordering of Question 1, put $R_{\mu\nu\rho\sigma}=g_{\sigma\lambda}R_{\mu\nu\rho}{}^\lambda$ and $R_{\nu\rho}=g^{\mu\sigma}R_{\mu\nu\rho\sigma}$. Contract the [second Bianchi identity](../../../second-bianchi-identity.md) in its derivative index $\mu$ and [curvature](../../../curvature.md) index $\rho$. The [curvature](../../../curvature.md) symmetries give

$$
\nabla^\rho R_{\nu\lambda\rho\sigma}
=\nabla_\lambda R_{\nu\sigma}-\nabla_\nu R_{\lambda\sigma}.
$$

Now contract $\lambda,\sigma$. The left-hand side becomes $-\nabla^\rho R_{\nu\rho}$, while the right-hand side becomes $\nabla^\sigma R_{\nu\sigma}-\nabla_\nu R$. Thus

$$
2\nabla^\mu R_{\mu\nu}=\nabla_\nu R.
$$

Using $\nabla g=0$ yields the [contracted Bianchi identity](../../../contracted-bianchi-identity.md)

$$
\boxed{\nabla^\mu G_{\mu\nu}=0,\qquad
G_{\mu\nu}=R_{\mu\nu}-\tfrac12g_{\mu\nu}R.}
$$

Taking the [covariant divergence](../../../covariant-divergence.md) of the [Einstein field equations](../../../einstein-field-equations-split.md), with constant $G$, then gives $8\pi G\nabla^\mu T_{\mu\nu}=0$. The matter equation is therefore consistent with the geometric identity rather than imposing an extra incompatible condition on the metric.

[Stress-energy conservation](../../../stress-energy-conservation.md) expresses the local balance of [energy](../../../energy-split.md) and [momentum](../../../momentum-split.md), including their transport and the effects of the gravitational [Levi-Civita connection](../../../levi-civita-connection.md). In a freely falling frame at a point it reduces there to the familiar ordinary divergence law. A global conserved [energy](../../../energy-split.md) requires additional geometric structure, such as a timelike [Killing vector field](../../../killing-vector-field-split.md); it does not follow in an arbitrary [spacetime](../../../spacetime.md) just by replacing a [covariant derivative](../../../covariant-derivative.md) with an ordinary derivative.

For [relativistic dust](../../../relativistic-dust.md),

$$
0=\nabla_\mu(\rho u^\mu u^\nu)
=u^\nu\nabla_\mu(\rho u^\mu)+\rho u^\mu\nabla_\mu u^\nu.
$$

With signature $(+,-,-,-)$, $u^\nu u_\nu=1$ implies $u_\nu u^\mu\nabla_\mu u^\nu=0$. Contracting gives $\nabla_\mu(\rho u^\mu)=0$; where $\rho>0$, substitution then gives $u^\mu\nabla_\mu u^\nu=0$. Thus the continuity law combines rest-[mass](../../../mass.md) conservation and free [geodesic](../../../geodesic.md) motion for this matter model.

For the [Newtonian limit](../../../newtonian-limit.md), take $c=1$ and $\eta=\operatorname{diag}(1,-1,-1,-1)$, consistently with Question 3. Use the static weak field sourced by the time-independent, slowly moving matter, retaining first order in $\epsilon$ and leading order in the spatial speed. Write spatial gradients with $\partial^i=\delta^{ij}\partial_j$ here; these are Euclidean spatial indices in the Newtonian equation. The [Levi-Civita connection](../../../levi-civita-connection.md) formula gives

$$
\Gamma_{00}{}^i=-\tfrac12\eta^{ij}\partial_j(\epsilon h_{00})
=\frac\epsilon2\delta^{ij}\partial_jh_{00}.
$$

The exact change from [proper time](../../../proper-time.md) to $t$ in the spatial [geodesic equation](../../../geodesic-equation.md) is

$$
\frac{d^2x^i}{dt^2}
=-\Gamma_{\alpha\beta}{}^i v^\alpha v^\beta
+\Gamma_{\alpha\beta}{}^0v^\alpha v^\beta v^i,\qquad v^0=1.
$$

Terms containing spatial velocities are negligible at leading order, leaving

$$
\boxed{\frac{d^2x^i}{dt^2}=-\partial^i\Phi,\qquad
\Phi=\frac\epsilon2h_{00}.}
$$

An additive constant in $\Phi$ is immaterial to this acceleration and is normally fixed by the asymptotic time normalization. With units restored, $g_{00}=1+2\Phi_{\rm physical}/c^2$.

At the same order, staticity and the [curvature](../../../curvature.md) definition give

$$
R_{00}=\partial_\lambda\Gamma_{00}{}^\lambda
-\partial_0\Gamma_{\lambda0}{}^\lambda+O(\epsilon^2)
=\frac\epsilon2\delta^{ij}\partial_i\partial_jh_{00}
=\nabla^2\Phi.
$$

The trace of the four-dimensional Einstein equations is $R=-8\pi GT$, so their trace-reversed form is

$$
R_{\mu\nu}=8\pi G\left(T_{\mu\nu}-\tfrac12g_{\mu\nu}T\right).
$$

For nonrelativistic dust, $u^0\simeq1$, $u^i\simeq0$, so $T_{00}\simeq\rho$ and $T\simeq\rho$. Keeping leading matter terms therefore gives $R_{00}=4\pi G\rho$. Combining this with the geometric expression yields

$$
\boxed{\nabla^2\Phi=4\pi G\rho.}
$$

This trace reversal is essential: equating $R_{00}$ directly to $8\pi G\rho$ would miss the factor of two. The approximation is the quasistatic Newtonian sector; arbitrary independently imposed gravitational radiation is not part of that sector.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2011](../../2011-split.md)
3. [Past exam of the general relativity course of the University of Oxford](../../split.md)
4. [General relativity course of the University of Oxford](../../../general-relativity-course-of-the-university-of-oxford.md)
5. [Year 3 of the physics course of the University of Oxford](../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
