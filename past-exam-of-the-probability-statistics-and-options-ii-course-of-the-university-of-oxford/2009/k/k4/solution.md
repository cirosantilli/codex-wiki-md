<h1 id="k/k4/solution">Solution</h1>

↑ **Parent:** [K4](../k4.md)

Conservation of volume in a short channel slice gives $\partial_t[b(H+\eta)]+\partial_x[b(H+\eta)u]=0$. Keeping first-order terms in $u,\eta$ gives $\boxed{\eta_t+(H/b)(bu)_x=0}$.

Euler's momentum equation is $\partial_tv+(v\cdot\nabla)v=-\nabla p/\rho-g\hat z$. For irrotational flow $v=\nabla\phi$, integration gives the [Unsteady Bernoulli equation](../../../../unsteady-bernoulli-equation.md) $\phi_t+|\nabla\phi|^2/2+p/\rho+gz=C(t)$. On the zero-pressure surface $z=\eta$, linearization gives $\phi_t+g\eta=C(t)$. Differentiate with respect to $x$ to remove the spatially constant term, giving $\boxed{u_t+g\eta_x=0}$. These are the cross-sectionally averaged shallow-water approximations encoded in the stated assumptions.

Differentiate the [mass](../../../../mass.md) equation in time and use the momentum equation to get

$$
\boxed{\eta_{tt}=\frac{gH}b(b\eta_x)_x.}
$$

For $b=b_0e^{\mu x}$ this is $\eta_{tt}=gH(\eta_{xx}+\mu\eta_x)$. A time-harmonic amplitude $N(x)$ satisfies $N''+\mu N'+\omega^2N/(gH)=0$. Write $N=e^{-\mu x/2}W$ to obtain

$$
W''+\left(\frac{\omega^2}{gH}-\frac{\mu^2}4\right)W=0.
$$

Spatially oscillating waves therefore occur exactly when the coefficient is positive:

$$
\boxed{\omega>\frac\mu2\sqrt{gH}.}
$$

Below threshold the solutions have real exponential spatial factors and are evanescent rather than propagating; equality gives the zero-[wavenumber](../../../../wavenumber.md) threshold. For a concrete outgoing wave let $\kappa=\sqrt{\omega^2/(gH)-\mu^2/4}>0$. Then $U(x)=u_0e^{-\mu x/2}e^{-i\kappa x}$ obeys the oscillating boundary condition, and $N(x)=H(\kappa+i\mu/2)U(x)/\omega$ follows from [mass](../../../../mass.md) conservation. The phase $\omega t-\kappa x$ moves into $x>0$.

## ↑ Ancestors (12)

1. [K4](../k4.md)
2. [K](../../k.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
