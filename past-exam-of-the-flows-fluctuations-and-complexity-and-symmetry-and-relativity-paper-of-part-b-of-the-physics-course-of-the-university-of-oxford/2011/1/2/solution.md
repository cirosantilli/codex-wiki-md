<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For planar [incompressible flow](../../../../incompressible-flow.md), $u_x+w_z=0$. Locally this permits a [streamfunction](../../../../stream-function.md) with $u=\psi_z$, $w=-\psi_x$, because equality of the mixed derivatives enforces [incompressibility](../../../../incompressible-flow.md). The remaining component of the [curl](../../../../curl.md) is $u_z-w_x=\psi_{zz}+\psi_{xx}$, so [irrotational flow](../../../../irrotational-flow.md) requires [Laplace's equation](../../../../laplace-equation.md) for $\psi$.

Put $K=\pi/b$. The sinusoidal contribution to the supplied [streamfunction](../../../../stream-function.md) has $\psi_{xx}=U_0aK^2\cos(Kx)e^{-Kz}$ and $\psi_{zz}=-U_0aK^2\cos(Kx)e^{-Kz}$; the linear term is also harmonic. Hence

$$
u=U_0[1+aK\cos(Kx)e^{-Kz}],\qquad
w=-U_0aK\sin(Kx)e^{-Kz}.
$$

As $z\to\infty$, these approach the specified [uniform flow](../../../../uniform-flow.md), $(u,w)=(U_0,0)$.

The impermeability [kinematic boundary condition](../../../../kinematic-boundary-condition.md) is $w=u\,z_s'(x)$ on $z=z_s(x)$, equivalently $\psi$ is constant on the wall. For $aK\ll1$, evaluating the perturbed velocities at $z=0$ gives $w=-U_0aK\sin(Kx)=U_0z_s'$ to first order. The residual is of order $U_0(aK)^2$. Equivalently $\psi(x,z_s)=U_0a\cos(Kx)[1-e^{-Ka\cos(Kx)}]=O(U_0Ka^2)$. The surface velocity is

$$
\boxed{u_s=U_0[1+aK\cos(Kx)e^{-Ka\cos(Kx)}]
=U_0[1+aK\cos(Kx)]+O(U_0(aK)^2).}
$$

The first expression is the supplied approximate field evaluated exactly at the wall; its accuracy as a wall-flow solution is still only first order in $a/b$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the flows, fluctuations and complexity and symmetry and relativity paper of Part B of the physics course of the University of Oxford](../../../split.md)
5. [Flows, fluctuations and complexity and symmetry and relativity paper of Part B of the physics course of the University of Oxford](../../../../flows-fluctuations-and-complexity-and-symmetry-and-relativity-paper-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
