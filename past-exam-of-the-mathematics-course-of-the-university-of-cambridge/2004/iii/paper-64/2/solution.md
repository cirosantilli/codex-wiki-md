<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The equilibrium [isothermal equation of state](../../../../../globally-isothermal-equation-of-state.md) is $p=c_s^2\rho$. [Hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) gives $p_z=-\rho\Omega^2z$, hence

$$
\frac{d\ln\rho}{dz}=-\frac{\Omega^2z}{c_s^2},\qquad
\boxed{\rho(z)=\rho_0e^{-z^2/(2H^2)},\quad H=\frac{c_s}{|\Omega|}.}
$$

Here $\Omega\ne0$ is assumed. This is the same local harmonic-gravity balance as [isothermal vertical structure in stellar gravity](../../../../../isothermal-vertical-structure-in-stellar-gravity.md).

For $\gamma>1$, this equilibrium is stably stratified under [adiabatic fluid perturbations](../../../../../adiabatic-fluid-perturbation.md). Its squared [buoyancy frequency](../../../../../buoyancy-frequency.md) is

$$
N^2=g\left(\frac1\gamma\frac{p_z}{p}-\frac{\rho_z}{\rho}\right)
=\frac{\gamma-1}{\gamma}\frac{g^2}{c_s^2}\ge0.
$$

A general perturbation can therefore support [acoustic waves](../../../../../acoustic-wave.md) restored by compression and [internal gravity waves](../../../../../internal-wave.md) restored by [buoyancy](../../../../../buoyancy.md), with nonoscillatory [entropy](../../../../../entropy.md) or vortical disturbances also possible. The prescribed [velocity](../../../../../velocity.md) is purely vertical and horizontally uniform. It describes vertical [acoustic waves](../../../../../acoustic-wave.md); it does not contain the horizontally varying circulation required for an oscillatory internal-gravity branch. For zero horizontal [wavenumber](../../../../../wavenumber.md), that branch has zero [frequency](../../../../../frequency.md). An isothermal equilibrium must not be confused with an isothermal perturbation: the latter would remove the buoyancy restoring force.

Introduce the [fluid Lagrangian displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) $\xi(z)e^{i\sigma t}$, so $w=i\sigma\xi$. Use $\delta\rho,\delta p$ for [fluid Eulerian perturbations](../../../../../eulerian-perturbation-of-a-fluid-variable.md) and $\Delta\rho,\Delta p$ for [fluid Lagrangian perturbations](../../../../../lagrangian-perturbation-of-a-fluid-variable.md). The [continuity equation](../../../../../continuity-equation.md) and the adiabatic relation are

$$
\delta\rho=-(\rho\xi)_z,\qquad
\Delta\rho=-\rho\xi_z,\qquad
\Delta p=\gamma p\frac{\Delta\rho}{\rho},\qquad
\delta p=-\gamma p\xi_z-\xi p_z.
$$

The fixed external [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) is not perturbed. The vertical [linearized Euler equations](../../../../../linearized-euler-equations.md) consequently give

$$
-\sigma^2\rho\xi=-(\delta p)_z-g\,\delta\rho.
$$

Substituting the preceding relations, and using $p_z=-\rho g$ and $p_{zz}=-\rho_zg-\rho g_z$, reduces its right-hand side to

$$
\gamma p\xi_{zz}-\gamma\rho g\xi_z-\rho g_z\xi.
$$

Since $g=\Omega^2z$ and $g_z=\Omega^2$, the same equation holds for $w$:

$$
\boxed{w_{zz}-\frac z{H^2}w_z+
\frac1\gamma\left(\frac{\sigma^2}{c_s^2}-\frac1{H^2}\right)w=0.}
$$

The rigid fixed base supplies the essential condition **$w(0)=0$**. At infinity the condition is finite [kinetic energy](../../../../../kinetic-energy.md), not bounded [velocity](../../../../../velocity.md) amplitude; a [polynomial](../../../../../polynomial-split.md) can grow while the Gaussian [mass density](../../../../../density.md) makes its energy finite.

