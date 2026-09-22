<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Differentiate the [material derivative](../../../../../material-derivative.md) of the [passive scalar](../../../../../passive-scalar.md) component by component. With $\sigma_{ij}=\partial_j u_i$,

$$
(\partial_t+u_j\partial_j)\partial_i\theta
=-\partial_i u_j\,\partial_j\theta.
$$

The chain rule along a [Lagrangian trajectory](../../../../../lagrangian-trajectory.md) $\dot X=u(X,t)$ therefore gives the [covector evolution of a material scalar gradient](../../../../../covector-evolution-of-a-material-scalar-gradient.md)

$$
\boxed{\dot k=-\sigma^T k.}
$$

The transpose matters: a [gradient](../../../../../gradient.md) is transported as a [covector](../../../../../covector.md), rather than as a material separation vector. When $u_3=0$, the third row of $\sigma$ vanishes, and

$$
\dot k_1=-\sigma_{11}k_1-\sigma_{21}k_2,\qquad
\dot k_2=-\sigma_{12}k_1-\sigma_{22}k_2,\qquad
\dot k_3=-\sigma_{13}k_1-\sigma_{23}k_2.
$$

Let $k_h=(k_1,k_2)^T$ and set

$$
S=\begin{pmatrix}a&b\\b&-a\end{pmatrix},\qquad
c=\sqrt{a^2+b^2},\qquad S^2=c^2I.
$$

For $c>0$, the [matrix exponential](../../../../../matrix-exponential.md) gives the exact horizontal solution

$$
k_h(t)=\left[I\cosh(ct)-\frac{S}{c}\sinh(ct)\right]k_h(0)
=e^{ct}p_-+e^{-ct}p_+,
\qquad p_\pm=\frac12\left(I\pm\frac{S}{c}\right)k_h(0).
$$

The two projections are onto the [eigenspaces](../../../../../eigenspace.md) with [eigenvalues](../../../../../eigenvalue.md) $-c$ and $+c$. If $p_-\ne0$, write $p_-=k_0(\cos\phi,\sin\phi)^T$ with $k_0=|p_-|>0$. Then

$$
\boxed{k_1\sim k_0e^{ct}\cos\phi,\qquad k_2\sim k_0e^{ct}\sin\phi.}
$$

The stated growing asymptotic requires this nonzero projection. An initial [gradient](../../../../../gradient.md) entirely in the other [eigenspace](../../../../../eigenspace.md) decays, and when $c=0$ the horizontal [gradient](../../../../../gradient.md) is constant.

For constant vertical shear, write $h=(\sigma_{13},\sigma_{23})^T$. Integrating the third component using the exact horizontal solution yields

$$
k_3(t)=k_3(0)-\frac{h\cdot p_-}{c}(e^{ct}-1)
-\frac{h\cdot p_+}{c}(1-e^{-ct}).
$$

Consequently, if $D=h\cdot(\cos\phi,\sin\phi)$ is nonzero, $k_3\sim-k_0D e^{ct}/c$, and

$$
\boxed{\alpha=\frac{|k_3|}{|k_h|}\longrightarrow\frac{|D|}{c}.}
$$

If $D=0$, exponential growth of $k_3$ is absent, but the ratio still tends to zero on the growing horizontal branch. Thus exponential vertical growth is generic, not unconditional. The [scalar-gradient inclination in a steady planar strain](../../../../../scalar-gradient-inclination-in-a-steady-planar-strain.md) is the tangent of the angle between the scalar's normal and the horizontal plane. Equivalently, it is the cotangent of the inclination of an isoconcentration surface to that plane. Large $\alpha$ corresponds to nearly horizontal scalar surfaces; small $\alpha$ corresponds to nearly vertical ones.

For the probability calculation, take $\Gamma,\Lambda>0$. The [independent random variables](../../../../../independent-random-variables.md) $a,b$ with [normal distributions](../../../../../normal-distribution.md) of variance $\Gamma^2$ make $c$ distributed according to the [Rayleigh distribution](../../../../../rayleigh-distribution.md), with

$$
\mathbb P(c\ge r)=e^{-r^2/(2\Gamma^2)}\quad(r\ge0).
$$

The advertised [Gaussian-over-Rayleigh inclination distribution](../../../../../gaussian-over-rayleigh-inclination-distribution.md) also needs $D$ to be independent of $(a,b)$; its Gaussian marginal alone does not imply this. Under that intended assumption, for $A>0$,

