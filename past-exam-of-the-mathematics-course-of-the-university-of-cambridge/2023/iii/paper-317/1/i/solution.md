<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The four [stellar structure equations](../../../../../../stellar-structure-equations.md) are

$$
\frac{dm_r}{dr}=4\pi r^2\rho,
\qquad
\frac{dP}{dr}=-\frac{Gm_r\rho}{r^2},
$$



$$
\frac{dL_r}{dr}=4\pi r^2\rho\epsilon,
\qquad
\frac{dT}{dr}=-\frac{3\kappa\rho L_r}{16\pi a_{
m rad}c,r^2T^3},
$$

together with the perfect-gas [equation of state](../../../../../../equation-of-state.md)

$$
P=\frac{\rho k_BT}{\mu m_u}.
$$

Here $a_{\rm rad}$ is the [radiation constant](../../../../../../radiation-constant.md), $\epsilon$ is the specific [stellar energy-generation rate](../../../../../../stellar-energy-generation-rate.md), and $\kappa$ is the [opacity](../../../../../../opacity.md).

Put $x=r/R$. Integrating the prescribed density gives the [enclosed mass](../../../../../../enclosed-mass.md)

$$
m_r=4\pi\rho_c\left(\frac{r^3}{3}-\frac{r^4}{4R}\right).
$$

Since $m_R=M$,

$$
\boxed{\rho_c=\frac{3M}{\pi R^3}},
\qquad
\boxed{m_r=Mx^3(4-3x)}.
$$

Integrating [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) inward from $P(R)=0$ gives

$$
\boxed{
P(r)=\frac{GM\rho_c}{R}
\left(\frac5{12}-2x^2+\frac73x^3-\frac34x^4\right)}.
$$

The ideal-gas law then gives

$$
\boxed{
T(r)=\frac{\mu m_uGM}{k_BR}
\frac{(1-x)(5+10x-9x^2)}{12}}.
$$

In particular,

$$
\boxed{P_c=\frac{5GM^2}{4\pi R^4}},
\qquad
\boxed{T_c=\frac{5\mu m_uGM}{12k_BR}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
