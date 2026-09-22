<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Eliminate the instantaneous [Stokes flow](../../../../../../stokes-flow-split.md) [velocity](../../../../../../velocity.md) in favour of [temperature](../../../../../../temperature.md). On a horizontal [Fourier mode](../../../../../../fourier-mode.md) $k$, the [Stokes temperature-slaving operator](../../../../../../stokes-temperature-slaving-operator.md) maps $\theta$ to $w=\mathcal W_R\theta$, where $(D^2-k^2)^2w=Rk^2\theta$ and $w=w''=0$. The [temperature](../../../../../../temperature.md) evolution has [linear operator](../../../../../../linear-operator.md) $\mathcal L_R=D^2-k^2+\mathcal W_R$ and [bilinear map](../../../../../../bilinear-map.md) $\mathcal N(\phi,\chi)=-\mathbf u_R[\phi]\cdot\nabla\chi$. Under the homogeneous thermal [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md), $\mathcal L_{R_c}$ is [self-adjoint](../../../../../../self-adjoint-operator.md). Normalize its critical [eigenfunction](../../../../../../eigenfunction.md) as $g(z)=\sin\pi z$ and set $s=k_c^2+\pi^2$; the critical vertical [velocity](../../../../../../velocity.md) is $f=s g$.

At order $\epsilon$, the critical [eigenfunction](../../../../../../eigenfunction.md) equation gives $\mathcal L_{R_c}(g e^{ik_cx})=0$. At order $\epsilon^2$, the [weakly nonlinear expansion](../../../../../../weakly-nonlinear-expansion.md) contains the imposed second harmonic and the quadratic products of the critical mode: a horizontally uniform [temperature](../../../../../../temperature.md) correction proportional to $|A|^2$ and, in a general vertical-mode calculation, a second harmonic proportional to $A^2$. These corrections are found by solving the noncritical [boundary value problems](../../../../../../boundary-value-problem.md), with homogeneous thermal data except for the imposed forcing.

At order $\epsilon^3$, the [method of multiple scales](../../../../../../method-of-multiple-scales.md) produces the slow derivative $A_\tau$, the detuning term $R_2\partial_R\mathcal L_R$, and the two cross-advection terms involving first- and second-order fields. Project the $e^{ik_cx}$ component onto the [adjoint eigenfunction](../../../../../../adjoint-eigenfunction.md) using the vertical [inner product](../../../../../../inner-product.md). This is the [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md): divide each resonant projection by $\langle g,g\rangle_z$. The detuning supplies $\mu A$ with $\mu\propto R_2$; interactions of horizontal [wavenumbers](../../../../../../wavenumber.md) $2k_c$ and $-k_c$ permit $\beta A^*$ with $\beta\propto\gamma$; self-interaction through the slaved mean and second harmonic supplies $-\lambda|A|^2A$. Other products have the wrong horizontal [wavenumber](../../../../../../wavenumber.md). Reflection $x\mapsto-x$ permits real coefficients with this cosine forcing. Thus the symmetry-allowed [spatially forced convection amplitude equation](../../../../../../spatially-forced-convection-amplitude-equation.md) is

$$
\boxed{A_\tau=\mu A+\beta A^*-\lambda|A|^2A.}
$$

There is a useful specialization that should not be silently missed. For the literal one-vertical-mode [Stokes flow](../../../../../../stokes-flow-split.md) problem, the [vanishing two-to-one forcing coefficient for Stokes convection](../../../../../../vanishing-two-to-one-forcing-coefficient-for-stokes-convection.md) makes $\beta=0$ at this order. To see this, write a positive second-harmonic forcing component as $(w,\theta)=(W(z),\Theta(z))e^{2ik_cx}$, incorporating the cosine's factor $1/2$. Its coupling to the negative critical harmonic has projected integrand, apart from sign and its factor $A^*$,