$$
\begin{aligned}
\mathbb P(\alpha\le A)
&=\mathbb E\left[\exp\left(-\frac{D^2}{2\Gamma^2A^2}\right)\right]\\
&=\frac1{\sqrt{2\pi}\Lambda}\int_{-\infty}^{\infty}
\exp\left[-\frac{d^2}{2}\left(\frac1{\Lambda^2}+\frac1{\Gamma^2A^2}\right)\right],dd\\
&=\frac{\Gamma A}{\sqrt{\Gamma^2A^2+\Lambda^2}}.
\end{aligned}
$$

The [cumulative distribution function](../../../../../cumulative-distribution-function.md) is zero for $A\le0$. Differentiating gives

$$
\boxed{p_\alpha(A)=\frac{\Lambda^2\Gamma}{(\Gamma^2A^2+\Lambda^2)^{3/2}}\quad(A\ge0),}
$$

and the [probability density function](../../../../../probability-density-function.md) is zero for negative $A$. Its integral is one because the [cumulative distribution function](../../../../../cumulative-distribution-function.md) tends to one at infinity. Independence is a real hypothesis: $D=(\Lambda/\Gamma)a$ has exactly the stated Gaussian marginal but makes $\alpha\le\Lambda/\Gamma$ almost surely, contradicting the unbounded support of this density. A sufficient physical model is isotropic Gaussian vertical shear, independent of $a,b$, whose projection in any horizontal direction has variance $\Lambda^2$.

If the strain varies slowly, the horizontal [gradient](../../../../../gradient.md) must align with the current growing direction, and the vertical-to-horizontal ratio must adjust before that strain changes. Both adjustment times are of order $c^{-1}$. Thus the local condition is **$c\tau_\sigma\gg1$**, and the typical condition for the specified statistics is

$$
\boxed{\Gamma\tau_\sigma\gg1.}
$$

This is an adiabatic approximation, not a uniform statement about arbitrarily weak instantaneous strains: samples with $c\tau_\sigma\lesssim1$ retain memory of earlier strain. The instantaneous [eigenvector](../../../../../eigenvector.md) must likewise turn slowly compared with $c$.

For rapidly fluctuating vertical shear, insert the large-time horizontal solution into its [stochastic differential equation](../../../../../stochastic-differential-equation.md):

$$
dk_3=-k_0g e^{ct}\bigl(\cos\phi\,dW^{(1)}+\sin\phi\,dW^{(2)}\bigr)
=-k_0g e^{ct}\,dW.
$$

The linear combination $W=\cos\phi W^{(1)}+\sin\phi W^{(2)}$ is a [Brownian motion](../../../../../brownian-motion-split.md): it has independent Gaussian increments and increment variance $(\cos^2\phi+\sin^2\phi)dt=dt$. For the signed inclination $\beta=k_3 e^{-ct}/k_0$, the [Itô product rule](../../../../../ito-product-rule.md) introduces no extra cross term because the exponential factor is deterministic. It follows that

$$
\boxed{d\beta=-c\beta\,dt-g\,dW.}
$$

This is an [Ornstein-Uhlenbeck process](../../../../../ornstein-uhlenbeck-process.md), explaining why [white-noise vertical shear gives an Ornstein-Uhlenbeck inclination](../../../../../white-noise-vertical-shear-gives-an-ornstein-uhlenbeck-inclination.md). Its [Fokker-Planck equation](../../../../../fokker-planck-equation.md) is

$$
\boxed{\partial_t p=c\,\partial_B(Bp)+\frac{g^2}{2}\partial_B^2p.}
$$

In a stationary state the [Fokker-Planck probability current](../../../../../fokker-planck-probability-current.md) $j=-cBp-(g^2/2)p'$ is constant. A nonzero constant current cannot give an integrable, nonnegative density at both ends of the real line, so $j=0$. Integrating $p'/p=-2cB/g^2$ and normalizing with the [Gaussian integral](../../../../../gaussian-integral.md) gives

$$
\boxed{p_\beta(B;c)=\sqrt{\frac{c}{\pi g^2}}\exp\left(-\frac{cB^2}{g^2}\right),\qquad B\in\mathbb R.}
$$

The stationary [variance](../../../../../variance-split.md) is $g^2/(2c)$. More explicitly the [explicit Ornstein-Uhlenbeck solution](../../../../../explicit-ornstein-uhlenbeck-solution.md) has mean $\beta(0)e^{-ct}$ and variance $g^2(1-e^{-2ct})/(2c)$, confirming convergence to this density. Here $c>0$ and $g\ne0$ are needed for the stated smooth stationary density; at $c=0$ there is no confinement, while $g=0$ gives a point mass at zero.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
