<h1 id="k/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The exact free-surface kinematic condition is $\eta_t+\phi_x\eta_x=\phi_y$ evaluated at $y=\eta$. Linearizing about a flat [surface](../../../../topological-surface-split.md) at rest drops products of small quantities and evaluates at $y=0$, giving $\phi_y=\eta_t$. [Bernoulli's equation](../../../../bernoulli-equation.md) with constant atmospheric pressure gives $\phi_t+g\eta=0$ to the same order. The rigid bed has no normal flow, hence $\phi_y=0$ at $y=-h$.

In the fluid, [incompressibility](../../../../incompressible-flow.md) and the velocity-potential representation give $\Delta\phi=0$. For $k>0$, take

$$
\phi(x,y,t)=\frac{Ag}{\omega}
\frac{\cosh(k(y+h))}{\cosh(kh)}\sin(kx-\omega t).
$$

It is harmonic, satisfies the bed condition and the linear dynamic condition. At the [surface](../../../../topological-surface-split.md) its vertical derivative is $Agk\tanh(kh)\sin(kx-\omega t)/\omega$, while $\eta_t=A\omega\sin(kx-\omega t)$. Therefore the kinematic condition is equivalent to

$$
\boxed{\omega^2=gk\tanh(kh),\qquad
c=\frac\omega k=\sqrt{\frac gk\tanh(kh)}.}
$$

Finally $\tanh q=q-q^3/3+O(q^5)$. Taking the square root gives

$$
\boxed{c=\sqrt{gh}\left(1-\frac16k^2h^2+O((kh)^4)\right).}
$$

The first term is nondispersive shallow-water speed; the next term is the leading finite-depth dispersion correction.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [K](../../k.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
