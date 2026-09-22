<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take the difference of two [weak solutions](../../../../../../../weak-solution.md), so $f=\psi_0=\psi_1=0$. At the stated $H^1(U_T)$ regularity, it is not justified simply to test by $u_t$, which need not belong to the spatial test space $H_0^1$. Instead use the antiderivative test underlying [uniqueness of Sobolev weak solutions of a wave equation](../../../../../../../uniqueness-of-sobolev-weak-solutions-of-a-wave-equation.md).

Fix $s\in(0,T]$ and define

$$
v(t)=\begin{cases}\displaystyle\int_t^su(r)dr,&0\leq t<s,\\0,&s\leq t\leq T,
\end{cases}
\qquad z(t)=\int_0^tu(r)dr.
$$

These are [Bochner integrals](../../../../../../../bochner-integral.md) in $H_0^1$. The function $v$ is an admissible space-time $H^1$ test, $v_t=-u$ before $s$, and $v(t)=z(s)-z(t)$. The time term in the [weak formulation](../../../../../../../weak-formulation.md) is

$$
-\int_0^s(u_t,v_t)dt=\frac12\|u(s)\|_2^2,
$$

because $u(0)=0$. Symmetry of $a^{ij}$ and [integration by parts](../../../../../../../integration-by-parts.md) in time give

$$
\int_0^s\int_Ua^{ij}u_{x_i}v_{x_j}
=\frac12\int_Ua^{ij}(x,0)z_{x_i}(s)z_{x_j}(s)
+\frac12\int_0^s\int_Ua_t^{ij}v_{x_i}v_{x_j}.
$$

For the lower-order part, [integration by parts](../../../../../../../integration-by-parts.md) in space gives

$$
\int_U(b^i u_{x_i}v+cuv)
=\int_Uu\bigl((c-\operatorname{div}b)v-b\cdot Dv\bigr).
$$

Bounded coefficients, the [Poincaré inequality](../../../../../../../poincare-inequality.md) for $v$, and the [Young inequality](../../../../../../../young-s-inequality-for-products.md) now imply

$$
\|u(s)\|_2^2+\theta\|Dz(s)\|_2^2
\leq C\int_0^s\bigl(\|u(t)\|_2^2+\|Dv(t)\|_2^2\bigr)dt.
$$

Since $Dv(t)=Dz(s)-Dz(t)$,

$$
\|u(s)\|_2^2+\theta\|Dz(s)\|_2^2
\leq C\int_0^s\bigl(\|u(t)\|_2^2+\|Dz(t)\|_2^2\bigr)dt
+Cs\|Dz(s)\|_2^2.
$$

For $s$ in a sufficiently short fixed interval, absorb the last term into the left-hand side. The [Gronwall inequality](../../../../../../../gronwall-inequality.md) applied to $\|u(s)\|_2^2+(\theta/2)\|Dz(s)\|_2^2$ proves $u=0$ on that interval. The equation gives continuity of $u_t$ in $H^{-1}$, so both initial traces at its endpoint are again zero. Repeating with the same uniform coefficient bounds covers $[0,T]$. Therefore

$$
\boxed{\text{the weak solution is unique whenever it exists.}}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
