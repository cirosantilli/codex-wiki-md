<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $u,w\in X$, the forcing terms cancel, giving

$$
\begin{aligned}
\langle A(u)-A(w),u-w\rangle
={}&\int_\Omega\bigl(|\nabla u|^2\nabla u-|\nabla w|^2\nabla w\bigr)\cdot(\nabla u-\nabla w)\,dx\\
&+\int_\Omega(u^7-w^7)(u-w)\,dx.
\end{aligned}
$$

The scalar [function](../../../../../function-split.md) $s\mapsto s^7$ is strictly increasing on all of $\mathbb R$, so the second [integrand](../../../../../integrand.md) is nonnegative. For the first one, use the [quartic gradient monotonicity inequality](../../../../../quartic-gradient-monotonicity-inequality.md). Put $d=\xi-\eta$ and $m=(\xi+\eta)/2$ for real [vectors](../../../../../vector.md) $\xi,\eta$. Expanding gives

$$
\begin{aligned}
(|\xi|^2\xi-|\eta|^2\eta)\cdot(\xi-\eta)
&=|m|^2|d|^2+2(m\cdot d)^2+\frac14|d|^4\\
&\geq\frac14|\xi-\eta|^4.
\end{aligned}
$$

Consequently

$$
\boxed{\langle A(u)-A(w),u-w\rangle
\geq\frac14\|\nabla(u-w)\|_4^4
=\frac14\|u-w\|_X^4>0\quad(u\ne w).}
$$

The last strict inequality uses the [Poincaré inequality](../../../../../poincare-inequality.md): if the [weak gradient](../../../../../weak-gradient.md) of $u-w\in W_0^{1,4}(\Omega)$ vanishes, then $u=w$. This proves that $A$ is a [strictly monotone operator](../../../../../strictly-monotone-operator.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../split.md)
6. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
