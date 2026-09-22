<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use a flat five-dimensional metric of signature $(+----)$ and a circle coordinate $y\sim y+2\pi r$. Start with the canonically normalized [Maxwell action](../../../../../maxwell-action.md)

$$
S_5=-\frac14\int d^4x\int_0^{2\pi r}dy\,F_{MN}F^{MN},
\qquad F_{MN}=\partial_M A_N-\partial_N A_M.
$$

Expand the real [Maxwell field](../../../../../electromagnetic-field.md) in a [Fourier series](../../../../../fourier-series-split.md):

$$
A_M(x,y)=\frac1{\sqrt{2\pi r}}\sum_{n\in\mathbb Z}A_M^{(n)}(x)e^{iny/r},
\qquad A_M^{(-n)}=(A_M^{(n)})^*.
$$

The circle integral makes different modes orthogonal. Writing $a^{(n)}=A_5^{(n)}$ and $k_n=n/r$, the resulting four-dimensional [action](../../../../../action.md) is

$$
S_4=\int d^4x\sum_n\left[-\frac14F_{\mu\nu}^{(n)}F^{\mu\nu(-n)}
+\frac12(\partial_\mu a^{(n)}-ik_nA_\mu^{(n)})
(\partial^\mu a^{(-n)}+ik_nA^{\mu(-n)})\right].
$$

The scalar sign is positive because the fifth direction is spacelike in the chosen mostly-minus metric. This expression follows directly by separating the $\mu\nu$ and the two identical $\mu5$ contributions in $F_{MN}F^{MN}$.

A five-dimensional [gauge transformation](../../../../../gauge-transformation.md) $A_M\mapsto A_M+\partial_M\Lambda$ acts on its modes by

$$
\delta A_\mu^{(n)}=\partial_\mu\Lambda^{(n)},\qquad
\delta a^{(n)}=ik_n\Lambda^{(n)}.
$$

For $n\ne0$, define the gauge-invariant vector

$$
B_\mu^{(n)}=A_\mu^{(n)}-\frac1{ik_n}\partial_\mu a^{(n)}.
$$

Then $F_{\mu5}^{(n)}=-ik_nB_\mu^{(n)}$, so its term is a [Proca field](../../../../../proca-field.md) mass term $+\tfrac12k_n^2B_\mu^{(n)}B^{\mu(-n)}$. Equivalently, a periodic mode-dependent [gauge transformation](../../../../../gauge-transformation.md) sets $a^{(n)}=0$. The nonzero modes are massive vectors whose longitudinal polarization is supplied by $a^{(n)}$ through the [Stueckelberg mechanism](../../../../../stueckelberg-mechanism.md):

$$
\boxed{m_n=\frac{|n|}{r}\quad(n\ne0).}
$$

For each positive $n$ there is one complex vector, equivalently the two real sine/cosine vectors, each with three physical polarizations. The negative mode is its conjugate, not another independent complex field. This is the infinite [Kaluza-Klein tower](../../../../../kaluza-klein-tower.md) of the [Maxwell reduction on a circle](../../../../../maxwell-reduction-on-a-circle.md).

At $n=0$, $\delta a^{(0)}=0$ under periodic infinitesimal gauge transformations. The zero modes are a massless vector with two polarizations and a real massless scalar with one. The scalar is the circle component, or [Wilson line](../../../../../wilson-line.md) degree of freedom; a generic constant value cannot be removed by a periodic gauge parameter. Both have $m_0=0$. At energies $E\ll1/r$, the free theory's [low-energy effective action](../../../../../low-energy-effective-action.md) is therefore

$$
\boxed{S_{\mathrm{low}}=\int d^4x\left[-\frac14F_{\mu\nu}^{(0)}F^{\mu\nu(0)}
+\frac12\partial_\mu a^{(0)}\partial^\mu a^{(0)}\right].}
$$

There is no scalar potential in this free Maxwell theory. If the original action instead has coefficient $1/g_5^2$ and unrescaled constant zero-mode fields are used, integrating the circle gives $g_4^2=g_5^2/(2\pi r)$; canonical field rescaling recovers the normalization displayed above.

For the gravitational part, allow a circle radius field $R(x)$ with vacuum value $r$, and use a dimensionless angle $\chi\sim\chi+2\pi$ in the [Kaluza-Klein theory](../../../../../kaluza-klein-theory.md) ansatz

$$
ds_5^2=g_{\mu\nu}(x)dx^\mu dx^\nu
-R(x)^2\bigl[d\chi+\kappa A_\mu(x)dx^\mu\bigr]^2.
$$

The vector comes from off-diagonal metric components; $R$ is the [radion](../../../../../radion.md). Perform the coordinate transformation $\chi'=\chi-\kappa\lambda(x)$, leaving $x$ unchanged. Since $d\chi=d\chi'+\kappa\partial_\mu\lambda\,dx^\mu$, the metric has the same form with

$$
\boxed{A_\mu'=A_\mu+\partial_\mu\lambda,\qquad R'=R,\qquad g_{\mu\nu}'=g_{\mu\nu}.}
$$

Thus a higher-dimensional [diffeomorphism](../../../../../diffeomorphism.md) becomes an Abelian [gauge transformation](../../../../../gauge-transformation.md) in the reduced theory. Changing the sign convention for the internal coordinate shift reverses the displayed sign without changing its content.

More generally, continuous internal isometries give lower-dimensional [gauge symmetries](../../../../../gauge-invariance.md), with vector fields from metric components along the corresponding [Killing vector fields](../../../../../killing-vector-field.md). The circle translation group gives $U(1)$. A scalar mode $\psi_n(x)e^{in\chi}$ transforms as $\psi_n'=e^{in\kappa\lambda}\psi_n$, so $D_\mu\psi_n=(\partial_\mu-in\kappa A_\mu)\psi_n$ transforms covariantly. This derives [Kaluza-Klein charge quantization](../../../../../kaluza-klein-charge-quantization.md) in the chosen vector normalization. The metric vector is a graviphoton; if a five-dimensional Maxwell field is present as well, its zero-mode photon is a separate field originating from that Maxwell gauge symmetry.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
