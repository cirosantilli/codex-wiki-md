<h1 id="16a/solution">Solution</h1>

↑ **Parent:** [16A](../16a.md)

The one-dimensional [probability current](../../../../../probability-current.md) is

$$
\boxed{j=\frac{\hbar}{2mi}(\psi^*\psi'-\psi\psi'^*)=\frac\hbar m\operatorname{Im}(\psi^*\psi').}
$$

At a finite jump of the potential, both $\psi$ and $\psi'$ are continuous. A jump in $\psi$ would create a delta derivative in the stationary [Schrödinger equation](../../../../../schrodinger-equation.md), and integrating that equation across an increasingly small interval then shows continuity of $\psi'$. Accordingly impose continuity of both quantities at zero and at $a$.

For an incident wave of positive energy, define $k=\sqrt{2mE}/\hbar$. With no wave incident from the right, the left region has

$$
\psi=Ae^{ikx}+Be^{-ikx},\qquad j_{\mathrm{left}}=\frac{\hbar k}{m}(|A|^2-|B|^2).
$$

The interference terms cancel from the imaginary part in the current formula. If $E>V_0$, let $k_0=\sqrt{2m(E-V_0)}/\hbar$. In the right region,

$$
\psi=Ce^{ik_0(x-a)},\qquad j_{\mathrm{right}}=\frac{\hbar k_0}{m}|C|^2.
$$

For $0<E<V_0$, let $\kappa_0=\sqrt{2m(V_0-E)}/\hbar$. Boundedness at positive infinity excludes the growing exponential, so

$$
\psi=Ce^{-\kappa_0(x-a)},\qquad j_{\mathrm{right}}=0.
$$

The decaying solution has zero current even if its amplitude is nonzero. These exterior forms do not require $E$ to lie on a particular side of $V_1$: in the finite middle layer the solution is oscillatory for $E>V_1$, exponential for $E<V_1$, and linear at $E=V_1$; matching determines the amplitudes.

Define the [reflection coefficient](../../../../../reflection-coefficient.md) as reflected current magnitude divided by incident current, and the [transmission coefficient](../../../../../transmission-coefficient.md) as outward right current divided by incident current. Then

$$
\boxed{R=\frac{|B|^2}{|A|^2},\qquad
T=\begin{cases}\dfrac{k_0|C|^2}{k|A|^2},&E>V_0,\\0,&0<E<V_0.\end{cases}}
$$

The denominator is $j_{\mathrm{incident}}=\hbar k|A|^2/m$. For a real potential, differentiation gives

$$
j'=\frac{\hbar}{2mi}(\psi^*\psi''-\psi\psi''^*)=0
$$

by the stationary [Schrödinger equation](../../../../../schrodinger-equation.md). Continuity at each interface preserves this conserved current, so $j_{\mathrm{left}}=j_{\mathrm{right}}$. Dividing by incident current yields

$$
\boxed{R+T=1,\qquad T=0\text{ and }R=1\text{ if }0<E<V_0.}
$$

There can be penetration into the barrier without transmission to infinity, because the entire right half-line remains classically forbidden.

## ↑ Ancestors (10)

1. [16A](../16a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
