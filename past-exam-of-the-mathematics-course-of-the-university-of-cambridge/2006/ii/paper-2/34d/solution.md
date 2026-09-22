<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

[Heat capacity](../../../../../heat-capacity.md) at fixed volume is $C_V=(\partial E/\partial T)_{V,N}=T(\partial S/\partial T)_{V,N}$. From the [Helmholtz free energy](../../../../../helmholtz-free-energy.md) differential $dF=-S\,dT-P\,dV$ at fixed particle number, equality of mixed derivatives gives $(\partial S/\partial V)_T=(\partial P/\partial T)_V$. Differentiating once more gives

$$
\boxed{\left(\frac{\partial C_V}{\partial V}\right)_T=T\left(\frac{\partial^2P}{\partial T^2}\right)_V.}
$$

For the [canonical partition function](../../../../../canonical-partition-function.md), $F=-k_BT\log Z$, $E=k_BT^2\partial_T\log Z$, and $S=k_B(\log Z+T\partial_T\log Z)$. Thus, for $V>aN$,

$$
\boxed{P=\frac{Nk_BT}{V-aN},\quad E=\frac32Nk_BT,\quad C_V=\frac32Nk_B,}
$$

and

$$
\boxed{S=k_B\left[-\log N!+N\log(V-aN)+\frac{3N}{2}\log(bT)+\frac{3N}{2}\right].}
$$

No Stirling approximation is needed. The [heat capacity](../../../../../heat-capacity.md) is independent of volume, while the [pressure](../../../../../pressure.md) is linear in [temperature](../../../../../temperature.md), so both sides of the Maxwell-derived identity vanish.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
