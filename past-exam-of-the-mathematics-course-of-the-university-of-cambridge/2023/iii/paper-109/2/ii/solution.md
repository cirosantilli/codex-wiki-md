<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the four families from the hint. Put $N=2^n$, $u=|\mathcal U_1|/N$, and $v=|\mathcal V_1|/N$. The families $\mathcal U_1,\mathcal V_1$ are up-sets, while their complements $\mathcal U_2,\mathcal V_2$ are down-sets. Applying the [Harris-Kleitman inequality](../../../../../../harris-inequality.md) to the up-sets, and equivalently to the down-sets after taking complements of the ground set, gives

$$
|\mathcal U_1\cap\mathcal V_1|\geq Nuv,
\qquad
|\mathcal U_2\cap\mathcal V_2|\geq N(1-u)(1-v).
$$

The cross-incomparability assumption gives

$$
\mathcal A\subseteq\mathcal U_1\cap\mathcal V_2,
\qquad
\mathcal B\subseteq\mathcal U_2\cap\mathcal V_1.
$$

Consequently

$$
|\mathcal A|\leq Nu(1-v),
\qquad
|\mathcal B|\leq N(1-u)v.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) now yields

$$
\sqrt{|\mathcal A|}+\sqrt{|\mathcal B|}
\leq\sqrt N\bigl(\sqrt{u(1-v)}+\sqrt{(1-u)v}\bigr)
\leq\sqrt N=2^{n/2}.
$$

This is the sharp two-family [Cross-Sperner inequality](../../../../../../cross-sperner-inequality.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
