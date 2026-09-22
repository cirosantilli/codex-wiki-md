<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed volume define $E_B=\int_VB^2/(2\mu_0)\,dV$ and $J=\nabla\times B/\mu_0$. Differentiate and use the [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md). The vector identity

$$
B\cdot\nabla\times(u\times B)
=\nabla\cdot[(u\times B)\times B]+(u\times B)\cdot\nabla\times B
$$

then gives the general balance

$$
\frac{dE_B}{dt}=\frac1{\mu_0}\oint_S[(u\cdot B)B-B^2u]\cdot dS
-\int_Vu\cdot(J\times B)\,dV.
$$

The volume term is the work done by the magnetic force on the fluid, with the opposite sign for [magnetic energy](../../../../../../magnetic-energy.md). Under the force-free assumption of part (b), it vanishes, leaving the requested boundary expression. Without that assumption, or another reason for zero net Lorentz work, a boundary-only balance is not generally valid.

For an axisymmetric boundary its normal has no azimuthal component. The [differential rotation](../../../../../../differential-rotation.md) is tangential, so $u\cdot dS=0$, and $u\cdot B=R\Omega B_\phi=\Omega f(\psi)$. Therefore $\dot E_B=\mu_0^{-1}\oint_S\Omega f(\psi)B\cdot dS$. A thin axisymmetric tube between neighboring flux labels carries flux $2\pi d\psi$. Its exit endpoint contributes $+2\pi\Omega_{\rm out}f\,d\psi$ and its entry endpoint contributes $-2\pi\Omega_{\rm in}f\,d\psi$. Pair the endpoints, counting each once, to obtain

$$
\boxed{\frac{dE_B}{dt}=\frac{2\pi}{\mu_0}\int f(\psi)\Delta\Omega(\psi)\,d\psi,
\quad\Delta\Omega=\Omega_{\rm out}-\Omega_{\rm in}.}
$$

The endpoint convention fixes the sign. Include each connected tube segment through $V$ once; a field line with no boundary crossing contributes nothing. This is [magnetic-energy injection by differential boundary rotation](../../../../../../magnetic-energy-injection-by-differential-boundary-rotation.md). A common angular [velocity](../../../../../../velocity.md) at both ends produces no such injection.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
