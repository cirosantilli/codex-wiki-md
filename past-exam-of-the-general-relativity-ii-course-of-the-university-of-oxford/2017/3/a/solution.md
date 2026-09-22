<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A regular [hypersurface](../../../../hypersurface.md) $f=0$, with $df\ne0$, is a [null hypersurface](../../../../null-hypersurface.md) if its normal [covector](../../../../covector.md) has zero squared [norm](../../../../norm.md):

$$
g^{ab}(\partial_af)(\partial_bf)=0\quad\text{on }f=0.
$$

Its normal [vector](../../../../vector.md) is then also tangent to the [hypersurface](../../../../hypersurface.md); the induced [metric tensor](../../../../metric-tensor.md) is degenerate.

For the [Kerr metric](../../../../kerr-metric.md) the normal to a constant-$r$ surface has squared [norm](../../../../norm.md)

$$
g^{rr}=\frac{\Delta}{\Sigma},\qquad
\Delta=(r-r_+)(r-r_-),\qquad
r_\pm=M\pm\sqrt{M^2-a^2}.
$$

For $0<a<M$ the two roots are positive and distinct. To verify that they are genuine regular [null hypersurfaces](../../../../null-hypersurface.md), rather than trusting singular [Boyer-Lindquist coordinates](../../../../boyer-lindquist-coordinates.md), introduce [ingoing Kerr coordinates](../../../../ingoing-kerr-coordinates.md)

$$
dv=dt+\frac{r^2+a^2}{\Delta}\,dr,\qquad
d\psi=d\phi+\frac a\Delta\,dr.
$$

Substitution gives

$$
\begin{aligned}
ds^2={}&-\left(1-\frac{2Mr}{\Sigma}\right)dv^2
+2\,dv\,dr+\Sigma\,d\theta^2
-2a\sin^2\theta\,dr\,d\psi\\
&-\frac{4Mar\sin^2\theta}{\Sigma}\,dv\,d\psi
+\sin^2\theta\left(r^2+a^2+
\frac{2Ma^2r\sin^2\theta}{\Sigma}\right)d\psi^2.
\end{aligned}
$$

There are no $\Delta^{-1}$ terms. At either root $\Sigma>0$, and the [determinant](../../../../determinant.md) is $-\Sigma^2\sin^2\theta$ away from the angular coordinate poles. Thus the [metric tensor](../../../../metric-tensor.md) extends smoothly across each root. The raised normal on either surface is

$$
\left.(d r)^\sharp\right|_{r_\pm}
=\frac{r_\pm^2+a^2}{\Sigma}
\left(\partial_v+\Omega_\pm\partial_\psi\right),
\qquad
\Omega_\pm=\frac{a}{r_\pm^2+a^2}.
$$

This is a nonzero null [Killing vector field](../../../../killing-vector-field-split.md) normal to the surface. Both surfaces are [Killing horizons](../../../../killing-horizon.md), with [horizon angular velocities](../../../../horizon-angular-velocity.md) $\Omega_\pm$.

**The event-horizon terminology in the paper needs qualification.** In the usual asymptotically flat [Kerr black hole](../../../../kerr-black-hole.md) extension, relative to a chosen exterior's [future null infinity](../../../../future-null-infinity.md), the future branch of $r=r_+$ is the [event horizon](../../../../event-horizon.md), the boundary $\partial J^-(\mathscr I^+)$. In the intervening black-hole region $\Delta<0$, the coordinate $r$ has timelike gradient and future-directed curves move toward smaller $r$; they cannot return across the outer boundary to that exterior. The inner surface $r=r_-$ is a [Cauchy horizon](../../../../cauchy-horizon.md), not a second [event horizon](../../../../event-horizon.md) for the same asymptotic end. Nullness is a local property; identifying an [event horizon](../../../../event-horizon.md) additionally requires this global [causal structure](../../../../causal-structure.md).[Sections 6.3.2 and 6.2.4: regular extension across the two Kerr roots, global diagram and the inner Cauchy horizon](../../../../general-relativity-by-david-tong.md)

The allowed endpoint $a=0$ provides an especially concrete counterexample to the unrestricted description of both roots. The [Kerr metric](../../../../kerr-metric.md) then becomes [Schwarzschild spacetime](../../../../schwarzschild-spacetime-split.md), $r_+=2M$ is its regular [event horizon](../../../../event-horizon.md), but $r_-=0$ is a [curvature singularity](../../../../curvature-singularity.md):

$$
R_{abcd}R^{abcd}=\frac{48M^2}{r^6}\longrightarrow\infty.
$$

It is not a regular inner [null hypersurface](../../../../null-hypersurface.md). Thus the two-horizon calculation above assumes $0<a<M$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity II course of the University of Oxford](../../../split.md)
5. [General relativity II course of the University of Oxford](../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
