<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each $t$, let

$$
B_t[u,v]=\int_U\left(\sum_{i,j}a^{ij}(x,t)u_{x_i}v_{x_j}
+\sum_i b^i(x,t)u_{x_i}v+c(x,t)uv\right)dx.
$$

A [weak energy solution of a variable-coefficient wave equation](../../../../../../../weak-energy-solution-of-a-variable-coefficient-wave-equation.md) is a function $u\in H^1(U_T)$ with zero lateral trace, equivalently $u\in L^2(0,T;H_0^1(U))$, whose time trace satisfies $u(0)=\psi_0$ in $L^2(U)$ and for which

$$
\boxed{\int_0^T\bigl[-(u_t,v_t)_{L^2}+B_t[u,v]\bigr]dt
=\int_0^T(f,v)_{L^2}dt+(\psi_1,v(0))_{L^2}}
$$

for every $v\in H^1(U_T)$ with zero lateral trace and $v(T)=0$. Here $u\in H^1(0,T;L^2(U))$ has a continuous $L^2$ representative, so the displacement trace is well defined.

The velocity condition is encoded by the boundary term in time; an arbitrary space-time $H^1$ function need not have an $L^2$ trace of $u_t$. The equation implies $u_{tt}=f-L(t)u\in L^2(0,T;H^{-1}(U))$, hence $u_t$ has a continuous $H^{-1}$ representative and $u_t(0)=\psi_1$ in that sense. This is the [weak formulation](../../../../../../../weak-formulation.md) obtained by [integration by parts](../../../../../../../integration-by-parts.md) once in time and once in space.

## ↑ Ancestors (12)

1. [I](../i.md)
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
