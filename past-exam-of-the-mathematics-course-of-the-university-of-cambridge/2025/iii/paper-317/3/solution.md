<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $P=K\rho^2$, the specific enthalpy is

$$
H(\rho)=\int_0^\rho\frac{dP}{\rho'}=2K\rho.
$$

Hydrostatic equilibrium says $\nabla(H+\Phi)=0$. Taking a Laplacian and using the gravitational [Poisson equation](../../../../../poisson-equation.md) gives the [Helmholtz equation](../../../../../helmholtz-equation.md)

$$
\boxed{\nabla^2\rho+k^2\rho=0},
\qquad
k^2=\frac{2\pi G}{K}.
$$

For a spherical star, regularity at the centre selects the $n=1$ [stellar polytrope](../../../../../stellar-polytrope.md)

$$
\rho(r)=\rho_c\frac{\sin kr}{kr}.
$$

Its first zero is $kR=\pi$, hence

$$
\boxed{R=\frac\pi k=\left(\frac{K\pi}{2G}\right)^{1/2}}.
$$

Direct integration gives $M=4\rho_cR^3/\pi$, and therefore

$$
\boxed{\frac{\bar\rho}{\rho_c}
=\frac{3M}{4\pi R^3\rho_c}=\frac3{\pi^2}}.
$$

On the cube, the separated positive solution

$$
\rho(x,y,z)=\rho_c
\sin\frac{\pi x}{L}
\sin\frac{\pi y}{L}
\sin\frac{\pi z}{L}
$$

vanishes on all six faces. It solves the same Helmholtz equation when

$$
\frac{3\pi^2}{L^2}=k^2,
\qquad
L=\left(\frac{3\pi K}{2G}\right)^{1/2}.
$$

The mean of each sine over $[0,L]$ is $2/\pi$, so

$$
\boxed{\frac{\bar\rho}{\rho_c}=\left(\frac2\pi\right)^3=\frac8{\pi^3}}.
$$

The interior fields formally solve the local structure equations, but an isolated fluid surface must be an equipotential and its interior gravitational field must match a decaying exterior solution with continuous normal derivative. A cube does not satisfy the global free-boundary conditions for a nonrotating self-gravitating barotrope. Such sharp planar faces and edges are also not observed in stars; ordinary pressure and gravity smooth the body toward a sphere.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
