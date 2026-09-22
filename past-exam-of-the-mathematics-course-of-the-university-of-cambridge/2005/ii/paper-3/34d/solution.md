<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

Periodic boundary conditions give wavevectors $(2\pi/L)(n_x,n_y)$. In the continuum, large-box limit each state occupies area $(2\pi/L)^2$ in wavevector space. A circular annulus therefore contains $[L^2/(2\pi)^2]2\pi k\,dk$ spinless states. Since $\epsilon=\hbar^2k^2/(2m)$, the [density of states](../../../../../density-of-states.md) is

$$
\boxed{g_0=\frac{mL^2}{2\pi\hbar^2}.}
$$

At finite $L$ the exact spectrum is discrete; this formula is its continuum density.

With electron spin the two Zeeman branches are $\epsilon_{\mathrm{kin}}\mp\mu H$. The requested calculation includes this spin coupling and neglects orbital coupling to the field; for a perpendicular field, [Landau levels](../../../../../landau-level.md) would change the result. It is appropriate for a field parallel to the [ideal](../../../../../ideal.md) two-dimensional plane, or for the stated spin-only model. Taking $\mu H\geq0$, the lower branch starts at $-\mu H$, and the upper one at $\mu H$, so

$$
\boxed{g(\epsilon)=\begin{cases}0,&\epsilon<-\mu H,\\g_0,&-\mu H<\epsilon<\mu H,\\2g_0,&\epsilon>\mu H.\end{cases}}
$$

Construct the ground state by filling the lowest one-electron levels subject to the [Pauli exclusion principle](../../../../../pauli-exclusion-principle.md). If the [Fermi energy](../../../../../fermi-energy.md) $\epsilon_F$ exceeds $\mu H$, the two populations are $N_+=g_0(\epsilon_F+\mu H)$ and $N_-=g_0(\epsilon_F-\mu H)$. Consequently

$$
\boxed{N=2g_0\epsilon_F=\frac{mL^2}{\pi\hbar^2}\epsilon_F,\qquad
M=\mu(N_+-N_-)=\frac{\mu^2mL^2}{\pi\hbar^2}H.}
$$

The [ground-state energy](../../../../../ground-state-energy.md), including the Zeeman term, follows by integrating the energy over each occupied branch:

$$
E_0=g_0\int_{-\mu H}^{\epsilon_F}\epsilon\,d\epsilon+
 g_0\int_{\mu H}^{\epsilon_F}\epsilon\,d\epsilon
=g_0(\epsilon_F^2-\mu^2H^2)
=\boxed{\frac{\pi\hbar^2N^2}{2mL^2}-\frac12MH.}
$$

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
