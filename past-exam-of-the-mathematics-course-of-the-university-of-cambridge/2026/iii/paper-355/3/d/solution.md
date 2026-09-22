<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the single-mode approximation write

$$
\widetilde E=Lra_1^2+Lua_1^4,
\qquad
r=\frac{F_c-F}{4},
\qquad
u=\frac F{64}.
$$

For the reference energy $U_0=Lg_1a_1^2$,

$$
Z_0=\sqrt{\frac{\pi k_BT}{Lg_1}},
\quad
F_0=\frac{k_BT}{2}\log\frac{Lg_1}{\pi k_BT},
$$



$$
\langle a_1^2\rangle_0=\frac{k_BT}{2Lg_1},
\qquad
\langle a_1^4\rangle_0=\frac{3(k_BT)^2}{4L^2g_1^2}.
$$

Up to an irrelevant constant from subtracting $\langle U_0\rangle_0$, the variational free energy is

$$
\boxed{\mathcal F(g_1)=
\frac{k_BT}{2}\log\frac{Lg_1}{\pi k_BT}
+\frac{rk_BT}{2g_1}
+\frac{3u(k_BT)^2}{4Lg_1^2}}.
$$

Minimization gives

$$
g_1^2-rg_1-\frac{3u k_BT}{L}=0,
$$

so the positive optimum is

$$
\boxed{g_1^*=\frac18\left[
F_c-F+\sqrt{(F_c-F)^2+\frac{3Fk_BT}{L}}
\right]}.
$$

The compression estimate through quartic order is

$$
\boxed{C(F)\simeq C_2-\frac34C_2^2},
\qquad
C_2=\frac{k_BT}{8Lg_1^*}.
$$

Using $f=F/F_c$ and $L_p=A/(k_BT)$,

$$
\boxed{C_2=
\frac{L/(\pi^2L_p)}
{1-f+\sqrt{(1-f)^2+3fL/(\pi^2L_p)}}}.
$$

This is finite and smooth at $f=1$, unlike the zero-temperature branch point. The width of the [thermal rounding of a buckling transition](../../../../../../thermal-rounding-of-a-buckling-transition.md) is controlled by the dimensionless flexibility $L/L_p$ and vanishes for an increasingly stiff or cold filament.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
