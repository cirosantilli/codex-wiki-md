<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the recovered [uranium](../../../../../uranium.md) inventory, rather than the initial fuel mass, as the recycle feed. Its available mass is

$$
F_r=33(1-0.015)=32.505 \mathrm{t\,U\,yr^{-1}}.
$$

Assuming the same [enrichment tails](../../../../../enrichment-tails.md) assay and the specified higher recycled-fuel assay, the [isotopic mass balance](../../../../../isotopic-mass-balance.md) gives

$$
P_r=F_r\frac{0.0085-0.003}{0.043-0.003}=4.4694375 \mathrm{t\,U\,yr^{-1}},\qquad W_r=28.0355625 \mathrm{t\,U\,yr^{-1}}.
$$

Treat this fuel as replacing the same heavy-metal mass of ordinary fresh fuel: the stipulated higher [uranium-235](../../../../../uranium-235.md) content compensates for [uranium-236](../../../../../uranium-236.md). The displaced natural feed is

$$
\Delta F=9.25P_r=\boxed{41.3423 \mathrm{t\,U\,yr^{-1}}},
$$

about **12.63% of the once-through natural-uranium requirement**. The residual natural feed demand is $286.052 \mathrm{t\,U\,yr^{-1}}$.

For separative work accounting define

$$
V(x)=(1-2x)\ln\frac{1-x}{x},\qquad S=PV(x_p)+WV(x_w)-FV(x_f).
$$

Using kilograms in this expression gives kg-SWU. For ordinary fresh fuel the work per product kilogram is

$$
s_f=V(0.040)+8.25V(0.003)-9.25V(0.007)=5.34661 \mathrm{kg\!\text{-}\!SWU\,kg^{-1}}.
$$

The fresh work avoided by substituting $P_r$ is $23896.3 \mathrm{kg\!\text{-}\!SWU\,yr^{-1}}$, but producing that recycled product still requires

$$
S_r=1000\big[P_rV(0.043)+W_rV(0.003)-F_rV(0.0085)\big]
=22409.6 \mathrm{kg\!\text{-}\!SWU\,yr^{-1}}.
$$

Hence the **net** saving is

$$
\Delta S=1000P_rs_f-S_r=\boxed{1486.73 \mathrm{kg\!\text{-}\!SWU\,yr^{-1}}}.
$$

The work saving is only about **0.786%** of the original annual separative work. Crediting the whole avoided fresh-fuel work without charging the recycle work would substantially overstate the saving. This is an annual resource account at the supplied assays, with no isotope-separation equipment model.

## ↑ Ancestors (10)

1. [C](../c.md)
2. [1](../../1.md)
3. [Module NE4](../../../paper-ne4-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
