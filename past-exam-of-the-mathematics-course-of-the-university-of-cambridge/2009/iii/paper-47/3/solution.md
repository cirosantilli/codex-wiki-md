<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $t=\log\mu$ and use $\alpha_i=g_i^2/(4\pi)$. The [renormalization-group beta function](../../../../../beta-function-physics.md) implies

$$
\frac{d\alpha_i}{dt}=\frac{\beta_i}{2\pi}\alpha_i^2,
\qquad
\frac{d\alpha_i^{-1}}{dt}=-\frac{\beta_i}{2\pi}.
$$

Integrating the one-loop [running coupling](../../../../../running-coupling.md) equation gives

$$
\boxed{\alpha_i^{-1}(\mu)=\alpha_i^{-1}(M_Z)
-\frac{\beta_i}{2\pi}\log\frac\mu{M_Z}.}
$$

Here the sign of $\beta_i$ is the sign convention in the question: a negative coefficient makes the inverse coupling increase towards high energy.

For [gauge coupling unification](../../../../../gauge-coupling-unification.md), let $L=\log(M_{\mathrm{GUT}}/M_Z)/(2\pi)$ and let $a_G$ be the common inverse coupling at the unification scale. The normalized [hypercharge](../../../../../hypercharge.md) coupling is $(5/3)\alpha_1$, so

$$
\frac35\alpha_1^{-1}(M_Z)=a_G+\frac35\beta_1L,
\qquad
\alpha_2^{-1}(M_Z)=a_G+\beta_2L,
\qquad
\alpha_3^{-1}(M_Z)=a_G+\beta_3L.
$$

Subtract the second relation from the first to determine $L$, then subtract it from the third. Provided $3\beta_1/5-\beta_2\ne0$, this proves

$$
\boxed{\alpha_3^{-1}(M_Z)=\alpha_2^{-1}(M_Z)
+\frac{\beta_3-\beta_2}{3\beta_1/5-\beta_2}
\left[\frac35\alpha_1^{-1}(M_Z)-\alpha_2^{-1}(M_Z)\right].}
$$

The factors $3/5$ belong to the inverse normalized coupling; dropping them changes the prediction.

Use the [Standard Model](../../../../../standard-model-split.md) gauge group $SU(3)_C\times SU(2)_L\times U(1)_Y$ and convention $Q=T_3+Y$. One fermion family and one complex [Higgs doublet](../../../../../higgs-field.md) have the following [Standard Model representations](../../../../../standard-model-representation.md). The left-handed quark and lepton doublets contain two [Weyl spinors](../../../../../weyl-spinor.md) each; the right-handed fields are single Weyl species.

$$
\begin{array}{c|ccc|c|c}
\text{field}&SU(3)_C&SU(2)_L&Y&\text{spin}&\text{chirality}\\\hline
Q_L=(u_L,d_L)&\mathbf3&\mathbf2&1/6&1/2&L\\
u_R&\mathbf3&\mathbf1&2/3&1/2&R\\
d_R&\mathbf3&\mathbf1&-1/3&1/2&R\\
L_L=(\nu_L,e_L)&\mathbf1&\mathbf2&-1/2&1/2&L\\
e_R&\mathbf1&\mathbf1&-1&1/2&R\\
\phi&\mathbf1&\mathbf2&1/2&0&\text{not applicable}
\end{array}
$$

The row $u_R$ denotes the right-handed [up quark](../../../../../up-quark.md). Equivalently an all-left-handed table replaces the three right-handed fields by $u_R^c:(\overline{\mathbf3},\mathbf1)_{-2/3}$, $d_R^c:(\overline{\mathbf3},\mathbf1)_{1/3}$, and $e_R^c:(\mathbf1,\mathbf1)_1$; these are alternative descriptions, not extra fermions. The minimal model has no [right-handed neutrino](../../../../../right-handed-neutrino.md). For completeness, the family-independent gauge fields are the spin-one [gluons](../../../../../gluon.md) $(\mathbf8,\mathbf1)_0$, weak gauge bosons $(\mathbf1,\mathbf3)_0$, and hypercharge gauge boson $(\mathbf1,\mathbf1)_0$; they are not counted once per family.

For the [Standard Model one-loop gauge coefficients](../../../../../standard-model-one-loop-gauge-coefficients.md), include three fermion families and one Higgs doublet. With $T(\mathbf N)=1/2$, the colour [Dynkin index](../../../../../dynkin-index.md) sum in one family is

$$
\sum_{f,\,\text{one family}}T_3(f)=2\cdot\frac12+\frac12+\frac12=2.
$$

The first factor two counts the two members of $Q_L$; the colour trace is already included in the [Dynkin index](../../../../../dynkin-index.md). There is no coloured scalar. Hence

$$
\boxed{\beta_3=-11+\frac23(3\cdot2)=-7.}
$$

For $SU(2)_L$, the three colours of $Q_L$ and the lepton doublet give $3(1/2)+1/2=2$ per family. The Higgs contributes $T_2(\phi)=1/2$. Thus

$$
\boxed{\beta_2=-\frac{22}3+\frac23(3\cdot2)+\frac13\frac12=-\frac{19}6.}
$$

For $U(1)_Y$, sum squared [hypercharges](../../../../../hypercharge.md) over every colour and doublet component. One family contributes

$$
6\left(\frac16\right)^2+3\left(\frac23\right)^2
+3\left(-\frac13\right)^2+2\left(-\frac12\right)^2+(-1)^2
=\frac{10}3.
$$

The two complex Higgs components contribute $2(1/2)^2=1/2$. There is no Abelian gauge self-interaction term, so

$$
\boxed{\beta_1=\frac23\left(3\cdot\frac{10}3\right)+\frac13\frac12=\frac{41}6.}
$$

This $\beta_1$ is for the unnormalized coupling $g_Y$ used in the question. For $g_1^{\mathrm{GUT}}=\sqrt{5/3}\,g_Y$, the corresponding coefficient is $(3/5)\beta_1=41/10$. This distinction is required for a consistent unification calculation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
