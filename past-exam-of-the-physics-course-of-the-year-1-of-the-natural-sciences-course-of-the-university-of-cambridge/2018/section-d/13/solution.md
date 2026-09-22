<h1 id="section-d/13/solution">Solution</h1>

↑ **Parent:** [13](../13.md)

**Equation and interpretation.** The supplied equation is the [time-independent Schrödinger equation](../../../../time-independent-schrodinger-equation.md) for a nonrelativistic particle with [mass](../../../../mass.md) $m$ in a prescribed [potential energy](../../../../potential-energy.md) $V(x)$. Equivalently,

$$
\widehat H\psi=E\psi,\qquad
\widehat H=-\frac{\hbar^2}{2m}\frac{d^2}{dx^2}+V(x).
$$

It is an [eigenvalue](../../../../eigenvalue.md) problem for the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md). A stationary energy state has full [wavefunction](../../../../wave-function-split.md) $\Psi(x,t)=\psi(x)e^{-iEt/\hbar}$. By the [Born rule](../../../../born-rule.md), $|\psi(x)|^2dx$ is the probability of finding the particle in a small interval $dx$, with [wavefunction normalization](../../../../wavefunction-normalization.md) $\int_{-\infty}^{\infty}|\psi|^2dx=1$.

**Infinite barriers.** Infinite exterior [potential energy](../../../../potential-energy.md) excludes any finite-energy probability outside the interval. The [infinite square well](../../../../infinite-square-well.md) consequently has $\psi=0$ outside and the hard-wall boundary conditions

$$
\boxed{\psi(0)=\psi(a)=0.}
$$

The interior [wavefunction](../../../../wave-function-split.md) must meet the zero exterior amplitude continuously. Its derivative need not be continuous across an infinite wall; imposing both zero value and zero derivative would eliminate every nonzero interior solution.

**Ground state.** Inside the well $V=0$, so $\psi''+k^2\psi=0$, with $k=\sqrt{2mE}/\hbar$. Its general solution is $A\sin kx+B\cos kx$. The left wall gives $B=0$, and the right wall gives $ka=n\pi$ for $n=1,2,\ldots$. Thus the discrete energy [eigenvalues](../../../../eigenvalue.md) are $E_n=n^2\pi^2\hbar^2/(2ma^2)$. The smallest, $n=1$, is the [ground state](../../../../ground-state.md). Since

$$
\int_0^a\sin^2\frac{\pi x}{a}\,dx=\frac a2,
$$

its normalized [wavefunction](../../../../wave-function-split.md), choosing an irrelevant overall phase to make it positive inside, is

$$
\boxed{\psi_1(x)=\begin{cases}
\sqrt{2/a}\,\sin(\pi x/a),&0<x<a,\\
0,&x\le0\ \text{or}\ x\ge a,
\end{cases}\qquad E_1=\frac{\pi^2\hbar^2}{2ma^2}.}
$$

**Finite barriers.** For a finite step and constant particle [mass](../../../../mass.md), both $\psi$ and $\psi'$ are continuous at $x=0,a$. [Wavefunction matching at a finite potential step](../../../../wavefunction-matching-at-a-finite-potential-step.md) follows by integrating the [Schrödinger equation](../../../../schrodinger-equation.md) across a vanishingly small neighborhood of the step: a bounded potential cannot generate a finite jump in $\psi'$. The bound-state exterior solutions decay rather than vanish identically:

$$
\psi(x)\propto e^{\kappa x}\quad(x<0),\qquad
\psi(x)\propto e^{-\kappa(x-a)}\quad(x>a),\qquad
\kappa=\frac{\sqrt{2m(V_w-E)}}{\hbar}.
$$

Normalizability excludes the growing exterior exponentials. The equivalent interior boundary conditions are $\psi'(0)=\kappa\psi(0)$ and $\psi'(a)=-\kappa\psi(a)$; neither boundary value is zero for the nontrivial [ground state](../../../../ground-state.md).

The [ground state of a finite square well](../../../../ground-state-of-a-finite-square-well.md) remains symmetric about $a/2$ and has no nodes. It bends smoothly into exponential tails at both walls, extending over a larger region than the infinite-well state. Its maximum after normalization is lower for the deep well considered here. When $V_w\gg E$, the penetration length $1/\kappa$ is short, so the two shapes are close except near the walls and in the exterior tails.

<a id="section-d/13/image-normalized-infinite-and-finite-well-ground-states-with-smooth-exponentially-decaying-tails-for-the-finite-well"></a>
![](../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018-ia-physics-q13-well-states.png)

**[Figure 3](#section-d/13/image-normalized-infinite-and-finite-well-ground-states-with-smooth-exponentially-decaying-tails-for-the-finite-well). Normalized infinite- and finite-well ground states, with smooth exponentially decaying tails for the finite well**.

The finite curve is an illustrative exact matched solution with $V_w=10E_{1,\infty}$; no numerical wall height is specified by the question.

**Energy comparison.** The finite barriers relax the confinement, allowing a less rapidly varying interior [wavefunction](../../../../wave-function-split.md) and therefore smaller [kinetic energy](../../../../kinetic-energy.md). More explicitly, the even interior solution is proportional to $\cos[k(x-a/2)]$, and matching to the tails gives $k\tan(ka/2)=\kappa$. The lowest root lies at $0<ka<\pi$, while the infinite well has $ka=\pi$. Hence

$$
\boxed{E_{1,\rm finite}<\frac{\pi^2\hbar^2}{2ma^2}=E_{1,\infty}.}
$$

As $V_w\to\infty$, the tails disappear and the finite-well energy approaches the infinite-well value from below. This comparison uses the same zero of [potential energy](../../../../potential-energy.md) inside both wells.

## ↑ Ancestors (12)

1. [13](../13.md)
2. [Section D](../../section-d.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
