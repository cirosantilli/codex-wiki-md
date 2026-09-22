<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Applying the [law of mass action](../../../../../law-of-mass-action.md) to the [sequential two-site enzyme reaction network](../../../../../sequential-two-site-enzyme-reaction-network.md) gives

$$
\begin{aligned}
\dot s&=-k_1se+k_{-1}c_1-k_3sc_1+k_{-3}c_2,\\
\dot e&=-k_1se+(k_{-1}+k_2)c_1,\\
\dot c_1&=k_1se-(k_{-1}+k_2)c_1-k_3sc_1+(k_{-3}+k_4)c_2,\\
\dot c_2&=k_3sc_1-(k_{-3}+k_4)c_2,\\
\dot p&=k_2c_1+k_4c_2.
\end{aligned}
$$

Adding the appropriate equations gives the [conservation laws](../../../../../conservation-law.md) $e+c_1+c_2=e_0$ and $s+c_1+2c_2+p=s_0$. In particular $e=e_0(1-v_1-v_2)$ after [nondimensionalization](../../../../../nondimensionalization.md).

Define the dimensionless reaction rates $a_1=k_{-1}/(k_1s_0)$, $a_3=k_{-3}/(k_1s_0)$, $b_2=k_2/(k_1s_0)$, $b_4=k_4/(k_1s_0)$ and $r_3=k_3/k_1$. Substitution, with primes denoting $d/d\tau$, yields

$$
\boxed{\begin{aligned}
u'&=-u(1-v_1-v_2)+a_1v_1-r_3uv_1+a_3v_2,\\
\epsilon v_1'&=u(1-v_1-v_2)-(a_1+b_2)v_1-r_3uv_1+(a_3+b_4)v_2,\\
\epsilon v_2'&=r_3uv_1-(a_3+b_4)v_2.
\end{aligned}}
$$

These right sides are $f,g_1,g_2$, respectively, with $u(0)=1$ and $v_1(0)=v_2(0)=0$. When $\epsilon\ll1$, the form of these [ordinary differential equations](../../../../../ordinary-differential-equation.md) displays the faster relaxation of the complexes, which motivates a subsequent [quasi-steady-state approximation](../../../../../quasi-steady-state-approximation.md).

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
