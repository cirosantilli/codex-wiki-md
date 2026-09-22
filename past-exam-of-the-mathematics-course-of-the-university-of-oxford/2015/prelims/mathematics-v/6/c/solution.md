<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the positive weights

$$
\boxed{a=\rho_1c_1,\qquad b=\rho_2c_2.}
$$

These are the [volumetric heat capacities](../../../../../../volumetric-heat-capacity.md). The [heat equations](../../../../../../heat-equation.md) and [integration by parts](../../../../../../integration-by-parts.md) give

$$
\begin{aligned}
I'(t)
&=2k_1\int_{-L}^0T_1T_{1xx}\,dx+2k_2\int_0^LT_2T_{2xx}\,dx\\
&=2k_1[T_1T_{1x}]_{-L}^{0}+2k_2[T_2T_{2x}]_0^L
-2k_1\int_{-L}^0T_{1x}^2\,dx-2k_2\int_0^LT_{2x}^2\,dx.
\end{aligned}
$$

The exterior [boundary terms](../../../../../../boundary-term.md) vanish because the [temperatures](../../../../../../temperature-split.md) there are zero. At the [thermal interface](../../../../../../thermal-interface.md), the remaining term is

$$
2T(0,t)\,[k_1T_{1x}(0_-,t)-k_2T_{2x}(0_+,t)]=0
$$

by continuity of [temperature](../../../../../../temperature-split.md) and [heat flux](../../../../../../heat-flux-density.md). Hence the weighted [energy estimate](../../../../../../energy-estimate.md) is

$$
\boxed{I'(t)=-2k_1\int_{-L}^0T_{1x}^2\,dx-2k_2\int_0^LT_{2x}^2\,dx\leq0.}
$$

Both weights are positive, so $I\geq0$. Zero initial [temperatures](../../../../../../temperature-split.md) give $I(0)=0$, forcing $I(t)=0$ for all $t>0$. Each [temperature](../../../../../../temperature-split.md) therefore vanishes throughout its slab. Applying this argument to a difference also proves [uniqueness](../../../../../../uniqueness.md) for arbitrary common [initial data](../../../../../../initial-data-in-general-relativity.md) in this [thermal interface problem](../../../../../../thermal-interface-problem.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
