<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two [tree-level Feynman diagrams](../../../../../../tree-level-feynman-diagram.md) have t-channel [W boson](../../../../../../w-boson.md) exchange. The antiquark process reverses the fermion-flow arrows on the lower line.

<a id="4/b/image-charged-current-neutrino-scattering-on-a-down-quark-and-an-up-antiquark-via-w-plus-exchange"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-305-neutrino-scattering.png)

**[Figure 2](#4/b/image-charged-current-neutrino-scattering-on-a-down-quark-and-an-up-antiquark-via-w-plus-exchange). Charged-current neutrino scattering on a down quark and an up antiquark via W-plus exchange**.

Each vertex contributes $g/(2\sqrt2)$ multiplying a chiral current. At momentum transfer $|q^2|\ll M_W^2$, the [gauge-boson propagator](../../../../../../gauge-boson-propagator.md) is approximated by its momentum-independent term $g_{\alpha\beta}/M_W^2$, up to the overall phase. The longitudinal term does not contribute to these conserved massless currents. Thus the coefficient is $g^2/(8M_W^2)=G_F/\sqrt2$, giving the [Fermi interaction](../../../../../../fermi-interaction.md). For the quark and antiquark amplitudes, apart from irrelevant overall phases,

$$
\mathcal M_d=\frac{G_F}{\sqrt2}[\bar u(p')\gamma^\alpha(1-\gamma^5)u(p)]
[\bar u(k')\gamma_\alpha(1-\gamma^5)u(k)],
$$

and

$$
\mathcal M_{\bar u}=\frac{G_F}{\sqrt2}[\bar u(p')\gamma^\alpha(1-\gamma^5)u(p)]
[\bar v(k)\gamma_\alpha(1-\gamma^5)v(k')].
$$

The low-energy operator form is $\mathcal L_{\rm eff}=-(G_F/\sqrt2)(\bar e\gamma^\alpha(1-\gamma^5)\nu_e)(\bar u\gamma_\alpha(1-\gamma^5)d)+\text{h.c.}$; its external spinor matrix elements are the displayed products.

For an unpolarized initial parton, average over its two spin states. There is no factor $1/2$ for the incoming active [neutrino](../../../../../../neutrino.md), which has one allowed [helicity](../../../../../../helicity.md). The initial color average cancels the final color sum, so there is no surviving color multiplicity in this parton cross section. Define

$$
T^{\alpha\beta}(a,b)=\operatorname{Tr}[\not a\gamma^\alpha(1-\gamma^5)\not b\gamma^\beta(1-\gamma^5)]
=8\left(a^\alpha b^\beta+a^\beta b^\alpha-g^{\alpha\beta}a\cdot b
+i\epsilon^{\alpha\beta\rho\sigma}a_\rho b_\sigma\right).
$$

The symmetric and antisymmetric parts have zero cross contraction. Their separate contractions are $128[(a\cdot c)(b\cdot d)+(a\cdot d)(b\cdot c)]$ and $128[(a\cdot c)(b\cdot d)-(a\cdot d)(b\cdot c)]$. Thus the given [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) identity yields

$$
T^{\alpha\beta}(a,b)T_{\alpha\beta}(c,d)=256(a\cdot c)(b\cdot d).
$$

Including the coefficient $G_F^2/2$ and the initial-parton [spin average](../../../../../../spin-average.md) gives

$$
\overline{|\mathcal M_d|^2}=64G_F^2(p\cdot k)(p'\cdot k'),\qquad
\overline{|\mathcal M_{\bar u}|^2}=64G_F^2(p\cdot k')(p'\cdot k).
$$

Massless kinematics and $q=p-p'=k'-k$ imply $p\cdot k=p'\cdot k'=s/2$. From $y_q=k\cdot q/(k\cdot p)$, $p'\cdot k=p\cdot k'=s(1-y_q)/2$. Therefore

$$
\overline{|\mathcal M_d|^2}=16G_F^2s^2,\qquad
\overline{|\mathcal M_{\bar u}|^2}=16G_F^2s^2(1-y_q)^2.
$$

To reduce the supplied phase-space formula, use the massless center-of-mass flux $2s$ and $d\Phi_2=d\Omega/(32\pi^2)$. This gives $d\sigma/d\Omega=\overline{|\mathcal M|^2}/(64\pi^2s)$. In that frame $y_q=(1-\cos\vartheta)/2$, so $d\Omega/dy_q=4\pi$. Hence

$$
\boxed{A(s)=\frac{s}{\pi},\qquad B(s,y_q)=\frac{s}{\pi}(1-y_q)^2,\qquad 0\leq y_q\leq1.}
$$

The antiquark channel's angular factor is a consequence of the chiral current and the reversed lower-line spinor order, rather than a color factor.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
