<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

An [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) has $\dot\phi=0$ and $\boxed{J'(\phi_0)=0}$. Since $K(\phi_0)>0$, the linearized displacement $\psi=\phi-\phi_0$ satisfies

$$
K(\phi_0)\ddot\psi+J''(\phi_0)\psi=0.
$$

Thus $J''(\phi_0)>0$ gives a [stable equilibrium](../../../../../../stable-equilibrium.md), while $J''(\phi_0)<0$ gives an unstable [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md). More generally, a [strict local minimum](../../../../../../strict-local-minimum.md) of $J$ is sufficient for stability by the conserved first [integral](../../../../../../integral-split.md) in [b](../b.md). **When $J''(\phi_0)=0$, the second-[derivative](../../../../../../derivative.md) test alone is inconclusive**, and the local shape of $J$ must be examined.

For the specified [ellipse](../../../../../../ellipse.md), put $D=1+e\cos\phi>0$. Direct [differentiation](../../../../../../differentiation.md) gives

$$
f'=\frac{\cos\phi+e}{D^2},\qquad q'=-\frac{\sin\phi}{D^2}.
$$

Consequently, with $\eta=g/\omega^2$ and $\omega\ne0$,

$$
J'(\phi)=\frac{\omega^2\sin\phi}{D^3}\left[\eta(1+e\cos\phi)-(\cos\phi+e)\right].
$$

Two [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) always occur at $\boxed{\phi=0,\pi\pmod{2\pi}}$. Any further [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) must satisfy

$$
\boxed{\cos\phi=\frac{\eta-e}{1-e\eta}.}
$$

To decide exactly when this is possible, view the [equation](../../../../../../equation.md) as $\eta=(c+e)/(1+ec)$ with $c=\cos\phi$. Its [derivative](../../../../../../derivative.md) $(1-e^2)/(1+ec)^2$ is positive on $[-1,1]$, and it takes endpoint values $-1$ and $1$. Since $g>0$ implies $\eta>0$, the complete list is:

- If $0<\eta<1$, there are **four distinct [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) modulo $2\pi$**: $0$, $\pi$, and $\displaystyle\pm\arccos\frac{\eta-e}{1-e\eta}$. For $0<\eta<e$ the additional positive [angle](../../../../../../angle.md) lies in $(\pi/2,\pi)$; at $\eta=e$ the additional pair is $\pm\pi/2$; for $e<\eta<1$ it lies in $(0,\pi/2)$.
- If $\eta=1$, the additional pair merges with $\phi=0$, leaving **two distinct [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md)**, $0$ and $\pi$.
- If $\eta>1$, there are **only the two [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md)** $0$ and $\pi$. In particular, $\eta=1/e$ does not introduce a missing case: the undivided bracket is then the positive constant $1/e-e$, so there is no extra root.

These are positions of the bead at rest relative to the rotating hoop. No stability classification of the particular [ellipse](../../../../../../ellipse.md) is needed.

## ↑ Ancestors (12)

1. [c](../c.md)
2. [6](../../6.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
