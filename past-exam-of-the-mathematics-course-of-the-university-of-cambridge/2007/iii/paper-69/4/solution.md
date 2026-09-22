<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For an isolated, virialized three-dimensional Newtonian system with negligible boundary-pressure terms, the [virial theorem](../../../../../virial-theorem.md) gives $2K+W=0$. Hence its total energy is $E=K+W=-K$. Defining the kinetic temperature by $K=3NkT/2$ gives

$$
\boxed{\frac{dE}{dT}=-\frac32Nk<0.}
$$

Thus losing energy makes the system hotter, while adding energy makes it cooler. This [negative heat capacity of a virialized gravitational system](../../../../../negative-heat-capacity-of-a-virialized-gravitational-system.md) uses the inverse-distance potential and the stated boundary assumptions; it is not a dimension-independent consequence of self-gravity.

A [gravothermal catastrophe](../../../../../gravothermal-catastrophe.md) occurs when a stellar core loses heat to its halo through [two-body relaxation](../../../../../two-body-relaxation.md), contracts and becomes hotter because of its negative [heat capacity](../../../../../heat-capacity.md). The larger temperature gradient then drives more heat outward and accelerates contraction. In the confined three-dimensional isothermal sequence this runaway is associated with loss of a regular thermodynamic equilibrium at a finite total energy. It is different from a fast collisionless instability.

For the rods, use energies and masses per unit axial length, consistently with their logarithmic interaction. Define

$$
q=\frac{GM\beta}{2},\qquad x=\frac{R^2}{R_e^2},\qquad F(x)=1-q+qx,\qquad
\psi_e=-GM\log(V/V_0).
$$

Integrating the two-dimensional [Maxwell-Boltzmann velocity distribution](../../../../../maxwell-boltzmann-velocity-distribution.md) gives $\rho=Ae^{\beta\psi}$, with a positive normalization $A$. The proposed potential has $\psi=\psi_e-2\log F/\beta$, so this requires $\rho\propto F^{-2}$. Direct differentiation gives

$$
\psi'=-\frac{2GM R}{R_e^2F},\qquad
\frac1R(R\psi')'=-\frac{4GM(1-q)}{R_e^2F^2}.
$$

Consequently the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) is satisfied precisely by

$$
\boxed{\rho(R)=\frac{M(1-q)}{\pi R_e^2F^2}.}
$$

The free normalization of the velocity distribution can be chosen to give this density. Its enclosed line mass verifies total-mass normalization:

$$
M(<R)=M(1-q)\int_0^x\frac{du}{(1-q+qu)^2}
=\boxed{\frac{Mx}{F(x)}},\qquad M(<R_e)=M.
$$

At the wall $F(1)=1$, so the required potential value is also satisfied. This establishes the [two-dimensional self-gravitating rod equilibrium](../../../../../two-dimensional-self-gravitating-rod-equilibrium.md), including its field equation, distribution law, mass and boundary condition.

A regular positive solution needs $F(0)=1-q>0$. Since $\beta=m/(kT)$,

$$
\boxed{T>T_{\min},\qquad kT_{\min}=\frac12GMm.}
$$

The minimum is an infimum of regular equilibrium temperatures. At equality the central logarithm is singular; for $T<T_{\min}$, $F$ vanishes inside the box. Thus equality is not a regular isothermal rod configuration.

Each of the two velocity components has second moment $1/\beta$, so the kinetic energy is $K=M/\beta=NkT$. With the given reference potential, the gravitational potential energy is $W=-\tfrac12\int\rho\psi\,d^2R$. Using $dM=M(1-q)dx/F^2$ gives

$$
W=-\frac{M\psi_e}{2}+\frac1\beta\int\log F\,dM.
$$

The remaining integral can be evaluated explicitly:

$$
\begin{aligned}
\int\log F\,dM
&=\frac{M(1-q)}q\int_{1-q}^1\frac{\log F}{F^2}\,dF\\
&=\frac{M(1-q)}q\left[-\frac{\log F+1}{F}\right]_{1-q}^1
=M\left[1+\frac1q\log(1-q)\right].
\end{aligned}
$$

Adding $K$ therefore yields

$$
E=\frac{GM^2}{2}\log(V/V_0)+\frac{M}{\beta}\left[2+\frac1q\log(1-q)\right].
$$

Now $NkT_{\min}=GM^2/2$, $\Theta=T/T_{\min}=1/q$ and $M/\beta=NkT_{\min}\Theta$. The [energy-temperature curve of a two-dimensional self-gravitating rod gas](../../../../../energy-temperature-curve-of-a-two-dimensional-self-gravitating-rod-gas.md) is consequently

$$
\boxed{E=NkT_{\min}\left[\log(V/V_0)+2\Theta+\Theta^2\log(1-\Theta^{-1})\right],\qquad\Theta>1.}
$$

At fixed box area, differentiation gives

$$
C_V=Nk\left[2+2\Theta\log(1-\Theta^{-1})+\frac{\Theta}{\Theta-1}\right].
$$

To establish its sign rather than infer it from a plot, expand the logarithm for $\Theta>1$:

$$
2\Theta+\Theta^2\log(1-\Theta^{-1})
=\Theta-\frac12-\sum_{j=3}^{\infty}\frac1{j\Theta^{j-2}},
\qquad
\boxed{\frac{C_V}{Nk}=1+\sum_{j=3}^{\infty}\frac{j-2}{j\Theta^{j-1}}>1.}
$$

The series and its derivative converge locally uniformly in $\Theta>1$. Moreover $E\to-\infty$ as $\Theta\downarrow1$ and $E\to+\infty$ as $\Theta\to\infty$. Thus every finite energy on this mean-field isothermal sequence has a unique regular equilibrium temperature, and there is no finite-energy termination or turning point. The central density $M/[V(1-q)]$ diverges only in the infinite-negative-energy limit.

**There is no finite-energy gravothermal catastrophe in this two-dimensional rod model.** Its logarithmic interaction gives a different caloric curve from the three-dimensional inverse-distance problem. This microcanonical conclusion does not prohibit a distinct fixed-temperature collapse: in the [canonical ensemble](../../../../../canonical-ensemble.md), a bath at or below $T_{\min}$ admits no regular equilibrium of this family.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
