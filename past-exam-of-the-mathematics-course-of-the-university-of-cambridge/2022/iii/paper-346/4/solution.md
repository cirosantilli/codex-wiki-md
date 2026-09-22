<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write proper position as $\mathbf r=a(t)\mathbf x$ and proper velocity as

$$
\mathbf u=\dot{\mathbf r}=H\mathbf r+\mathbf v,
\qquad
\mathbf v=a\dot{\mathbf x}.
$$

Substitute this decomposition into the proper-coordinate [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md), use $\nabla_r=a^{-1}\nabla_x$, and subtract the homogeneous-background acceleration. With $\rho=\bar\rho(1+\delta)$, one obtains the comoving [peculiar-velocity equation](../../../../../peculiar-velocity-equation.md)

$$
\boxed{\frac{\partial\mathbf v}{\partial t}+\frac{\dot a}{a}\mathbf v
+\frac1a(\mathbf v\mathbin\cdot\nabla)\mathbf v
=-\frac1a\nabla\Phi
-\frac1{a\bar\rho(1+\delta)}\nabla P.}
$$

The [peculiar gravitational potential](../../../../../peculiar-gravitational-potential.md) $\Phi$ is the total Newtonian potential with the potential of the exactly homogeneous expanding background subtracted. Its gradient therefore generates only accelerations relative to the [Hubble flow](../../../../../hubble-flow.md).

For a pressureless fluid, [linearization](../../../../../linearization.md) discards the quadratic advection term, leaving

$$
\dot{\mathbf v}+H\mathbf v=-\frac1a\nabla\Phi,
\qquad
\boxed{\frac d{dt}(a\mathbf v)=-\nabla\Phi.}
$$

In the early [Einstein-de Sitter universe](../../../../../einstein-de-sitter-universe.md), the growing mode has $\Phi(\mathbf x,t)=[D(a)/a]\Phi_i(\mathbf x)$. Integration gives

$$
\boxed{\mathbf v=-\frac{\nabla\Phi_i}{a}\int^t\frac{D(a)}a\,dt.}
$$

The [linear growth factor](../../../../../linear-growth-factor.md) obeys

$$
\ddot D+2H\dot D=4\pi G\bar\rho D.
$$

Since $\bar\rho=\bar\rho_i/a^3$ after choosing $a_i=1$, this is equivalent to

$$
\boxed{\frac{D(a)}a=\frac1{4\pi G\bar\rho_i}
\frac d{dt}\left(a^2\frac{dD}{dt}\right).}
$$

It follows that $a\mathbf v=-a^2\dot D\nabla\Phi_i/(4\pi G\bar\rho_i)$. Since $\dot{\mathbf x}=\mathbf v/a$, one final integration gives the [Zeldovich approximation](../../../../../zeldovich-approximation.md)

$$
\boxed{\mathbf x(t)\simeq\mathbf x_i
-\frac{D(a)}{4\pi G\bar\rho_i}\nabla\Phi_i,}
$$

where an additive initial displacement has been absorbed into $\mathbf x_i$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
