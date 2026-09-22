<h1 id="18c/solution">Solution</h1>

↑ **Parent:** [18C](../18c.md)

Let the perturbed interface be $z=\eta(x,y,t)$. For inviscid disturbances about rest, the initially irrotational velocities remain potential flows,

$$
\mathbf u_i=\nabla\phi_i,
\qquad \nabla^2\phi_i=0,
$$

in the upper layer $0<z<h$ and lower layer $-h<z<0$. The rigid walls impose [no-penetration boundary condition](../../../../../no-penetration-boundary-condition.md)

$$
\partial_z\phi_1=0\ (z=h),
\qquad
\partial_z\phi_2=0\ (z=-h),
$$

and zero normal derivative at $x,y=0,2h$. Linearizing the kinematic and pressure-continuity conditions at $z=0$ gives

$$
\eta_t=\partial_z\phi_1=\partial_z\phi_2,
\qquad
\rho_1(\phi_{1t}+g\eta)=\rho_2(\phi_{2t}+g\eta).
$$

The horizontal Neumann eigenfunctions are

$$
\cos\frac{m\pi x}{2h}\cos\frac{n\pi y}{2h},
\qquad
k=\frac\pi{2h}\sqrt{m^2+n^2},
$$

where $m,n$ are nonnegative integers, not both zero. For time dependence $e^{-i\omega t}$, the vertical factors satisfying the rigid lids are

$$
\phi_1=A_1\cosh k(z-h),
\qquad
\phi_2=A_2\cosh k(z+h).
$$

The kinematic condition gives their interface values

$$
\phi_1(0)=\frac{i\omega}{k}\coth(kh)\eta,
\qquad
\phi_2(0)=-\frac{i\omega}{k}\coth(kh)\eta.
$$

Substitution into the dynamic condition yields the [interfacial gravity-wave dispersion relation](../../../../../interfacial-gravity-wave-dispersion-relation.md)

$$
\boxed{\omega^2=\frac{\rho_2-\rho_1}{\rho_1+\rho_2}gk\tanh(kh)}.
$$

For $\rho_2>\rho_1$, the lowest nontrivial wavenumber is $k=\pi/(2h)$, with the two degenerate modes $(m,n)=(1,0)$ and $(0,1)$. If $\rho_1\ll\rho_2$, the relation reduces to the finite-depth free-surface result $\omega^2\simeq gk\tanh(kh)$. If $\rho_1>\rho_2$, then $\omega^2<0$ and disturbances grow exponentially: this is the [Rayleigh-Taylor instability](../../../../../rayleigh-taylor-instability.md).

## ↑ Ancestors (10)

1. [18C](../18c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
