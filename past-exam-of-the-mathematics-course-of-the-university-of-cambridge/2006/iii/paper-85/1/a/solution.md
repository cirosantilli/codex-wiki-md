<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $S=u^2+v^2$. At a nonzero [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) the two equations form the homogeneous linear system

$$
\begin{pmatrix}\mu-S/2&1-\sigma+S/2\\1+\sigma-S/2&\mu-S/2\end{pmatrix}\binom uv=0.
$$

Its [determinant](../../../../../../determinant.md) must vanish, giving $S^2/2-(\mu+\sigma)S+\mu^2+\sigma^2-1=0$. Thus

$$
\boxed{S=\mu+\sigma\pm\sqrt{2-(\mu-\sigma)^2},\quad S>0.}
$$

Each positive real [polynomial root](../../../../../../root-of-a-polynomial.md) gives an antipodal [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) pair; a negative [polynomial root](../../../../../../root-of-a-polynomial.md) does not describe a real [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md). A direction is specified by $\sin2\theta=S/2-\mu$, $\cos2\theta=S/2-\sigma$, where $u=\sqrt S\cos\theta$, $v=\sqrt S\sin\theta$. This is the [polar form of the cubic confinement model](../../../../../../polar-form-of-the-cubic-confinement-model.md). The origin is always an [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md).

The origin's [eigenvalues](../../../../../../eigenvalue.md) are $\lambda_\pm=\mu\pm\sqrt{1-\sigma^2}$. A simple zero [eigenvalue](../../../../../../eigenvalue.md) occurs on $\mu^2+\sigma^2=1$, except at $\mu=0$. The symmetry of an [odd function](../../../../../../odd-function.md) $(u,v)\mapsto(-u,-v)$ makes the generic steady bifurcation a [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md). At a point $(\sigma,\mu_0)$ on this circle with $\mu_0\ne0$, vary $\mu=\mu_0+\delta$. Expanding the [radius](../../../../../../radius.md) equation gives $S\sim2\mu_0\delta/(\mu_0+\sigma)$. In a signed, unit-eigenvector [centre manifold](../../../../../../center-manifold.md) coordinate, the cubic coefficient therefore has sign $-(\mu_0+\sigma)/(2\mu_0)$.

On the lower semicircle $\mu_0=-\sqrt{1-\sigma^2}$ the transverse [eigenvalue](../../../../../../eigenvalue.md) is negative: the [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) is supercritical for $\sigma<1/\sqrt2$ and subcritical for $\sigma>1/\sqrt2$. On the upper semicircle it is supercritical for $\sigma>-1/\sqrt2$ and subcritical for $\sigma<-1/\sqrt2$ in the [centre manifold](../../../../../../center-manifold.md) direction, but its transverse [eigenvalue](../../../../../../eigenvalue.md) is positive, so the bifurcating [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are not fully attracting. At $(\sigma,\mu_0)=(\pm1/\sqrt2,\mp1/\sqrt2)$ the cubic vanishes. The [radius](../../../../../../radius.md) equation instead gives $\delta=-S^2/(4\mu_0)+o(S^2)$, a nonzero quintic degeneracy with [amplitude](../../../../../../wave-amplitude.md) proportional to $|\delta|^{1/4}$: these are [degenerate pitchforks in the cubic confinement model](../../../../../../degenerate-pitchfork-in-the-cubic-confinement-model.md).

A [Hopf bifurcation](../../../../../../hopf-bifurcation.md) occurs at $\mu=0$, $|\sigma|>1$, with frequency $\sqrt{\sigma^2-1}$. To determine its direction, first note that the divergence is $2\mu-2S$. The [Bendixson-Dulac criterion](../../../../../../bendixson-dulac-theorem.md) excludes every nonconstant [periodic orbit](../../../../../../periodic-orbit.md) for $\mu\le0$, since this divergence is negative except possibly at the origin. We can also calculate a nonzero saturation coefficient. Set $a=|\sigma+1|$, $b=|\sigma-1|$ and $V=au^2+bv^2$. At $\mu=0$ the linear orbits are [ellipses](../../../../../../ellipse.md) of constant $V$. Direct [differentiation](../../../../../../differentiation.md) gives

$$
\dot V=2\mu V-S\bigl[V+(b-a)uv\bigr].
$$

On a linear [ellipse](../../../../../../ellipse.md), write $u=\sqrt{V/a}\cos\phi$, $v=\sqrt{V/b}\sin\phi$. The angular speed is constant; the averages of $u^3v$ and $uv^3$ vanish, while $\langle S\rangle=V|\sigma|/(\sigma^2-1)$. Averaging the cubic terms, or removing their oscillatory parts by a periodic change of coordinates in its [normal form](../../../../../../normal-form-dynamical-systems.md), gives for $\varrho=\sqrt V$

$$
\dot\varrho=\mu\varrho-\frac{|\sigma|}{2(\sigma^2-1)}\varrho^3
+O(\varrho^5+|\mu|\varrho^3).
$$

The cubic coefficient is strictly negative. Hence a small attracting [limit cycle](../../../../../../limit-cycle.md) exists for $\mu>0$, and

$$
\boxed{\text{the Hopf bifurcation is supercritical}.}
$$

Finally $(\sigma,\mu)=(\pm1,0)$ have a nonzero [nilpotent matrix](../../../../../../nilpotent-matrix.md) as their [linearization](../../../../../../linearization.md) with two zero [eigenvalues](../../../../../../eigenvalue.md). They are reflection-symmetric double-zero bifurcations where the [Hopf bifurcation](../../../../../../hopf-bifurcation.md) and steady thresholds meet; an ordinary nonzero-frequency [Hopf bifurcation](../../../../../../hopf-bifurcation.md) calculation does not apply there. These, the two degenerate [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) points, and the generic [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md)/[Hopf bifurcation](../../../../../../hopf-bifurcation.md) loci above exhaust the origin's local loss-of-hyperbolicity possibilities.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
