<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Neglect condensation and the smaller droplets' fall speed, while retaining their specified liquid-water content. For [exponential cloud collector growth](../../../../exponential-cloud-collector-growth.md), the collection law and spherical collector [mass](../../../../mass.md) give

$$
4\pi\rho_lR^2\dot R=\pi R^2(k_RR)LE,\quad
\dot R=\alpha_RR,\qquad\alpha_R=\frac{k_RLE}{4\rho_l}=1.6\times10^{-3}\,\mathrm{s^{-1}}.
$$

Thus $R(t)=R_0e^{\alpha_Rt}$. The growing terminal speed eventually exceeds the updraft, and

$$
\boxed{h_R(t)=Ut-\frac{k_RR_0}{\alpha_R}(e^{\alpha_Rt}-1)
=t\,\mathrm{m\,s^{-1}}-100\,\mathrm m\,(e^{0.0016t}-1),}
$$

where the last expression uses $t$ in seconds and $U=1\,\mathrm{m\,s^{-1}}$. Numerically,

$$
\boxed{h_R(1000\,\mathrm s)=605\,\mathrm m,\qquad h_R(2000\,\mathrm s)=-353\,\mathrm m\quad\text{(formal extrapolation)}.}
$$

The trajectory reaches maximum height when $k_RR=U$, at $t=1145\,\mathrm s$, $R=125\,\mu\mathrm m$ and $h_{\max}=620\,\mathrm m$. It returns to cloud base near $t=1860\,\mathrm s$, with radius about $392\,\mu\mathrm m$. The left-to-right sketch in the preceding figure shows this rise and subsequent fall.

Once the drop leaves the cloud, the prescribed in-cloud $L$, $U$ and collection law need not persist. Consequently the negative $2000$-second value describes the requested constant-coefficient model's extension, not a prediction that collection continues below cloud base. Its actual subsequent height needs an outside-cloud model. Within the cloud, the exponential feedback between increasing radius and increasing swept volume explains how a minority of collector drops can escape the condensation bottleneck and initiate warm rain; depletion, breakup and changes in fall law eventually limit indefinite exponential growth.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
