<h1 id="9d/solution">Solution</h1>

↑ **Parent:** [9D](../9d.md)

For $T=\frac12\dot q^T T\dot q$ and $V=\frac12q^T Vq$, where the [matrices](../../../../../matrix.md) are symmetric and constant, the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) give $T\ddot q+Vq=0$. A [normal mode](../../../../../normal-mode.md) $q=v e^{i\omega t}$ therefore solves $(V-\omega^2T)v=0$.

A string segment of horizontal length $b$ has extension $\sqrt{b^2+(\Delta q)^2}-b=(\Delta q)^2/(2b)+O((\Delta q)^4)$. Multiplying by the tension $S$ and using $m=1$ and $S/b=1$, the quadratic [kinetic energy](../../../../../kinetic-energy.md) and [potential energy](../../../../../potential-energy.md) are

$$
T=\tfrac12(\dot q_1^2+\dot q_2^2+\dot q_3^2),\qquad V=\tfrac12\{q_1^2+(q_1-q_2)^2+(q_2-q_3)^2+q_3^2\}.
$$

Thus $T=I$ and $V=\begin{pmatrix}2&-1&0\\-1&2&-1\\0&-1&2\end{pmatrix}$. Taking $v_i=\sin(ij\pi/4)$, $i=1,2,3$, gives the three [eigenvalues](../../../../../eigenvalue.md) $2-2\cos(j\pi/4)$, $j=1,2,3$. The [normal mode](../../../../../normal-mode.md) frequencies are

$$
\boxed{\omega_1=\sqrt{2-\sqrt2},\qquad\omega_2=\sqrt2,\qquad\omega_3=\sqrt{2+\sqrt2}}.
$$

## ↑ Ancestors (10)

1. [9D](../9d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
