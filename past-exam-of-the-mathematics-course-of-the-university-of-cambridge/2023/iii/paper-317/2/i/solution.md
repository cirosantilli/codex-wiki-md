<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose first that the gas-pressure fraction $\beta=P_g/P$ is spatially constant, with $0<\beta<1$. This is a sufficient condition for a [stellar polytrope](../../../../../../stellar-polytrope.md). Since

$$
P_g=\frac{\rho k_BT^{1+s}}{\mu_1m_u},
\qquad
P_{\rm rad}=\frac{a_{\rm rad}T^4}{3},
$$

the ratio $P_{\rm rad}/P_g=(1-\beta)/\beta$ gives

$$
\rho=C_\beta T^{3-s},
\qquad
C_\beta=\frac{a_{\rm rad}\mu_1m_u}{3k_B}
\frac{\beta}{1-\beta}.
$$

Therefore

$$
P=\frac{a_{\rm rad}}{3(1-\beta)}T^4
=K\rho^{1+1/n},
$$

with

$$
\boxed{n=\frac{3-s}{1+s}},
\qquad
\boxed{
K(\beta)=\frac{a_{\rm rad}}{3(1-\beta)}
C_\beta^{-4/(3-s)}}.
$$

For an ordinary positive polytropic index one also assumes $0\leq s<3$.

The [radiative diffusion in a star](../../../../../../radiative-diffusion-in-a-star.md) equation can be written as

$$
\frac{dP_{\rm rad}}{dr}
=-\frac{\kappa\rho L_r}{4\pi cr^2}.
$$

Because $P_{\rm rad}=(1-\beta)P$ and $\beta$ is constant, [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) gives

$$
\frac{dP_{\rm rad}}{dr}
=-(1-\beta)\frac{Gm_r\rho}{r^2}.
$$

Equating them and using $\eta=(L_r/L)/(m_r/M)$ yields

$$
\boxed{\kappa\eta=4\pi cG(1-\beta)\frac{M}{L}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