$$
g\left(2f'\Theta+f\Theta'+\tfrac12W'g+Wg'\right)=\frac d{dz}\left(sg^2\Theta+\tfrac12g^2W\right).
$$

The integral vanishes because $g=0$ at both plates, even though $\Theta(0)$ is nonzero. This proves the cancellation without solving the forced profiles. The permitted coefficient is therefore zero times $\gamma$; [symmetry](../../../../../../symmetry-physics.md) alone does not establish nonzero phase pinning for the equations actually supplied.

The same normalization makes the remaining coefficients explicit. Since $\mathcal W_Rg=(Rk_c^2/s^2)g$, $\mu=R_2k_c^2/s^2$. The quadratic second harmonic cancels for $f=sg$, while the uniform correction is $\theta_{20}=-s|A|^2\sin(2\pi z)/(2\pi)$. Projecting $-w_1\partial_z\theta_{20}$ gives $-s^2|A|^2A/2$. Thus for the literal model and this [temperature](../../../../../../temperature.md) normalization,

$$
\boxed{\mu=\frac{R_2k_c^2}{s^2},\qquad \beta=0,\qquad \lambda=\frac{s^2}{2}>0.}
$$

A generic nonzero $\beta$ would require a nonvanishing projection in an amended physical model or a different forcing structure. It is still meaningful to classify the real-coefficient [amplitude equation](../../../../../../amplitude-equation.md) requested independently.

Write $A=x+iy$. Then $x_\tau=(\mu+\beta-\lambda(x^2+y^2))x$ and $y_\tau=(\mu-\beta-\lambda(x^2+y^2))y$. These are a [gradient flow](../../../../../../gradient-flow.md) for $V=-\tfrac12(\mu+\beta)x^2-\tfrac12(\mu-\beta)y^2+\tfrac\lambda4(x^2+y^2)^2$, so local minima give stable [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md). At the origin the two [eigenvalues](../../../../../../eigenvalue.md) are $\mu+\beta$ and $\mu-\beta$. The origin has exponential [asymptotic stability](../../../../../../asymptotic-stability.md) if $\mu<-|\beta|$, retains [asymptotic stability](../../../../../../asymptotic-stability.md) with algebraic decay at $\mu=-|\beta|$, and is unstable if $\mu>-|\beta|$. At equality, $\rho^2=x^2+y^2$ obeys $(\rho^2)_\tau\leq-2\lambda\rho^4$, since both linear coefficients are nonpositive. Integrating this inequality proves attraction even in the zero-eigenvalue direction.

For $\beta>0$ the stable nonzero [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are real; for $\beta<0$ they are imaginary:

$$
\boxed{\begin{cases}A=\pm\sqrt{(\mu+\beta)/\lambda},&\beta>0,\ \mu+\beta>0,\\ A=\pm i\sqrt{(\mu-\beta)/\lambda},&\beta<0,\ \mu-\beta>0.\end{cases}}
$$

The real branch has [Jacobian matrix](../../../../../../jacobian-matrix.md) [eigenvalues](../../../../../../eigenvalue.md) $-2(\mu+\beta),-2\beta$; the imaginary branch has $-2(\mu-\beta),2\beta$. The oppositely aligned branch, when it exists, is a [saddle equilibrium](../../../../../../saddle-equilibrium.md). No mixed real-imaginary nonzero equilibrium is possible when $\beta\neq0$.

For $\beta=0$, the origin is stable for $\mu\leq0$, with algebraic decay at zero. If $\mu>0$, the circle $|A|^2=\mu/\lambda$ is radially attracting. Each point has [Lyapunov stability](../../../../../../lyapunov-stability.md) but has a neutral phase direction, so it does not have individual [asymptotic stability](../../../../../../asymptotic-stability.md); the circle has [orbital stability](../../../../../../orbital-stability.md). This is the literal model's unpinned family. The general nonzero-$\beta$ branches instead exhibit [phase locking](../../../../../../phase-locking.md) to one of two phases separated by $\pi$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
