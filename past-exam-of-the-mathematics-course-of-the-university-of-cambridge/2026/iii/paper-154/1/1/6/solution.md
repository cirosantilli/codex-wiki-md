<h1 id="1/1/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Take the regular radial solution with $u(0)=1$. In the transformed variables it satisfies

$$
v(s)\sim e^{as},\qquad \dot v(s)\sim ae^{as}
\quad(s\to-\infty),
$$

so $J(s)\to0$. Since $s_c>1$, the [Lyapunov function](../../../../../../../lyapunov-function.md) immediately becomes negative. The trajectory cannot reach $v=0$, where $J=\dot v^2\geq0$, and $J<0$ confines it below the positive zero of $f$. Hence it remains positive and bounded for all $s$.

The identity $\dot J=-4(s_c-1)\dot v^2$ and the [LaSalle invariance principle](../../../../../../../lasalle-s-invariance-principle.md) force the omega-limit set to consist of equilibria. The negative limiting energy excludes $v=0$, leaving

$$
v(s)\longrightarrow c_\infty.
$$

Consequently

$$
r^{2/(p-1)}u(r)\longrightarrow c_\infty>0,
$$

so $\alpha=2/(p-1)$. At infinity, $|u'(r)|\sim ac_\infty r^{-a-1}$, and

$$
\int^infty |u'(r)|^2r^{d-1},dr
\asymp\int^infty r^{d-3-2a},dr
=\int^infty r^{2s_c-3},dr=\infty
$$

because $s_c>1$. Thus $\nabla u\notin L^2(\mathbb R^d)$.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 154](../../../../paper-154-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
