<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [orthonormal coframe](../../../../../orthonormal-coframe-in-spacetime.md) is a collection of independent [differential forms](../../../../../differential-form-split.md) $E^{\hat a}=e^{\hat a}{}_\mu dx^\mu$ satisfying $g_{\mu\nu}=\eta_{\hat a\hat b}e^{\hat a}{}_\mu e^{\hat b}{}_\nu$, with $\eta=\operatorname{diag}(-1,1,1,1)$. Locally one can diagonalize the [metric tensor](../../../../../metric-tensor.md) and rescale the resulting covectors, or use [Gram-Schmidt orthogonalization for a symmetric bilinear form](../../../../../gram-schmidt-orthogonalization-for-a-symmetric-bilinear-form.md), choosing a timelike direction first. The coframe is not unique: a local Lorentz transformation preserves the metric. For the [Levi-Civita connection](../../../../../levi-civita-connection.md), solve [Cartan's first structure equation](../../../../../cartan-s-first-structure-equation.md) and metric compatibility together:

$$
dE^{\hat a}+\omega^{\hat a}{}_{\hat b}\wedge E^{\hat b}=0,\qquad
\omega_{\hat a\hat b}=\eta_{\hat a\hat c}\omega^{\hat c}{}_{\hat b}=-\omega_{\hat b\hat a}.
$$

These determine the [connection 1-forms](../../../../../connection-1-form-split.md). The antisymmetry applies to the lowered pair of indices; a mixed time-space pair instead has $\omega^0{}_i=\omega^i{}_0$. Next [Cartan's second structure equation](../../../../../cartan-s-second-structure-equation.md) gives the [curvature 2-forms](../../../../../curvature-2-form.md), and reading off their coefficients determines the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md):

$$
\Omega^{\hat a}{}_{\hat b}=d\omega^{\hat a}{}_{\hat b}+\omega^{\hat a}{}_{\hat c}\wedge\omega^{\hat c}{}_{\hat b}
=\frac12R^{\hat a}{}_{\hat b\hat c\hat d}E^{\hat c}\wedge E^{\hat d},\qquad
R_{\hat b\hat d}=R^{\hat a}{}_{\hat b\hat a\hat d}.
$$

This also states the curvature-sign convention. Contracting gives the [Ricci tensor](../../../../../ricci-tensor.md), and its coordinate components are $R_{\mu\nu}=e^{\hat a}{}_\mu e^{\hat b}{}_\nu R_{\hat a\hat b}$.

On a static patch with $V>0$, choose

$$
E^0=\sqrt V\,dt,\quad E^1=\frac{dr}{\sqrt V},\quad E^2=r\,d\theta,\quad E^3=r\sin\theta\,d\phi.
$$

Write $h=\sqrt V$, $a=h'$, $b=h/r$, and $c=\cot\theta/r$. The [exterior derivative](../../../../../exterior-derivative.md) gives

$$
dE^0=-aE^0\wedge E^1,\qquad dE^1=0,\qquad
dE^2=bE^1\wedge E^2,\qquad dE^3=bE^1\wedge E^3+cE^2\wedge E^3.
$$

The nonzero independent [connection 1-forms](../../../../../connection-1-form-split.md) are consequently

$$
\omega^0{}_1=aE^0,\qquad \omega^1{}_2=-bE^2,\qquad
\omega^1{}_3=-bE^3,\qquad \omega^2{}_3=-cE^3,
$$

with $\omega^1{}_0=\omega^0{}_1$, spatial mixed pairs antisymmetric, and the remaining forms zero. For example,

$$
\Omega^0{}_1=d(aE^0)=-(hh''+h'^2)E^0\wedge E^1=-\frac{V''}2E^0\wedge E^1.
$$

Similarly $\Omega^0{}_2=\omega^0{}_1\wedge\omega^1{}_2=-abE^0\wedge E^2$, and the angular derivatives in $d\omega^1{}_3$ cancel against $\omega^1{}_2\wedge\omega^2{}_3$. The resulting [Cartan curvature forms for a static spherical metric](../../../../../cartan-curvature-forms-for-a-static-spherical-metric.md) are

$$
\boxed{\begin{aligned}
\Omega^0{}_1&=-\frac{V''}2E^0\wedge E^1,\\
\Omega^0{}_2&=-\frac{V'}{2r}E^0\wedge E^2,&\Omega^0{}_3&=-\frac{V'}{2r}E^0\wedge E^3,\\
\Omega^1{}_2&=-\frac{V'}{2r}E^1\wedge E^2,&\Omega^1{}_3&=-\frac{V'}{2r}E^1\wedge E^3,\\
\Omega^2{}_3&=\frac{1-V}{r^2}E^2\wedge E^3.
\end{aligned}}
$$

For the last entry, $d(-cE^3)=E^2\wedge E^3/r^2$ and $\omega^2{}_1\wedge\omega^1{}_3=-VE^2\wedge E^3/r^2$. The remaining [curvature 2-forms](../../../../../curvature-2-form.md) follow from $\Omega_{ab}=-\Omega_{ba}$.

Put $A=V''/2$, $B=V'/(2r)$, and $C=(1-V)/r^2$. Reading the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) from the forms and contracting gives the diagonal orthonormal [Ricci tensor](../../../../../ricci-tensor.md)

$$
\boxed{R_{\hat a\hat b}=\operatorname{diag}(A+2B,-A-2B,C-2B,C-2B).}
$$

For example $R_{00}=R^1{}_{010}+R^2{}_{020}+R^3{}_{030}=A+2B$, while $R_{22}=-B-B+C$. All off-diagonal entries vanish because the [curvature 2-forms](../../../../../curvature-2-form.md) only involve their own index planes. In the coordinate basis the nonzero components are

$$
\boxed{\begin{aligned}
R_{tt}&=V\left(\frac{V''}2+\frac{V'}r\right),&
R_{rr}&=-\frac1V\left(\frac{V''}2+\frac{V'}r\right),\\
R_{\theta\theta}&=1-V-rV',&
R_{\phi\phi}&=(1-V-rV')\sin^2\theta.
\end{aligned}}
$$

The angular [Einstein field equations](../../../../../einstein-field-equations.md) with the negative [cosmological constant](../../../../../cosmological-constant.md) give $(rV)'=1+3r^2/l^2$. Integrating introduces one real constant, conventionally written $-2m$:

$$
\boxed{V(r)=1-\frac{2m}{r}+\frac{r^2}{l^2}.}
$$

Substitution gives $V''/2+V'/r=3/l^2$, so the time and radial [Einstein field equations](../../../../../einstein-field-equations.md) hold as well. The solution is the [Schwarzschild--anti-de Sitter black hole](../../../../../schwarzschild-anti-de-sitter-black-hole.md) family, including its zero and negative mass limits.

For $m>0$, $V$ increases strictly from $-\infty$ at $r=0$ to $+\infty$ at infinity. Its unique positive simple zero $r_h$ satisfies $r_h^3+l^2r_h=2ml^2$. This zero is a [coordinate singularity](../../../../../coordinate-singularity.md), not a curvature singularity: with the ingoing coordinate $v=t+\int dr/V$, the radial metric is $-Vdv^2+2dv\,dr$ and is regular there. Inside the future black-hole region, $\nabla r=\partial_v+V\partial_r$ is future timelike, so every future-directed causal trajectory decreases $r$ and cannot return to the asymptotic anti-de Sitter boundary. Conversely, every exterior radius admits an outward [radial null geodesic](../../../../../radial-null-geodesic.md) reaching that boundary, since $\int_r^\infty dr/V$ converges. Thus **$m>0$ gives an event horizon at the unique positive zero of $V$**. Here the [event horizon](../../../../../event-horizon.md) is defined relative to the asymptotic timelike boundary of [Anti-de Sitter spacetime](../../../../../anti-de-sitter-spacetime.md). For $m=0$, $V=1+r^2/l^2>0$ and the spacetime is pure [Anti-de Sitter spacetime](../../../../../anti-de-sitter-spacetime.md), with **no black-hole event horizon**. For $m<0$, $V=1+2|m|/r+r^2/l^2>0$, so there is also **no event horizon**; the mass term produces a [naked singularity](../../../../../naked-singularity.md) at $r=0$. The field equation itself does not impose a positive mass integration constant.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
