<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [higher-order Euler-Lagrange equation](../../../../../../higher-order-euler-lagrange-equation.md) for a functional depending on $h_x$ and $h_{xx}$ gives

$$
k_ch_{xxxx}-\sigma h_{xx}=0.
$$

With the [membrane elastic length](../../../../../../membrane-elastic-length.md)

$$
\xi=\sqrt{\frac{k_c}{\sigma}},
$$

the general free-membrane profile is

$$
h(x)=A+Bx+Ce^{x/\xi}+De^{-x/\xi}.
$$

Two integrations by parts, followed by use of the field equation, turn the energy of any free interval $[a,b]$ into the [boundary term](../../../../../../boundary-term.md)

$$
E_m[a,b]=\frac12
\left[k_c(h_{xx}h_x-h_{xxx}h)+\sigma hh_x\right]_a^b.
$$

Take the undeformed membrane to have $h,h_x\to0$ at infinity. In the small-contact approximation, the cylindrical profile is

$$
h_c(x)=h_c(0)-\frac{x^2}{2R},
\qquad h_c'(\delta_o)=-\frac{\delta_o}{R}.
$$

Continuity of height and slope at the right contact point and exponential decay then give

$$
h(x)=\frac{\xi\delta_o}{R}e^{-(x-\delta_o)/\xi},
\qquad x\geq\delta_o,
$$

with its reflected copy on the left. The two free tails carry

$$
E_{\rm out}=2\cdot\frac12\int_{\delta_o}^{\infty}
\left(k_ch_{xx}^2+\sigma h_x^2\right)dx
=\frac{k_c\delta_o^2}{\xi R^2}.
$$

Within the contact, $h_{xx}=-1/R$. Since $\delta_o\ll\xi$, the tension contribution there is smaller than the bending contribution by $O(\delta_o^2/\xi^2)$, so

$$
E_{\rm contact}=\frac{k_c\delta_o}{R^2},
\qquad
E_a=-2\mathcal U\delta_o.
$$

Writing the [dimensionless adhesion strength](../../../../../../dimensionless-adhesion-strength.md) as $U=R^2\mathcal U/k_c$, the total energy is

$$
E(\delta_o)=\frac{k_c}{R^2}
\left[\frac{\delta_o^2}{\xi}+(1-2U)\delta_o\right].
$$

Its stationary point is

$$
\boxed{\delta_o=\xi\left(U-\frac12\right)}.
$$

It is an admissible bound state only for $U>1/2$; otherwise the constrained minimum is the unbound state $\delta_o=0$. Substitution gives

$$
\boxed{E_{\min}=-\frac{k_c\xi}{R^2}
\left(U-\frac12\right)^2}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
