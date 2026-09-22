<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The homogeneous [fixed point](../../../../../fixed-point.md) must satisfy $v=u^2$. The singular point $u=v=0$ is outside the domain of the reaction term, so substitution in the other equation gives the unique regular [spatially homogeneous equilibrium](../../../../../spatially-homogeneous-equilibrium.md)

$$
\boxed{u_*=1+r,\qquad v_*=(1+r)^2.}
$$

This is the [basally forced quadratic activator-inhibitor model](../../../../../basally-forced-quadratic-activator-inhibitor-model.md). The [linearization](../../../../../linearization.md) of its reaction terms gives the [Jacobian matrix](../../../../../jacobian-matrix.md)

$$
J=\begin{pmatrix}\dfrac{r-1}{r+1}&-\dfrac{r}{(1+r)^2}\\2q(1+r)&-q\end{pmatrix}.
$$

Put $a=(r-1)/(r+1)$, so $-1<a<1$. Its [trace](../../../../../matrix-trace.md) and [determinant](../../../../../determinant.md) are $a-q$ and $q$, and its [eigenvalues](../../../../../eigenvalue.md) are

$$
\lambda_\pm=\frac{a-q\pm\sqrt{(a-q)^2-4q}}2.
$$

Since $q>0$, both [eigenvalues](../../../../../eigenvalue.md) have negative real part exactly when $q>a$. Hence

$$
\boxed{q>\frac{r-1}{r+1}:\text{ linearly asymptotically stable};\qquad 0<q<\frac{r-1}{r+1}:\text{ unstable}.}
$$

For $r\leq1$ the equilibrium is always strictly linearly stable. For $r>1$, equality $q=a$ is an oscillatory threshold with $\lambda_\pm=\pm i\sqrt a$; the nonlinear qualification at this threshold is proved below.

Now insert a perturbation proportional to $e^{\lambda t+ikx}$. The [diffusion](../../../../../diffusion.md) terms subtract $k^2\operatorname{diag}(1,p)$ from $J$. With $s=k^2$ the mode [trace](../../../../../matrix-trace.md) and [determinant](../../../../../determinant.md) are

$$
\tau(s)=a-q-(1+p)s,\qquad \Delta(s)=ps^2+(q-pa)s+q.
$$

For a strictly stable homogeneous state, $q>a$ makes $\tau(s)<0$ for all $s\geq0$. A nonzero [Fourier mode](../../../../../fourier-mode.md) can therefore grow only if $\Delta(s)<0$, in which case its two real [eigenvalues](../../../../../eigenvalue.md) have opposite signs. The [determinant](../../../../../determinant.md) parabola has its minimum at $s_*=(pa-q)/(2p)$, and that minimum is $q-(pa-q)^2/(4p)$. The [two-species Turing criterion](../../../../../two-species-diffusion-driven-instability-criterion.md) is consequently derived here as

$$
\boxed{q>a,\qquad pa>q,\qquad (pa-q)^2>4pq.}
$$

These force $a>0$, hence $r>1$. Equivalently, solving $pa-q>2\sqrt{pq}$ for $\sqrt p$ gives

$$
\boxed{r>1,\qquad q>a,\qquad p>p_c=\frac{q}{(\sqrt{1+a}-1)^2}.}
$$

Thus the [inhibitor in a reaction-diffusion system](../../../../../inhibitor-in-a-reaction-diffusion-system.md) must diffuse sufficiently fast. Inside this region, the growing [wavenumbers](../../../../../wavenumber.md) obey

$$
s_-<k^2<s_+,\qquad s_\pm=\frac{pa-q\pm\sqrt{(pa-q)^2-4pq}}{2p}.
$$

At onset, the minimum touches zero and the two [determinant](../../../../../determinant.md) roots coalesce. Therefore

$$
\boxed{k_c^2=\frac{pa-q}{2p}=\sqrt{\frac qp},\qquad \lambda_c=\frac{2\pi}{k_c}=2\pi\left(\frac pq\right)^{1/4}.}
$$

Here $p$ is evaluated on the onset surface. These are the [Turing threshold of a basally forced quadratic activator-inhibitor model](../../../../../turing-threshold-of-a-basally-forced-quadratic-activator-inhibitor-model.md) and its continuum critical [wavelength](../../../../../wavelength.md). On a finite or domain with [periodic boundary conditions](../../../../../periodic-boundary-conditions.md) an admissible nonzero spatial mode must additionally fall in the stated band. Equality in the [diffusion](../../../../../diffusion.md) criterion is marginal onset, while $q=a$ is the distinct homogeneous oscillatory threshold.

For completeness, the [weak focus at the Hopf threshold of a basal activator-inhibitor model](../../../../../weak-focus-at-the-hopf-threshold-of-a-basal-activator-inhibitor-model.md) resolves the nonlinear homogeneous stability when $q=a>0$. Let $h=(1+a)/2$, $\beta=(1-a)/2$, $\omega=\sqrt a$, and set $u=(1+r)(1+x)$, $v=(1+r)^2(1+y)$, $X=x$, $Y=(hy-a x)/\omega$. Expanding the rational reaction term to cubic order gives

$$
\dot X=-\omega Y+F_2+F_3+O(4),\qquad\dot Y=\omega X+G_2+G_3+O(4),
$$

where

$$
F_2=\frac{(\beta X-\omega Y)^2}{h},\quad F_3=-\frac{(aX+\omega Y)(\beta X-\omega Y)^2}{h^2},\quad G_2=\omega(hX^2-F_2),\quad G_3=-\omega F_3.
$$

Write $X=\varrho\cos\theta$, $Y=\varrho\sin\theta$ and evaluate these [homogeneous polynomials](../../../../../homogeneous-polynomial.md) on the [unit circle](../../../../../complex-unit-circle.md). If $A=\cos\theta F_2+\sin\theta G_2$, $B=\cos\theta F_3+\sin\theta G_3$, and $C=\cos\theta G_2-\sin\theta F_2$, division of the radial and angular equations gives

$$
\frac{d\varrho}{d\theta}=\frac A\omega\varrho^2+\left(\frac B\omega-\frac{AC}{\omega^2}\right)\varrho^3+O(\varrho^4).
$$

The angular integral of $A$ is zero because it changes sign under $\theta\mapsto\theta+\pi$. Iterating its quadratic term once over a full cycle contributes the square of this zero integral, so the first nonzero [return map](../../../../../poincare-map.md) term is cubic. Using $\langle\cos^4\theta\rangle=3/8$, $\langle\cos^2\theta\sin^2\theta\rangle=1/8$ and the corresponding sixth moments gives $\langle B\rangle=a/4$ and $\langle AC\rangle/\omega=(a+1)/8$. The [Poincaré map](../../../../../poincare-map.md) is

$$
\varrho\longmapsto\varrho+\frac{2\pi}{\omega}\frac{a-1}{8}\varrho^3+O(\varrho^4).
$$

Because $0<a<1$, sufficiently small positive radii decrease on every return. The equilibrium at $q=a$ is therefore **nonlinearly asymptotically stable, with weak rather than exponential attraction**, despite its neutral linear [eigenvalues](../../../../../eigenvalue.md). The strict inequalities above describe the ordinary [diffusion](../../../../../diffusion.md)-driven instability from a strictly linearly stable homogeneous state.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
