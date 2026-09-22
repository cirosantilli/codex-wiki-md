<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For [massless quark Compton scattering](../../../../../massless-quark-compton-scattering.md), the [color average](../../../../../color-average.md) contributes one, since $(1/N_c)\sum_{i,j}|\delta_{ji}|^2=1$. The [spin average](../../../../../spin-average.md) and incoming [photon](../../../../../photon.md) [polarization](../../../../../polarization-waves.md) average supply $1/(2\cdot2)=1/4$. The [Ward identities](../../../../../ward-identity.md) permit use of $-g_{\mu\nu}$ for each [photon polarization completeness relation](../../../../../photon-polarization-completeness-relation.md), and the massless [fermion spin sum](../../../../../fermion-spin-sum.md) is $\sum_ru_r(p)\bar u_r(p)=\not p$.

Let

$$
A_{\mu\nu}=\gamma_\nu\frac{\not q_s}s\gamma_\mu+\gamma_\mu\frac{\not q_u}u\gamma_\nu.
$$

Reversing the [gamma matrices](../../../../../gamma-matrices.md) order gives its Dirac-conjugate matrix $\bar A^{\mu\nu}$. The squared [scattering amplitude](../../../../../scattering-amplitude.md) is

$$
\langle|\mathcal M|^2\rangle=\frac{e^4Q_u^4}{4}\operatorname{tr}(\not p_3 A_{\mu\nu}\not p_1\bar A^{\mu\nu}).
$$

For clarity evaluate the four traces before dividing by their denominators. The [Mandelstam variables](../../../../../mandelstam-variables.md) obey $s+t+u=0$, with $t=(p_1-p_3)^2$, $p_1\cdot p_2=s/2$, $p_1\cdot p_4=u(-1/2)$ and $p_1\cdot p_3=-t/2$. For the squared $s$-channel contribution, the [gamma matrix trace identities](../../../../../gamma-matrix-trace-identities.md) imply

$$
\begin{aligned}
T_{ss}&=\operatorname{tr}(\not p_3\gamma_\nu\not q_s\gamma_\mu\not p_1\gamma^\mu\not q_s\gamma^\nu)\\
&=-2\operatorname{tr}(\not p_3\gamma_\nu\not q_s\not p_1\not q_s\gamma^\nu)\\
&=-2s\operatorname{tr}(\not p_3\gamma_\nu\not p_2\gamma^\nu)
=4s\operatorname{tr}(\not p_3\not p_2)=-8su.
\end{aligned}
$$

Here $\not q_s\not p_1\not q_s=2(q_s\cdot p_1)\not q_s-q_s^2\not p_1=s\not p_2$ and $p_3\cdot p_2=-u/2$. For the squared $u$-channel contribution, $\not q_u\not p_1\not q_u=-u\not p_4$ gives

$$
T_{uu}=\operatorname{tr}(\not p_3\gamma_\mu\not q_u\gamma_\nu\not p_1\gamma^\nu\not q_u\gamma^\mu)=-16u(p_3\cdot p_4)=-8su.
$$

One interference trace reduces to

$$
\begin{aligned}
T_{su}&=\operatorname{tr}(\not p_3\gamma_\nu\not q_s\gamma_\mu\not p_1\gamma^\nu\not q_u\gamma^\mu)\\
&=-2\operatorname{tr}(\not p_3\gamma_\nu\not q_s\not q_u\gamma^\nu\not p_1)
=-32(q_s\cdot q_u)(p_3\cdot p_1)=0,
\end{aligned}
$$

since $q_s\cdot q_u=(s+t+u)/2=0$. The other interference trace is its complex conjugate and also vanishes. Therefore

$$
\boxed{\langle|\mathcal M|^2\rangle=-2e^4Q_u^4\left(\frac us+\frac su\right)=-\frac{32e^4}{81}\frac{s^2+u^2}{su},\qquad C=\frac{32e^4}{81}.}
$$

Equivalently $C=512\pi^2\alpha_{\mathrm{em}}^2/81$ in terms of the [fine-structure constant](../../../../../fine-structure-constant.md). In the physical noncollinear region $s>0$, $u<0$, so the result is positive. The singular massless endpoint $u=0$ reflects a [collinear divergence](../../../../../collinear-divergence.md); it is not a negative squared [scattering amplitude](../../../../../scattering-amplitude.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2020](../../../../2020-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
