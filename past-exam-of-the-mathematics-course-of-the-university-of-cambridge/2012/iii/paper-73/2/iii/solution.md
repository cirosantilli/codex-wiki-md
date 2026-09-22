<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\epsilon_{\rm loc}(\mathbf x)=2\nu S_{ij}S_{ij}$ and define a [coarse-grained energy dissipation](../../../../../../coarse-grained-energy-dissipation.md) at scale $r$, for example by a ball average,

$$
\epsilon_r(\mathbf x)=\frac{3}{4\pi r^3}\int_{|\mathbf y-\mathbf x|<r}\epsilon_{\rm loc}(\mathbf y)\,d^3y,
\qquad \langle\epsilon_r\rangle=\epsilon.
$$

This is the [random variable](../../../../../../random-variable-split.md) denoted $\epsilon_{\rm AV}(r)$. The [refined similarity](../../../../../../kolmogorov-refined-similarity-hypothesis.md) hypothesis uses the local supply of energy available to motions of size $r$, rather than replacing it everywhere by a global mean. In its [inertial range](../../../../../../inertial-range.md) form,

$$
\Delta v(r)=(r\epsilon_r)^{1/3}V,
\qquad
\langle(\Delta v)^p\mid\epsilon_r\rangle=C_p(r\epsilon_r)^{p/3}.
$$

At high local [Reynolds number](../../../../../../reynolds-number.md), $V$ has a universal conditional distribution independent of $\epsilon_r$, forcing details and $r$ within the [inertial range](../../../../../../inertial-range.md). This gives

$$
\boxed{S_p(r)=C_pr^{p/3}\langle\epsilon_r^{p/3}\rangle}.
$$

For signed odd orders the coefficients carry the appropriate sign; absolute [moments](../../../../../../moment.md) use their own coefficients. Universality is retained in the normalized conditional velocity statistics, while the distribution of $\epsilon_r$ can retain integral-scale information. This distinction resolves the particular averaging objection: its nonuniversal [viscous dissipation](../../../../../../viscous-dissipation.md) [moments](../../../../../../moment.md) are now explicitly present.

The quoted second [viscous dissipation](../../../../../../viscous-dissipation.md) [moment](../../../../../../moment.md) does not by itself determine every [longitudinal structure function](../../../../../../longitudinal-velocity-structure-function.md) exponent. The extra [lognormal intermittency model](../../../../../../lognormal-intermittency-model.md) assumes $Y_r=\log(\epsilon_r/\epsilon)$ is Gaussian. Write its [variance](../../../../../../variance-split.md) as $\sigma_r^2$. Normalization of the mean requires $\langle Y_r\rangle=-\sigma_r^2/2$, so

$$
\frac{\langle\epsilon_r^q\rangle}{\epsilon^q}
=\exp\left[\frac{q(q-1)}2\sigma_r^2\right].
$$

The second-[moment](../../../../../../moment.md) estimate gives $\exp(\sigma_r^2)=B(\ell/r)^\mu$. Hence, with $q=p/3$,

$$
S_p(r)=C_p\epsilon^{p/3}B^{p(p-3)/18}\ell^{\mu p(p-3)/18}
 r^{p/3-\mu p(p-3)/18},
\qquad
\boxed{\zeta_p=\frac p3-\frac\mu{18}p(p-3)}.
$$

In particular $\zeta_3=1$, $\zeta_2=2/3+\mu/9$ and $\zeta_6=2-\mu$.

The most problematic step is the extrapolation of a lognormal [viscous dissipation](../../../../../../viscous-dissipation.md) law to rare events and all [moment](../../../../../../moment.md) orders. It is not entailed by a measured second [moment](../../../../../../moment.md). Its quadratic exponents eventually decrease with $p$ and become negative for $p>3+6/\mu$. If the velocity has finite uniformly bounded [moments](../../../../../../moment.md), the bound $\langle|\Delta v|^p\rangle\le2^p\langle|u_x|^p\rangle$ prohibits such divergence as $r\to0$. Thus the model cannot be an unrestricted high-order [inertial range](../../../../../../inertial-range.md) law. This is a criticism of the lognormal closure, rather than an algebraic contradiction in [refined similarity](../../../../../../kolmogorov-refined-similarity-hypothesis.md) itself.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
