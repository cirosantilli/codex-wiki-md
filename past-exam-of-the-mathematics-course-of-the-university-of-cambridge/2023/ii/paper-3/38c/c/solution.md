<h1 id="38c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Integrating the incompressible [continuity equation](../../../../../../continuity-equation.md) $u_x+v_y=0$ across the moving gap, with $v(x,0)=0$ and $v(x,h)=-V$, gives the [Reynolds lubrication equation](../../../../../../reynolds-equation.md)

$$
\frac{dQ}{dx}=V.
$$

Hence

$$
Q=Vx+C
$$

for a constant $C$, and the flux formula from part (b) gives

$$
p_x=\frac{6\mu U}{h^2}
-\frac{12\mu(Vx+C)}{h^3}.
$$

Define the spatial mean

$$
\langle f\rangle=\frac1L\int_0^Lf(x)\,dx.
$$

Because both ends meet fluid at pressure $p_0$, the [pressure recovery condition in lubrication flow](../../../../../../pressure-recovery-condition-in-lubrication-flow.md) is

$$
0=p(L)-p(0)=\int_0^Lp_x\,dx.
$$

It determines

$$
C=\frac U2
\frac{\langle h^{-2}\rangle}{\langle h^{-3}\rangle}
-V\frac{\langle xh^{-3}\rangle}{\langle h^{-3}\rangle}.
$$

Therefore the requested [pressure gradient in a translating and squeezing finite gap](../../../../../../pressure-gradient-in-a-translating-and-squeezing-finite-gap.md) is

$$
\boxed{
p_x=\frac{6\mu U}{h^2}
-\frac{12\mu}{h^3}
\left[
Vx+\frac U2
\frac{\langle h^{-2}\rangle}{\langle h^{-3}\rangle}
-V\frac{\langle xh^{-3}\rangle}{\langle h^{-3}\rangle}
\right].}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [38C](../../38c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
