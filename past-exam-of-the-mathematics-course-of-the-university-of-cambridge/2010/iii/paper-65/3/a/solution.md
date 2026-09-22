<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the [Eulerian time average](../../../../../../eulerian-time-average.md) commute with space and time derivatives and let the statistically steady mean have no time derivative. Define $U=\overline u$, $V=\overline v$, $\hat u=u-U$ and $\hat v=v-V$, so $\overline{\hat u}=\overline{\hat v}=0$. Averaging instantaneous [incompressibility](../../../../../../incompressible-flow.md) gives

$$
\boxed{U_x+V_y=0,}
$$

and subtracting gives $\hat u_x+\hat v_y=0$ for the fluctuations. Start from the instantaneous streamwise [Navier-Stokes equation](../../../../../../navier-stokes-equation.md)

$$
u_t+u u_x+v u_y=-\frac1\rho p_x+\nu(u_{xx}+u_{yy}).
$$

Use [incompressibility](../../../../../../incompressible-flow.md) to write $u u_x+v u_y=\partial_x(u^2)+\partial_y(uv)$. The averaged products are $\overline{u^2}=U^2+\overline{\hat u^2}$ and $\overline{uv}=UV+\overline{\hat u\hat v}$. The mean conservative terms reduce back to $UU_x+VU_y$ because $U_x+V_y=0$. The [Reynolds-averaged momentum equation](../../../../../../reynolds-averaged-momentum-equation.md) is consequently

$$
\boxed{UU_x+VU_y=-\frac1\rho\bar p_x+\nu U_{yy}-\partial_y\overline{\hat u\hat v}-\partial_x\overline{\hat u^2}+\nu U_{xx}.}
$$

The signs use the positive covariance convention for the [Reynolds stress](../../../../../../reynolds-stress.md). In particular, both quadratic averages involve the fluctuations, not products of the mean $U$ with a fluctuation; the converted TeX loses the overbar/hat structure here.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
