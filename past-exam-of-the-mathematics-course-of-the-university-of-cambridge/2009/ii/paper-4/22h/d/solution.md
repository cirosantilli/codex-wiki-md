<h1 id="22h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The exact condition for this [diagonal operator on sequence space](../../../../../../diagonal-operator-on-sequence-space.md) is

$$
\boxed{T\text{ is compact on }\ell^2\quad\Longleftrightarrow\quad\lambda_n\longrightarrow0.}
$$

First, $T$ is bounded precisely when $\sup_n|\lambda_n|<\infty$, with [operator norm](../../../../../../operator-norm.md) equal to that supremum: the upper bound follows by summing $|\lambda_nx_n|^2$, and the coordinate unit vectors $e_n$ give the lower bound. If the supremum is infinite, choose distinct indices with $|\lambda_{n_j}|\ge j$ and set $x_{n_j}=1/j$, other coordinates zero. Then $x\in\ell^2$ but $Tx\notin\ell^2$, so the displayed prescription would not even define an everywhere-defined map into $\ell^2$.

If $T$ is compact but $\lambda_n\not\to0$, infinitely many indices satisfy $|\lambda_n|\ge\epsilon>0$. Along those indices,

$$
\|Te_n-Te_m\|^2=|\lambda_n|^2+|\lambda_m|^2\ge2\epsilon^2\quad(n\ne m),
$$

contradicting [compactness](../../../../../../compact-space.md). Conversely, if $\lambda_n\to0$, truncate to $T_Nx=(\lambda_1x_1,\ldots,\lambda_Nx_N,0,\ldots)$. This is a finite-rank [compact operator](../../../../../../compact-operator-split.md), and $\|T-T_N\|=\sup_{n>N}|\lambda_n|\to0$. To see [compactness](../../../../../../compact-space.md) directly, approximate the image of the [unit ball](../../../../../../unit-ball.md) by $T_N$ to within $\epsilon/2$, and cover its bounded finite-dimensional image by finitely many $\epsilon/2$-balls. Hence $T$'s unit-ball image is [totally bounded](../../../../../../totally-bounded-space.md); its closure is compact because $\ell^2$ is complete.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [22H](../../22h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
