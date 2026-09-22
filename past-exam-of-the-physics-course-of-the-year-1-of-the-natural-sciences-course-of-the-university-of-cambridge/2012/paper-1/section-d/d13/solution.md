<h1 id="section-d/d13/solution">Solution</h1>

↑ **Parent:** [D13](../d13.md)

Here $V(x)$ is [potential energy](../../../../../potential-energy.md), $E$ is the stationary-state total [energy eigenvalue](../../../../../energy-eigenvalue-split.md), and $\psi(x)$ is its spatial [wavefunction](../../../../../wave-function-split.md). [Wavefunction normalization](../../../../../wavefunction-normalization.md) gives $\int|\psi|^2dx=1$, and $|\psi|^2dx$ is the [probability](../../../../../probability.md) of finding the particle in $dx$.

A [bound state](../../../../../bound-state.md) requires $-V_0<E<0$. Inside the well the equation is $\psi''=-k^2\psi$, whereas outside it is $\psi''=q^2\psi$, with

$$
\boxed{k=\frac{\sqrt{2m(E+V_0)}}\hbar,\qquad q=\frac{\sqrt{-2mE}}\hbar.}
$$

The [ground state](../../../../../ground-state.md) is even and has no [node](../../../../../node-dynamical-systems.md), selecting $\cos(kx)$ inside. Normalizability selects decaying, not growing, exterior exponentials. Continuity of $\psi$ and $\psi'$ gives

$$
A\cos(ka/2)=Ce^{-qa/2},\qquad k\tan(ka/2)=q.
$$

The first [excited state](../../../../../excited-state.md), if present, is odd: a [sine](../../../../../sine.md) inside and opposite-sign decaying tails outside. Matching gives $-k_1\cot(k_1a/2)=q_1>0$. On its first odd branch, $\pi/2<k_1a/2<\pi$, hence $k_1a>\pi$. Since $k_1^2<2mV_0/\hbar^2$, existence requires

$$
\boxed{V_0>\frac{\pi^2\hbar^2}{2ma^2}.}
$$

This is the [first odd bound-state threshold of a square well](../../../../../first-odd-bound-state-threshold-of-a-square-well.md). There is no excited [bound state](../../../../../bound-state.md) below that threshold; equality gives a non-normalizable zero-energy limiting state, not an extra [bound state](../../../../../bound-state.md).

<a id="section-d/d13/image-original-finite-well-wavefunctions-an-even-nodeless-ground-state-and-an-odd-excited-state-in-a-deeper-illustrative-well"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1-ia2012-well-states.png)

**[Figure 4](#section-d/d13/image-original-finite-well-wavefunctions-an-even-nodeless-ground-state-and-an-odd-excited-state-in-a-deeper-illustrative-well). Original finite-well wavefunctions: an even nodeless ground state and an odd excited state in a deeper illustrative well**.

For the numerical well,

$$
V_0=\frac{\hbar^2(k^2+q^2)}{2m}=8.04\,\mathrm{eV}\simeq8.0\,\mathrm{eV},\qquad
\boxed{E=-\frac{\hbar^2q^2}{2m}=-4.95\,\mathrm{eV}.}
$$

The [exterior probability of a symmetric finite-well state](../../../../../exterior-probability-of-a-symmetric-finite-well-state.md) includes both tails:

$$
\boxed{P_{\rm out}=2\int_{a/2}^{\infty}C^2e^{-2qx}\,dx
=\frac{C^2}{q}e^{-qa}=0.178\simeq17.8\%.}
$$

The threshold is $9.40\,\mathrm{eV}$, exceeding the well depth, so **there is no excited [bound state](../../../../../bound-state.md)**. The rounded supplied coefficients integrate to $0.9973$ rather than exactly one; this rounding does not change the quoted [probability](../../../../../probability.md) precision materially.

## ↑ Ancestors (13)

1. [D13](../d13.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
