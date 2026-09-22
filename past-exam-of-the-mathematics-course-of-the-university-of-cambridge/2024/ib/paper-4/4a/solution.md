<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

The time-independent [Schrödinger equation](../../../../../schrodinger-equation.md) is

$$
-\frac{\hbar^2}{2m}\psi''(x)+V(x)\psi(x)=E\psi(x).
$$

Integrating it over $(a-\varepsilon,a+\varepsilon)$ and letting $\varepsilon\to0$ shows that $\psi'$ has no jump because $V$ is finite. A jump in $\psi$ would create a delta term in $\psi'$ and hence a [derivative](../../../../../derivative.md) of a delta in $\psi''$, so $\psi$ is also continuous.

For a [bound state](../../../../../bound-state.md) $-V_0<E<0$, define

$$
\eta^2=-\frac{2mE}{\hbar^2},
\qquad
k^2=\frac{2m(E+V_0)}{\hbar^2}.
$$

Then the proposed even [wavefunction](../../../../../wave-function.md) solves the equation away from the interfaces, and

$$
\boxed{k^2+\eta^2=\frac{2mV_0}{\hbar^2}}.
$$

Continuity at $x=a$ gives $B\cos(ka)=Ae^{-\eta a}$, while continuity of the [derivative](../../../../../derivative.md) gives $-Bk\sin(ka)=-A\eta e^{-\eta a}$. Dividing yields the second required relation

$$
\boxed{\eta=k\tan(ka)}.
$$

**Thus the lowest even state of the [finite square well](../../../../../finite-square-well.md) is the first-quadrant intersection, with $0<ka<\pi/2$, of the circle $k^2+\eta^2=2mV_0/\hbar^2$ and the curve $\eta=k\tan(ka)$.**

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
