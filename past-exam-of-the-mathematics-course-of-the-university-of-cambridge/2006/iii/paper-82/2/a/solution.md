<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $0<\theta_0<\pi$, put $a=k_0\cos\theta_0$ and $b=k_0\sin\theta_0>0$, and suppress the common factor $e^{i\omega t}$. The upper-half-plane incident [acoustic plane wave](../../../../../../acoustic-plane-wave.md) is $e^{iax+iby}$. A rigid zero-thickness screen imposes the same normal-derivative cancellation on both faces; the scattered [velocity potential](../../../../../../velocity-potential.md) is consequently odd in $y$. Across the open part $x>0$ it is continuous, so its trace there is zero. These complementary half-line data are what make the [Wiener-Hopf method](../../../../../../wiener-hopf-method.md) applicable.

Use the [Fourier transform](../../../../../../fourier-transform.md) $\widehat\phi(\kappa,y)=\int_{\mathbb R}\phi(x,y)e^{i\kappa x}dx$, with inverse exponential $e^{-i\kappa x}$. The outgoing [Helmholtz equation](../../../../../../helmholtz-equation.md) solution is $\widehat\phi=F^-(\kappa)e^{-\gamma y}$ for $y>0$, where $\gamma=\sqrt{\kappa^2-k_0^2}$ has $\gamma=i\sqrt{k_0^2-\kappa^2}$ on the propagating interval and positive real part on evanescent components. The [limiting absorption principle](../../../../../../limiting-absorption-principle.md) supplies the contour prescription. The transform $F^-$ of the trace supported on $x<0$ is analytic below the contour. Let $G^+$ be the analytic upper transform of the unknown derivative on $x>0$. The prescribed derivative on $x<0$ has transform

$$
\int_{-\infty}^0(-ib)e^{i(\kappa+a)x}dx=-\frac b{\kappa+a}.
$$

Since the upper normal derivative is $-\gamma F^-$, the [Wiener-Hopf equation](../../../../../../wiener-hopf-equation.md) is

$$
\gamma F^-+G^+=\frac b{\kappa+a}.
$$

For the [Wiener-Hopf factorization](../../../../../../wiener-hopf-factorization.md), choose $\gamma_+=(\kappa-k_0)^{1/2}$ analytic above and $\gamma_-=(\kappa+k_0)^{1/2}$ analytic below. Their [branch cuts](../../../../../../branch-cut.md) go into the opposite half-planes, with $\gamma_+(-a)=i\sqrt{k_0+a}$. Dividing by $\gamma_+$ and performing [pole subtraction in a Wiener-Hopf equation](../../../../../../pole-subtraction-in-a-wiener-hopf-equation.md) gives

$$
\frac b{(\kappa+a)\gamma_+(\kappa)}=
\frac b{(\kappa+a)\gamma_+(-a)}+
\frac b{\kappa+a}\left[\frac1{\gamma_+(\kappa)}-\frac1{\gamma_+(-a)}\right].
$$

The forcing pole is allocated to the lower analytic part; the second quotient has a removable pole and is upper analytic. Subtracting these parts leaves a common [entire function](../../../../../../entire-function.md). The finite-energy edge condition excludes an inverse-square-root singularity in the potential: its odd scattered trace is $O(\sqrt{|x|})$, so $F^-=O(|\kappa|^{-3/2})$. The normal derivative on the open side can be $O(x^{-1/2})$, giving $G^+=O(|\kappa|^{-1/2})$. Both sides of the entire remainder tend to zero. The [Liouville theorem](../../../../../../liouville-theorem.md) sets that remainder to zero, giving the explicit [Wiener-Hopf solution of rigid half-plane diffraction](../../../../../../wiener-hopf-solution-of-rigid-half-plane-diffraction.md):

$$
\boxed{F^-(\kappa)=\frac{b}{(\kappa+a)\gamma_+(-a)\gamma_-(\kappa)}=
\frac{-i\sqrt{2k_0}\sin(\theta_0/2)}{(\kappa+a)\sqrt{\kappa+k_0}}.}
$$

The scattered field on either side of the screen is therefore

$$
\phi(x,y)=\frac{\operatorname{sgn}y}{2\pi}\int F^-(\kappa)e^{-i\kappa x-\gamma|y|}d\kappa.
$$

Its forcing-pole [residue](../../../../../../residue.md) at $\kappa=-a$ is $-i$. Deforming to the outgoing [steepest descent contour](../../../../../../steepest-descent-contour.md) crosses this pole precisely when $|\theta|>\pi-\theta_0$, where $x=r\cos\theta$, $y=r\sin\theta$ and $-\pi<\theta<\pi$. The residue contributes $\operatorname{sgn}(y)e^{iax-ib|y|}$. Thus, away from transition boundaries, the scattered [geometrical optics](../../../../../../geometrical-optics.md) field is

$$
\phi_{\rm GO}=
\begin{cases}
e^{iax-iby},&\pi-\theta_0<\theta<\pi,\\
-e^{iax+iby},&-\pi<\theta<\theta_0-\pi,\\
0,&\text{otherwise}.
\end{cases}
$$

Adding the incident [acoustic plane wave](../../../../../../acoustic-plane-wave.md) gives incident plus unit [specular reflection](../../../../../../specular-reflection.md) in the upper reflected sector, just the incident wave in the remaining illuminated sectors, and zero in the lower shadow sector. The geometrical shadow boundaries also follow directly by tracing a straight ray to $y=0$: the reflected ray hits the screen at $x+y\cot\theta_0<0$, and the transmitted incident ray crosses the open part at $x-y\cot\theta_0>0$.

For the diffracted contribution, the outgoing phase $-i\kappa r\cos\theta-\gamma r|\sin\theta|$ has saddle $\kappa_s=k_0\cos\theta$, value $-ik_0r$, and second derivative $ir/(k_0\sin^2\theta)$. [Stationary phase](../../../../../../stationary-phase-method.md) therefore supplies $\sqrt{2\pi k_0/r}|\sin\theta|e^{-ik_0r+i\pi/4}$. Substituting $F^-(\kappa_s)$, and using $\operatorname{sgn}(y)|\sin\theta|/\sqrt{1+\cos\theta}=\sqrt2\sin(\theta/2)$, gives

$$
\boxed{\phi_d\sim\sqrt{\frac{2}{\pi k_0r}}\frac{\sin(\theta_0/2)\sin(\theta/2)}{\cos\theta+\cos\theta_0}e^{-ik_0r-i\pi/4}.}
$$

The full asymptotic scattered field is $\phi_{\rm GO}+\phi_d$. The angular edge-wave expression is not uniform on the geometrical boundaries. There is also a sign inconsistency in the supplied saddle formula: with its printed inverse exponential $e^{+i\kappa x}$, the outgoing saddle is $-k_0\cos\theta$, not $+k_0\cos\theta$. The consistent inverse convention used above gives the requested outgoing field without that ambiguity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
