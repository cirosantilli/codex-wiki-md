<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Each coordinate projection $S_j$ is compact, hence a [Lebesgue measurable set](../../../../../../lebesgue-measurable-set.md), because it is the continuous image of the compact set $K$. Its $(d-1)$-dimensional measure is finite. Choose any nonnegative integrable function $\eta$ on $\mathbb R$ with integral one, and define

$$
f(x)=1_K(x),\qquad s_j(x)=1_{S_j}(\widehat x_j)\eta(x_j).
$$

If $x\in K$, every projection $\widehat x_j$ belongs to $S_j$. If $x\notin K$, $f(x)=0$. Thus for every $j$, $f(x)\leq1_{S_j}(\widehat x_j)=\int s_j(\widehat x_j,t)\,dt$, so the introductory estimate applies. [Tonelli theorem](../../../../../../tonelli-theorem.md) gives $\|s_j\|_1=\lambda_{d-1}(S_j)$, and

$$
\|1_K\|_{d/(d-1)}=\lambda_d(K)^{(d-1)/d}.
$$

Substitute these values and raise to the $d$th power:

$$
\boxed{\lambda_d(K)^{d-1}\leq\prod_{j=1}^d\lambda_{d-1}(S_j)}.
$$

This proves the geometric [Loomis--Whitney inequality](../../../../../../loomis-whitney-inequality.md), including zero-volume sets or zero-measure projections, without any division by their measures.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
