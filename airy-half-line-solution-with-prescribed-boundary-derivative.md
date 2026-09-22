# Airy half-line solution with prescribed boundary derivative

↑ **Parent:** [Airy resolvent kernel](airy-resolvent-kernel.md)

For $u_t+u_{xxx}=0$ on $x>0$, define $V(x,p)=\int_0^\infty R_p(x-y)u_0(y)dy$ and let $G$ be the time [Laplace transform](laplace-transform.md) of $u_x(0,t)$. The transformed solution with spatial decay is

$$
U(x,p)=V(x,p)+\frac{e^{-p^{1/3}x}}{p^{1/3}}\left[V_x(0,p)-G(p)\right].
$$

Only one [characteristic root](characteristic-root-of-a-constant-coefficient-differential-equation.md) has negative [real part](real-part.md), so one scalar boundary derivative fixes the remaining homogeneous mode. The [Bromwich inversion formula](bromwich-inversion-formula.md) supplies an [integral representation](integral-representation.md) involving only the initial and boundary data. For general [linear differential equations](linear-differential-equation.md) on a half-line, the number and form of the necessary boundary data depend on the decaying spatial roots; [Fokas and Wang](https://arxiv.org/abs/1409.2083) study the corresponding boundary maps for linear dispersive equations.

## ↑ Ancestors (7)

1. [Airy resolvent kernel](airy-resolvent-kernel.md)
2. [Airy equation](airy-equation.md)
3. [Lax pair](lax-pair.md)
4. [Integrable systems](integrable-systems-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
