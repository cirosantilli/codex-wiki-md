<h1 id="k/k4/solution">Solution</h1>

↑ **Parent:** [K4](../k4.md)

A material interface obeys $\eta_t+\phi_{j,x}\eta_x=\phi_{j,y}$ at its actual height. Keeping only first-order terms and evaluating at the undisturbed interface gives $\phi_{1,y}=\phi_{2,y}=\eta_t$ at $y=0$. Linearized unsteady Bernoulli gives the pressure perturbation $-\rho_j(\phi_{j,t}+g\eta)$, after absorbing time-only constants into the potentials. Pressure [continuity](../../../../continuous-function.md) therefore gives

$$
\boxed{\rho_1\phi_{1,t}-\rho_2\phi_{2,t}+g(\rho_1-\rho_2)\eta=0\quad\text{at }y=0}.
$$

For $\vartheta=kx-\omega t$, choose potentials decaying away from the interface:

$$
\phi_1=\frac{A\omega}{k}e^{ky}\sin\vartheta\quad(y<0),\qquad
\phi_2=-\frac{A\omega}{k}e^{-ky}\sin\vartheta\quad(y>0).
$$

They are harmonic and their normal derivatives equal $A\omega\sin\vartheta=\eta_t$ at zero. The dynamic condition reduces to

$$
\boxed{\omega^2=gk\frac{\rho_1-\rho_2}{\rho_1+\rho_2},\qquad c=\frac\omega k=\sqrt{\frac{g(\rho_1-\rho_2)}{k(\rho_1+\rho_2)}}}.
$$

If the denser fluid is above, the squared frequency is negative. The corresponding perturbations grow or decay exponentially instead of oscillating: this is [Rayleigh-Taylor instability](../../../../rayleigh-taylor-instability.md), with growing rate $\sqrt{gk(\rho_2-\rho_1)/(\rho_1+\rho_2)}$ in the ideal model without surface tension.

## ↑ Ancestors (12)

1. [K4](../k4.md)
2. [K](../../k.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
