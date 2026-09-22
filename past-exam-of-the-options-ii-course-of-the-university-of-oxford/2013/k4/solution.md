<h1 id="k4/solution">Solution</h1>

↑ **Parent:** [K4](../k4.md)

The factor $\eta_{xx}/(1+\eta_x^2)^{3/2}$ is the signed [curvature](../../../curvature.md) of the graph, so the pressure jump is surface tension times curvature, the planar [Young–Laplace equation](../../../young-laplace-equation.md).

Take total velocity potentials $\Phi_-=\phi_-$ and $\Phi_+=Ux+\phi_+$. Each disturbance potential satisfies the [Laplace equation](../../../laplace-equation.md). The interface moves with the fluid: for $F=y-\eta(x,t)$, the material equation $F_t+v\cdot\nabla F=0$ gives $\eta_t+u\eta_x=v_y$. Keeping only first-order terms and evaluating at $y=0$ yields

$$
\boxed{\phi_{-,y}=\eta_t,\qquad\phi_{+,y}=\eta_t+U\eta_x.}
$$

The unsteady [Bernoulli equation](../../../bernoulli-equation.md) is $\Phi_t+|\nabla\Phi|^2/2+p/\rho=C(t)$, with any common gravitational contribution canceling across this equal-density interface. Subtracting the basic flow and linearizing gives $p'_-= -\rho\phi_{-,t}$ and $p'_+=-\rho(\phi_{+,t}+U\phi_{+,x})$. The linearized pressure jump is $T\eta_{xx}$. Hence

$$
\boxed{\phi_{-,t}-(\phi_{+,t}+U\phi_{+,x})=(T/\rho)\eta_{xx}.}
$$

Use complex modes with real parts understood:

$$
\eta=Ae^{i(kx-\omega t)},\qquad
\phi_-=B_-e^{ky}e^{i(kx-\omega t)},\quad
\phi_+=B_+e^{-ky}e^{i(kx-\omega t)}.
$$

The decaying vertical factors solve the Laplace equation in their respective half-planes. The kinematic conditions give $B_-=-i\omega A/k$ and $B_+=i(\omega-kU)A/k$. Substitution in the dynamic condition gives

$$
\boxed{\omega^2+(\omega-kU)^2=\frac T\rho k^3,\qquad
\omega=\frac{kU}{2}\pm\sqrt{\frac{Tk^3}{2\rho}-\frac{k^2U^2}{4}}.}
$$

When the discriminant is nonnegative, the [phase speeds](../../../phase-speed.md) are $U/2\pm\sqrt{Tk/(2\rho)-U^2/4}$. They are two dispersive capillary-wave branches advected by the mean velocity $U/2$.

When $\boxed{U^2>2Tk/\rho}$, the frequencies are complex conjugates and one mode grows exponentially, with growth rate $k\sqrt{U^2/4-Tk/(2\rho)}$. This is [Kelvin-Helmholtz instability](../../../kelvin-helmholtz-instability.md). Surface tension stabilizes sufficiently short waves, while for any nonzero shear, sufficiently long waves are unstable in this gravity-free equal-density model. A real cosine with real frequency describes the stable branches; the unstable case is represented by the real part of the corresponding growing complex mode.

## ↑ Ancestors (11)

1. [K4](../k4.md)
2. [2013](../../2013-split.md)
3. [Past exam of the options II course of the University of Oxford](../../split.md)
4. [Options II course of the University of Oxford](../../../options-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
