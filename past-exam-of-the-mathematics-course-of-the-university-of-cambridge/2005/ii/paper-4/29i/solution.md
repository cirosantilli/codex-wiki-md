<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

Use the minimization convention for [Pontryagin maximum principle](../../../../../pontryagin-maximum-principle.md): $H=c(x,t)+\lambda^Ta(x,u)$, with $\dot x=H_\lambda$, $\dot\lambda=-H_x$, and $u$ minimizing $H$ over its allowed set. The initial state is fixed; since terminal time is fixed and terminal state is free, the transversality condition is $\lambda(T)=\nabla K(x(T))$. No free-terminal-time condition $H(T)=0$ is imposed.

For the advertising problem, $\lambda_1(T)=\lambda_2(T)=0$ and $\dot\lambda_1=0$, so $\lambda_1=0$. Write $z=x_2>0$ and $\lambda=\lambda_2$. Then

$$
H=z+u(3-\lambda z),\qquad
\dot z=-uz,\qquad\dot\lambda=-1+u\lambda.
$$

The switching function $s=3-\lambda z$ satisfies $\dot s=z>0$, while $s(T)=3>0$. Thus there is at most one switch, from $u=1$ to $u=0$, and no singular interval. If $u$ were always zero, then $\lambda(t)=T-t$ and $s(0)=3-z(0)T<0$, contradicting [Hamiltonian](../../../../../hamiltonian.md) minimization. Hence a switch occurs at some $0<t_*<T$.

Before it, $z=z(0)e^{-t}$; after it, $\lambda=T-t$ and $z=z(0)e^{-t_*}$. Setting $s(t_*)=0$ gives

$$
\boxed{u(t)=
\begin{cases}1,&t<t_*,\\0,&t>t_*,\end{cases}
\qquad3e^{t_*}=z(0)(T-t_*)}.
$$

The left side increases and the right side decreases, so the switch is unique.

Sufficiency can also be proved directly. For any control with total effort $a=\int_0^Tu\,dt$, the cumulative effort by time $t$ is at most $\min(t,a)$. Since $z(t)=z(0)e^{-\int_0^tu}$, the best arrangement for that fixed effort is to advertise immediately at full strength for time $a$. Its cost is

$$
J(a)=z(0)(1-e^{-a})+z(0)(T-a)e^{-a}+3a.
$$

Its [derivative](../../../../../derivative.md) is $3-z(0)(T-a)e^{-a}$ and its second [derivative](../../../../../derivative.md) is $z(0)(T-a+1)e^{-a}>0$ on $[0,T]$. The unique minimizer is exactly the preceding $t_*$. This verifies a global optimum, not only a necessary extremal.

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
