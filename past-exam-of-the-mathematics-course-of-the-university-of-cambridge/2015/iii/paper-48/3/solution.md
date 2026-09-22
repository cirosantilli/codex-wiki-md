<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $A_s$ denote the [surface area of an n-sphere](../../../../../surface-area-of-an-n-sphere.md) for the unit sphere $S^s$. In this notation $s$ is the intrinsic dimension of the sphere. Cartesian factorization of the [Gaussian integral](../../../../../gaussian-integral.md) gives $I_N=\pi^{N/2}$. In [hyperspherical coordinates](../../../../../hyperspherical-coordinates.md),

$$
I_N=A_{N-1}\int_0^\infty\rho^{N-1}e^{-\rho^2}\,d\rho=\frac12A_{N-1}\Gamma(N/2).
$$

The substitution $t=\rho^2$ supplies the defining [Gamma function](../../../../../gamma-function.md) integral. Scaling the sphere radius multiplies its surface volume by $r^{N-1}$, hence

$$
\boxed{\operatorname{vol}(S^{N-1}_r)=A_{N-1}r^{N-1}=\frac{2\pi^{N/2}}{\Gamma(N/2)}r^{N-1}.}
$$

This is the volume of the sphere itself, not of its enclosed ball.

Take $D$ to denote spacetime dimension and $d=D-1$ spatial dimensions. In uncompactified flat space, [Gauss's law](../../../../../gauss-s-law.md) for a charge $q$ and permittivity $\varepsilon_d$ gives $E_r A_{d-1}r^{d-1}=q/\varepsilon_d$. Since $E_r=-d\varphi/dr$, the [electric potential](../../../../../electric-potential.md) for $d>2$, normalized to vanish at infinity, is

$$
\boxed{\varphi(r)=\frac{q}{(d-2)\varepsilon_d A_{d-1}r^{d-2}}=\frac{q}{(D-3)\varepsilon_{D-1}A_{D-2}r^{D-3}}.}
$$

Thus the four-dimensional [electric potential](../../../../../electric-potential.md) falls as $1/r$, and the five-dimensional one as $1/r^2$. If a convention counts only spatial dimensions as $D$, replace $d$ by $D$ in the first formula. For $d=2$, the integral instead gives $\varphi=-q\log(r/r_0)/(2\pi\varepsilon_2)$; for $d=1$, it gives $\varphi=-q|x|/(2\varepsilon_1)$ up to a constant. Neither case has a finite zero at infinity.

For a [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) $\Phi_g$, define the flux-normalized coupling $\kappa_d$ by $\nabla^2\Phi_g=\kappa_d m\delta^{(d)}(\mathbf x)$ and acceleration $-\nabla\Phi_g$. Exactly the same flux integration gives the attractive potential

$$
\boxed{\Phi_g(r)=-\frac{\kappa_d m}{(d-2)A_{d-1}r^{d-2}}\quad(d>2).}
$$

In $d=3$, $\kappa_3=4\pi G_4$ reproduces $-G_4m/r$. If $G_D$ is defined by the $D$-dimensional [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) $S=(16\pi G_D)^{-1}\int\sqrt{-g}\,R$, the weak static [Einstein field equations](../../../../../einstein-field-equations.md) give $\kappa_d=8\pi G_D(D-3)/(D-2)$ for $D>3$. Therefore

$$
\Phi_g=-\frac{8\pi G_Dm}{(D-2)A_{D-2}r^{D-3}}.
$$

Indeed, $R_{00}\simeq\nabla^2\Phi_g$ and $T_{00}-g_{00}T/(D-2)=(D-3)\rho/(D-2)$ in signature $(-+\cdots+)$. A Poisson-defined Newtonian theory in two spatial dimensions has a logarithmic potential, but pure three-dimensional Einstein gravity has no analogous local Newtonian point-mass force; the relativistic normalization must not be extrapolated to that exceptional dimension.

For an unwarped product with a fixed extra-dimensional metric, normalize the [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) by $\tfrac12M_*^{n+2}\int d^{4+n}x\sqrt{-g}\,R$. Integrating the part containing the four-dimensional curvature over the internal space gives $\tfrac12M_*^{n+2}\operatorname{vol}(S^n_R)\int d^4x\sqrt{-g_4}\,R_4$. Thus, using the [reduced Planck mass](../../../../../reduced-planck-mass.md),

$$
\boxed{M_{\rm Pl}^2=M_*^{n+2}\frac{2\pi^{(n+1)/2}}{\Gamma((n+1)/2)}R^n,\qquad R=M_*^{-1}\left[\frac{M_{\rm Pl}^2}{A_nM_*^2}\right]^{1/n}.}
$$

This is a volume relation for [compactification](../../../../../compactification-physics.md); a curved sphere additionally requires a mechanism supporting and stabilizing its background. It is not by itself a proof that a sphere times flat spacetime solves a vacuum gravitational theory.

With $M_*=10^3\,\mathrm{GeV}$, $M_{\rm Pl}=2.435\times10^{18}\,\mathrm{GeV}$ and $1\,\mathrm{GeV}^{-1}=1.97327\times10^{-16}\,\mathrm m$, the spherical-volume factors $A_1=2\pi$, $A_2=4\pi$, $A_6=16\pi^3/15$ give

$$
\boxed{R_{n=1}\simeq1.86\times10^{11}\,\mathrm m,\qquad R_{n=2}\simeq1.36\times10^{-4}\,\mathrm m,\qquad R_{n=6}\simeq1.48\times10^{-14}\,\mathrm m.}
$$

The first estimate is astronomical; the second is roughly a tenth of a millimetre. If both Planck scales are instead defined by $S=M_D^{D-2}\int\sqrt{-g}R/(16\pi)$, the same algebraic volume relation uses the unreduced $M_{\rm planck}=1.221\times10^{19}\,\mathrm{GeV}$. Holding that convention's $M_*=1\,\mathrm{TeV}$ gives radii larger by $(8\pi)^{1/n}$: approximately $4.69\times10^{12}\,\mathrm m$, $6.80\times10^{-4}\,\mathrm m$, $2.54\times10^{-14}\,\mathrm m$. These are different conventions for what is held fixed at one TeV, not different scaling laws.

Finally, compactify the fifth coordinate on a circle of circumference $L=2\pi R$. For a source and observer at the same compact coordinate, the [method of images](../../../../../method-of-images.md) turns a five-dimensional static potential $C/\rho^2$ into

$$
U(r)=C\sum_{j\in\mathbb Z}\frac1{r^2+j^2L^2}=\frac{C\pi}{Lr}\coth\left(\frac{\pi r}{L}\right).
$$

One can derive this image sum without assuming a summation formula. The [Fourier transform](../../../../../fourier-transform.md) of $1/(r^2+y^2)$ is $\pi e^{-r|k|}/r$; [Poisson summation](../../../../../poisson-summation-formula.md) then gives $\pi[1+2\sum_{\ell\ge1}e^{-2\pi\ell r/L}]/(Lr)$, which is the displayed hyperbolic cotangent. Therefore

$$
\boxed{U(r)=\frac{C\pi}{Lr}\left[1+2e^{-2\pi r/L}+O(e^{-4\pi r/L})\right]\quad(r\gg L).}
$$

The short-distance limit is $C/r^2$; the long-distance limit is the four-dimensional $1/r$ potential. These exponential corrections are the nonzero [Kaluza-Klein modes](../../../../../kaluza-klein-mode.md), with masses $2\pi|\ell|/L$. For electrostatics $C=q/(4\pi^2\varepsilon_4)$, so the effective permittivity is $\varepsilon_3=L\varepsilon_4$. For a Poisson-normalized gravitational potential, $C=-\kappa_4m/(4\pi^2)$ gives $\kappa_3^{\rm eff}=\kappa_4/L$. A massless scalar associated with the circle radius also contributes in an unstabilized gravitational compactification; recovering pure four-dimensional Einstein gravity with $G_4=G_5/L$ requires its stabilization or removal. The $1/r$ crossover itself is independent of this tensor-versus-scalar normalization issue.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