Put $x=z/H$ and $\lambda=(\sigma^2/\Omega^2-1)/\gamma$. The equation becomes the [Hermite differential equation](../../../../../hermite-differential-equation.md) in its probabilists' convention,

$$
w_{xx}-xw_x+\lambda w=0.
$$

For $w=\sum_{j\ge0}a_jx^j$, its recurrence is

$$
\boxed{a_{j+2}=\frac{j-\lambda}{(j+2)(j+1)}a_j.}
$$

The base condition makes $a_0=0$ and therefore every even coefficient zero. An odd series terminates at degree $2n+1$ when $\lambda=2n+1$. It remains to prove that a nonterminating odd solution cannot have finite energy; termination alone would not establish the requested exhaustion of modes.

For that purpose, set $y=e^{-x^2/4}w$. The finite-energy condition is $y\in L^2(0,\infty)$, and its equation is

$$
Ly\equiv\left(-\frac{d^2}{dx^2}+\frac{x^2}{4}\right)y
=\left(\lambda+\frac12\right)y,\qquad y(0)=0.
$$

Because the coefficients are even and the solution is odd at the base, extend $y$ oddly to the whole real line. Define lowering and raising operators

$$
a=\frac d{dx}+\frac x2,\qquad
a^\dagger=-\frac d{dx}+\frac x2,\qquad
L=a^\dagger a+\frac12,\qquad [L,a]=-a.
$$

Integration by parts gives $\|ay\|^2=\lambda\|y\|^2$, so $\lambda\ge0$. These identities apply to the square-integrable solution: multiplying its equation by a compactly cut off conjugate and taking larger cutoffs bounds $y'$ and $xy$ in $L^2$, and removes the endpoint terms. The same argument applies to each lowered [eigenfunction](../../../../../eigenfunction.md).

If $\lambda$ is not a nonnegative integer, repeatedly apply $a$. Each application lowers $\lambda$ by one and remains nonzero whenever its current value is positive, by the norm identity. After finitely many applications it would yield a nonzero square-integrable [eigenfunction](../../../../../eigenfunction.md) with negative $\lambda$, contradicting that identity. Thus $\lambda=N$ is a nonnegative integer. At $N=0$, $ay=0$ gives $y\propto e^{-x^2/4}$, which is even. Lowering reverses parity, so an initially odd [eigenfunction](../../../../../eigenfunction.md) can reach this even ground state only if $N$ is odd. Consequently $N=2n+1$. The recurrence then terminates and uniquely determines the odd solution from $a_1$.

The complete [adiabatic vertical modes of a Gaussian atmosphere](../../../../../adiabatic-vertical-modes-of-a-gaussian-atmosphere.md) are therefore

$$
\boxed{w_n(z)=A_n\mathrm{He}_{2n+1}(z/H),\qquad
\sigma_n^2=\Omega^2[1+\gamma(2n+1)],\quad n=0,1,2,\ldots.}
$$

Here $\mathrm{He}_j$ is the [Probabilists' Hermite polynomial](../../../../../probabilists-hermite-polynomial.md). For example the first shapes are $x$, $x^3-3x$, and $x^5-10x^3+15x$, with [frequencies](../../../../../frequency.md) squared $\Omega^2(1+\gamma)$, $\Omega^2(1+3\gamma)$, and $\Omega^2(1+5\gamma)$. Either sign of each real [frequency](../../../../../frequency.md) gives a time-harmonic solution. Gaussian moments make every displayed [polynomial](../../../../../polynomial-split.md) have finite [kinetic energy](../../../../../kinetic-energy.md). Without the fixed-base condition, finite energy alone would also admit even [polynomials](../../../../../polynomial-split.md), which is why that condition is necessary.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
