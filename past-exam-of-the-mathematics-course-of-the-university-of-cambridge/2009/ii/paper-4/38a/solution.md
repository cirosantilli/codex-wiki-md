<h1 id="38a/solution">Solution</h1>

↑ **Parent:** [38A](../38a.md)

In the shock rest frame the upstream and downstream speed magnitudes are $U$ and $U-V$. Denote the downstream density by $\rho_2$, and write $v_i=1/\rho_i$ for specific volume. The [Rankine-Hugoniot conditions for a perfect gas](../../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md) express conservation of mass, momentum and total energy:

$$
j=\rho_1U=\rho_2(U-V),\qquad p_1+j^2v_1=p_2+j^2v_2,
$$



$$
e_1+p_1v_1+\frac12j^2v_1^2=e_2+p_2v_2+\frac12j^2v_2^2,
\qquad e_i=\frac{p_iv_i}{\gamma-1}.
$$

These follow by balancing the respective fluxes across a stationary infinitesimal control volume around the [shock wave](../../../../../shock-wave.md). The mass relation also gives $V=j(v_1-v_2)$, and momentum gives $j^2(v_1-v_2)=p_2-p_1$.

Eliminate the kinetic-energy difference in the energy condition using momentum:

$$
e_2-e_1=p_1v_1-p_2v_2+\frac12(p_2-p_1)(v_1+v_2)
=\frac12(p_1+p_2)(v_1-v_2).
$$

Substitute the given perfect-gas internal energy and collect the coefficients of $v_1,v_2$:

$$
[(\gamma+1)p_2+(\gamma-1)p_1]v_2
=[(\gamma-1)p_2+(\gamma+1)p_1]v_1.
$$

Hence

$$
v_1-v_2=\frac{2(p_2-p_1)}{\rho_1[(\gamma+1)p_2+(\gamma-1)p_1]}.
$$

Finally $V^2=j^2(v_1-v_2)^2=(p_2-p_1)(v_1-v_2)$ gives

$$
\boxed{V^2=\frac{(p_2-p_1)^2}{\rho_1[(\gamma+1)p_2/2+(\gamma-1)p_1/2]}.}
$$

For the advancing piston choose the compressive branch $p_2>p_1$, $U>V>0$; the algebraic squared relation alone does not specify that branch.

## ↑ Ancestors (10)

1. [38A](../38a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
