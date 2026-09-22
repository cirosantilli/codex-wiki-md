<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

For this [chemical reaction network](../../../../../chemical-reaction-network.md), the [law of mass action](../../../../../law-of-mass-action.md) gives the reaction rates are $k_1s^2e$, $k_2c$ and $k_3c$. Their [stoichiometry](../../../../../stoichiometry.md) gives

$$
\dot s=-2k_1s^2e+2k_2c,\quad
\dot e=-k_1s^2e+(k_2+k_3)c,\quad
\dot c=k_1s^2e-(k_2+k_3)c,\quad
\dot p=2k_3c.
$$

Here the convention for $k_1$ absorbs any combinatorial factor for two identical reactants. Direct differentiation gives the two [conservation laws](../../../../../conservation-law.md)

$$
\boxed{e+c=e_0,\qquad s+2c+p=s_0.}
$$

Eliminating $e$ and $p$ leaves

$$
\dot s=-2k_1s^2(e_0-c)+2k_2c,\qquad
\dot c=k_1s^2(e_0-c)-(k_2+k_3)c.
$$

For positive $s_0,e_0,k_1$, use the [dimensionless variables](../../../../../dimensionless-variable.md) $u=s/s_0$, $v=c/e_0$ and $\tau=k_1e_0s_0t$. With prime marks denoting differentiation in $\tau$, this becomes

$$
\boxed{u'=-2u^2(1-v)+2(\mu-\lambda)v,\qquad\epsilon v'=u^2(1-v)-\mu v,}
$$

where

$$
\boxed{\epsilon=\frac{e_0}{s_0},\quad\mu=\frac{k_2+k_3}{k_1s_0^2},\quad\lambda=\frac{k_3}{k_1s_0^2},\quad u(0)=1,\quad v(0)=0.}
$$

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
