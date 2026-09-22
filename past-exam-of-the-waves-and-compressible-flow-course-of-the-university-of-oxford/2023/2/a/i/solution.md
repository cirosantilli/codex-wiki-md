<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the density and pressure as $\rho_0(z)+\rho'(x,z,t)$ and $p_0(z)+p'(x,z,t)$, respectively. The background satisfies [hydrostatic balance](../../../../../hydrostatic-balance.md), $p_0'=-g\rho_0$, and $\rho_0'/\rho_0=-\alpha$. Linearizing the [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid-split.md), [incompressibility](../../../../../incompressible-flow.md) and advection of density gives

$$
u_x+w_z=0,\qquad \rho_0u_t=-p'_x,\qquad \rho_0w_t=-p'_z-g\rho',\qquad \rho'_t=\alpha\rho_0w.
$$

Differentiate the horizontal equation in $x$ and use [incompressibility](../../../../../incompressible-flow.md) to obtain $p'_{xx}=\rho_0w_{zt}$. Differentiate the vertical equation in time and twice in $x$:

$$
\rho_0w_{ttxx}=-\partial_z(\rho_0w_{ztt})-\alpha g\rho_0w_{xx}.
$$

Dividing by $\rho_0>0$ gives the equation for [internal waves in an exponentially stratified incompressible fluid](../../../../../internal-waves-in-an-exponentially-stratified-incompressible-fluid.md),

$$
\boxed{\partial_t^2(\nabla^2w-\alpha w_z)+\alpha g\,w_{xx}=0}.
$$

The first-derivative term retains the variation of inertial density with height; no [Boussinesq approximation](../../../../../boussinesq-approximation.md) has been made.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the waves and compressible flow course of the University of Oxford](../../../../split.md)
6. [Waves and compressible flow course of the University of Oxford](../../../../../waves-and-compressible-flow-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
