<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $F_{12}=\partial_1A_2-\partial_2A_1$. Up to a total derivative, the covariant-gradient identity and completion of the magnetic and potential terms give

$$
\begin{aligned}
V={}&\frac12\int_D\left[
e^{-2\rho}\left(F_{12}-\frac{e^{2\rho}}2(1-|\Phi|^2)\right)^2
+|D_1\Phi+iD_2\Phi|^2\right]d^2x\\
&+\frac12\int_DF_{12},d^2x.
\end{aligned}
$$

For positive flux, equality in the [Bogomolny bound](../../../../../bogomolny-bound.md) therefore gives the [Bogomolny vortex equations](../../../../../bogomolny-vortex-equation.md)

$$
\boxed{D_1\Phi+iD_2\Phi=0,
\qquad
F_{12}=\frac{e^{2\rho}}2(1-|\Phi|^2)}.
$$

The opposite simultaneous signs describe negative winding.

For the orientation $dx^1\wedge dx^2>0$, the [Hodge star operator](../../../../../hodge-star-operator.md) is

$$
\boxed{*1=e^{2\rho}dx^1\wedge dx^2},
$$



$$
\boxed{*dx^1=dx^2,
\qquad *dx^2=-dx^1},
$$



$$
\boxed{*(dx^1\wedge dx^2)=e^{-2\rho}}.
$$

Thus

$$
\boxed{B=*dA=e^{-2\rho}F_{12}
=\frac12(1-|\Phi|^2)}.
$$

A radial vortex of winding $N>0$ has

$$
\boxed{\Phi=f(r)e^{iN\theta},
\qquad A=a(r)d\theta},
$$

with $f(0)=a(0)=0$, $f(1)=1$, $a(1)=N$, and equations

$$
\boxed{f'=\frac{N-a}{r}f,
\qquad
\frac{a'}r=\frac{e^{2\rho}}2(1-f^2)}.
$$

For $e^{2\rho}=8/(1-|z|^2)^2$, put $u=\log|\Phi|$. Away from zeros, the first vortex equation gives

$$
\Delta u=-\frac{e^{2\rho}}2(1-e^{2u}).
$$

Since

$$
\Delta[-\log(1-z\bar z)]=\frac4{(1-|z|^2)^2},
$$

the field $\psi=u-\log(1-z\bar z)+\log2$ satisfies the [Liouville equation](../../../../../liouville-equation.md)

$$
\boxed{\Delta\psi=e^{2\psi}}.
$$

For holomorphic $g:D\to D$, direct use of the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) verifies

$$
\boxed{e^{2\psi}=\frac{4|g'(z)|^2}{(1-|g(z)|^2)^2}}.
$$

Choosing $g(z)=z^{N+1}$ gives the radial [Witten hyperbolic vortex](../../../../../witten-hyperbolic-vortex.md)

$$
\boxed{\Phi(z)=
\frac{(N+1)z^N(1-|z|^2)}{1-|z|^{2N+2}}},
$$



$$
\boxed{A=a_N(r)d\theta,
\qquad
a_N(r)=\frac{2r^2}{1-r^2}
-\frac{(2N+2)r^{2N+2}}{1-r^{2N+2}}}.
$$

For $N=1$ these reduce to

$$
f(r)=\frac{2r}{1+r^2},
\qquad
a_1(r)=\frac{2r^2}{1+r^2}.
$$

Since $Bd\mu_g=dA=a_1'(r)dr\wedge d\theta$,

$$
\int_DBd\mu_g
=2\pi\int_0^1a_1'(r)dr
=2\pi[a_1(1)-a_1(0)]
=\boxed{2\pi}.
$$

This directly verifies the [Abelian Higgs vortex](../../../../../nielsen-olesen-vortex.md) flux relation for unit winding.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
