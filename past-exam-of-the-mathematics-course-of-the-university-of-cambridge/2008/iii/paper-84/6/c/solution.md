<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The balanced finite source has $Q(z)=CF_s^{1/3}(z+z_v)^{5/3}$ and $Q(0)=Q_s$. An ideal small opening exhausts the physical source volume $\pi Q_s$. When $z_f>h$, the opening is in the unprocessed lower region. Its outflow and the plume's entrainment both remove lower fluid, while all plume flux across the front enters the processed region. When $z_f<h$, the opening exhausts processed fluid, reducing the net growth of that region by $\pi Q_s$. Thus the [finite-source filling-box front with a side opening](../../../../../../finite-source-filling-box-front-with-a-side-opening.md) obeys

$$
\boxed{\dot z_f=
\begin{cases}
-a_p(z_f+z_v)^{5/3},&z_f>h,\\
-a_p[(z_f+z_v)^{5/3}-z_v^{5/3}],&0<z_f<h.
\end{cases}}
$$

The ideal exhaust switches fluid type as the front crosses its height. Above the opening the solution is $z_f=[(H+z_v)^{-2/3}+2a_pt/3]^{-3/2}-z_v$, and it reaches $h$ at

$$
t_h=\frac{3}{2a_p}\left[(h+z_v)^{-2/3}-(H+z_v)^{-2/3}\right].
$$

Below the opening, the implicit solution is

$$
t-t_h=\frac1{a_p}\int_{z_f}^{h}
\frac{d\zeta}{(\zeta+z_v)^{5/3}-z_v^{5/3}}.
$$

The model assumes an effective point opening with one-way source-volume exhaust; a tall opening supporting simultaneous density-driven exchange would need additional boundary-flow equations.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
