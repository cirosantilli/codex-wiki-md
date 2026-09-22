<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Seek the travelling forced component of the [surface elevation](../../../../surface-elevation.md) in the form $\eta=A\cos\chi$, where $\chi=x-ct$ and $A$ is a signed coefficient. The forcing has [wavenumber](../../../../wavenumber.md) one. [Separation of variables](../../../../separation-of-variables.md) in the [Laplace equation](../../../../laplace-equation.md), followed by the bed [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md), gives

$$
\phi=B\cosh(y+h)\sin\chi.
$$

Since $\eta_t=Ac\sin\chi$, the surface [kinematic boundary condition](../../../../kinematic-boundary-condition.md) requires $B\sinh h=Ac$, so

$$
\boxed{\phi=\frac{Ac}{\sinh h}\cosh(y+h)\sin(x-ct)}.
$$

At $y=0$, $\phi_t=-Ac^2\coth h\cos\chi$. The dynamic member of the [linearized free-surface boundary conditions](../../../../linearized-free-surface-boundary-conditions.md) therefore becomes

$$
A(g-c^2\coth h)+\frac{p_1}{\rho}=0.
$$

Consequently the signed response and the nonnegative [amplitude](../../../../wave-amplitude.md) are

$$
\boxed{A=-\frac{p_1}{\rho(g-c^2\coth h)},\qquad
a(c)=|A|=\frac{p_1}{\rho\,|g-c^2\coth h|}}.
$$

The [travelling-pressure response of finite-depth surface gravity waves](../../../../travelling-pressure-response-of-finite-depth-surface-gravity-waves.md) is opposite in phase to the imposed [pressure](../../../../pressure-split.md) below the resonant speed and in phase above it. These expressions describe the travelling forced component; freely propagating [surface gravity waves](../../../../surface-gravity-wave.md) can be superposed to meet additional [initial conditions](../../../../initial-condition.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
