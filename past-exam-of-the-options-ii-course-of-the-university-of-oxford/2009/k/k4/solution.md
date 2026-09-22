<h1 id="k/k4/solution">Solution</h1>

↑ **Parent:** [K4](../k4.md)

For a short channel slice, the fluid volume per unit length is $b(H+\eta)$ and the axial [volume flux](../../../../volumetric-flow-rate.md) is $b(H+\eta)u$. The quasi-one-dimensional [conservation of mass](../../../../mass-conservation.md) equation is therefore

$$
\partial_t[b(H+\eta)]+\partial_x[b(H+\eta)u]=0.
$$

Neglecting products of perturbations gives $\eta_t+(H/b)(bu)_x=0$. This uses the section-averaged approximation stipulated in the problem; small transverse velocities ensure impermeability of varying-width walls but are not leading axial terms.

The [Euler equations](../../../../euler-equations-for-an-inviscid-fluid-split.md) are $\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\rho^{-1}\nabla p-g\mathbf e_z$. For [irrotational flow](../../../../irrotational-flow.md), $\mathbf u=\nabla\phi$ and $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\nabla\phi|^2/2)$, so

$$
\phi_t+\frac12|\nabla\phi|^2+\frac p\rho+gz=C(t).
$$

At the zero-pressure free surface, linearization about rest gives $\phi_t+g\eta=C(t)$; differentiate in $x$ to get $u_t+g\eta_x=0$. Differentiating the mass equation in time and substituting gives

$$
\boxed{\eta_{tt}=\frac{gH}b(b\eta_x)_x}.
$$

Put $c_0=\sqrt{gH}$. For the exponential width, a time-harmonic amplitude satisfies

$$
N''+\mu N'+\frac{\omega^2}{c_0^2}N=0.
$$

Writing $N=e^{-\mu x/2}V$ removes the first derivative and gives $V''+k^2V=0$, where $k^2=\omega^2/c_0^2-\mu^2/4$. A nonzero real wavenumber, and hence a spatially travelling phase, exists precisely when

$$
\boxed{\omega>\frac\mu2\sqrt{gH}}.
$$

For this case an outward-going solution matching the oscillating boundary is

$$
U(x)=u_0e^{-\mu x/2-ikx},\qquad
N(x)=\frac H\omega(k+i\mu/2)U(x).
$$

Substitution in both linear equations verifies it, and $\operatorname{Im}(U(0)e^{i\omega t})=u_0\sin\omega t$. Below the cutoff the spatial exponents are real, giving evanescent responses; at equality the repeated-root solution has no travelling spatial phase.

This is the [cutoff frequency in an exponentially widening shallow-water channel](../../../../cutoff-frequency-in-an-exponentially-widening-shallow-water-channel.md).

## ↑ Ancestors (12)

1. [K4](../k4.md)
2. [K](../../k.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
