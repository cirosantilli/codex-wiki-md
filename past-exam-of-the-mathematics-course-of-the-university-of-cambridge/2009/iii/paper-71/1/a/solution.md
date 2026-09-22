<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [linear dispersive Stokes equation](../../../../../../linear-dispersive-stokes-equation.md) with time variable $t$. Put $E_k=e^{-ikx+\omega(k)t}$. Expanding the required [local relation](../../../../../../local-relation.md) gives

$$
(E_kq)_t+(E_kX)_x=E_k\bigl(q_t+\omega q+X_x-ikX\bigr).
$$

Choose $X=q_{xx}+ikq_x+(1-k^2)q$. Direct differentiation then yields

$$
X_x-ikX=q_{xxx}+q_x-ik(1-k^2)q.
$$

The unwanted coefficient of $q$ cancels precisely when $\omega(k)=ik(1-k^2)$. Hence

$$
\boxed{\omega(k)=i(k-k^3),\qquad X=q_{xx}+ikq_x+(1-k^2)q.}
$$

With these choices, the [local relation](../../../../../../local-relation.md) is exactly $E_k(q_t+q_x+q_{xxx})=0$ for every complex [spectral parameter for a linear boundary value problem](../../../../../../spectral-parameter-for-a-linear-boundary-value-problem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
