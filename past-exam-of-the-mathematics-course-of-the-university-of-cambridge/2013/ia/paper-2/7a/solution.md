<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

Retain the [derivative](../../../../../derivative.md) marks and coefficients from the printed system. In matrix form it is $M\dot u+Ku=b(t)$, with

$$
M=\begin{pmatrix}3&1\\1&4\end{pmatrix},\qquad
K=\begin{pmatrix}5&-1\\-2&7\end{pmatrix}.
$$

Since $\det M=11$, multiplication by its inverse gives

$$
\dot x+2x-y=e^{-t}+e^{-3t},\qquad
\dot y-x+2y=-e^{-t}+e^{-3t}.
$$

The [linear transformation](../../../../../linear-map.md) $u=x+y$, $v=x-y$ diagonalizes this system:

$$
\dot u+u=2e^{-3t},\qquad \dot v+3v=2e^{-t}.
$$

Both start at zero. An [integrating factor](../../../../../integrating-factor.md) gives $u=v=e^{-t}-e^{-3t}$, so

$$
\boxed{x(t)=e^{-t}-e^{-3t},\qquad y(t)=0}.
$$

Direct substitution into the two original equations confirms the different forcing coefficients; the exact cancellation in $y$ depends on those coefficients.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
