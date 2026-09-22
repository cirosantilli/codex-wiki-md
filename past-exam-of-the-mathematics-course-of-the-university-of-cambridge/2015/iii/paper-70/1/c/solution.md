<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Splitting the [free Schrodinger equation](../../../../../../free-schrodinger-equation.md) into real and imaginary parts gives

$$
\boxed{u_t=-v_{xx},\qquad v_t=u_{xx}.}
$$

Differentiating the first relation in time and using the second yields the [Euler-Bernoulli beam equation](../../../../../../euler-bernoulli-beam-equation.md) $u_{tt}+u_{xxxx}=0$. This is the [Schrodinger factorization of the elastic beam equation](../../../../../../schrodinger-factorization-of-the-elastic-beam-equation.md).

Assume the initial velocity has an integrable first spatial moment, as allowed by sufficient decay, and define

$$
v_0(x)=-\int_x^\infty(s-x)u_1(s)ds,\qquad q_0(x)=u_0(x)+iv_0(x).
$$

Then $v_0''=-u_1$ and $v_0$ decays at infinity. To encode the second boundary datum, define

$$
v_b(t)=v_0(0)+\int_0^t\widetilde u_1(s)ds,\qquad g_0(t)=\widetilde u_0(t)+iv_b(t).
$$

The [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) for the resulting [free Schrodinger equation](../../../../../../free-schrodinger-equation.md) is compatible at the corner, since $q_0(0)=g_0(0)$. Insert these explicit $q_0,g_0$ into the data-only complex integral in part (b), with $\widehat q_0$ and $G_0$ defined as in part (a). **The required displacement is the real part of that integral.** Equivalently, the uniformly convergent lifted integral in part (b) may be used with the same complex data.

The [Schrodinger factorization of the elastic beam equation](../../../../../../schrodinger-factorization-of-the-elastic-beam-equation.md) verifies every condition: $u(x,0)=u_0(x)$, $u_t(x,0)=-v_0''(x)=u_1(x)$, $u(0,t)=\widetilde u_0(t)$, and

$$
u_{xx}(0,t)=v_t(0,t)=v_b'(t)=\widetilde u_1(t).
$$

The corner requirements on $u_0''$ and $\widetilde u_0'$ ensure consistency of these derivative traces; the natural interpretation of the last printed compatibility is $\widetilde u_0'(0)=u_1(0)$. If its prime were instead imposed for every $t$, that would simply be an extra restriction on the data, and the same construction would still solve them.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
