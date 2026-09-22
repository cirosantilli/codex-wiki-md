<h1 id="34e/solution">Solution</h1>

↑ **Parent:** [34E](../34e.md)

In the [canonical ensemble](../../../../../canonical-ensemble.md), put $\beta=(k_BT)^{-1}$ and $Z=\sum_j e^{-\beta E_j}$. For a temperature-independent observable $A$, differentiating its normalized expectation gives $\partial_\beta\langle A\rangle=-\langle AE\rangle+\langle A\rangle\langle E\rangle$. Taking $A=E$ yields $\partial_\beta\langle E\rangle=-\operatorname{Var}E$. Since $\partial_\beta=-k_BT^2\partial_T$ at fixed volume,

$$
\boxed{\langle(E-\langle E\rangle)^2\rangle=k_BT^2C_V.}
$$

Differentiating $\langle E^2\rangle-\langle E\rangle^2$ with the same rule gives minus $\langle E^3\rangle-3\langle E\rangle\langle E^2\rangle+2\langle E\rangle^3$, namely minus the third [central moment](../../../../../central-moment.md). Thus

$$
\boxed{\langle(E-\langle E\rangle)^3\rangle=k_B^2\left[T^4\left(\frac{\partial C_V}{\partial T}\right)_V+2T^3C_V\right].}
$$

These identities exhibit the second and third energy [cumulants](../../../../../cumulant.md) as successive derivatives of $\log Z$.

For the monatomic [ideal gas](../../../../../ideal-gas.md), $\langle E\rangle=3Nk_BT/2$, $C_V=3Nk_B/2$ and $\partial_TC_V=0$. The [variance](../../../../../variance-split.md) is $3N(k_BT)^2/2$ and the third [central moment](../../../../../central-moment.md) is $3N(k_BT)^3$. Division by the corresponding mean-energy powers gives

$$
\boxed{\frac{\langle(E-\langle E\rangle)^2\rangle}{\langle E\rangle^2}=\frac2{3N},\qquad\frac{\langle(E-\langle E\rangle)^3\rangle}{\langle E\rangle^3}=\frac8{9N^2}.}
$$

## ↑ Ancestors (10)

1. [34E](../34e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
