<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $P=\sum_{j\leq\alpha}p_j(x)\partial^j$, setting unused [coefficients](../../../../../../coefficient.md) to zero. Split the [Adler trace](../../../../../../adler-trace.md) into its fixed leading part and variable parts:

$$
l_P(L)=\operatorname{Tr}(P\partial^m)
+\sum_{l=0}^{m-1}\operatorname{Tr}(P u_l\partial^l).
$$

Cyclicity from part (i) gives

$$
\operatorname{Tr}(P u_l\partial^l)
=\operatorname{Tr}(u_l\partial^lP)
=\int u_l\operatorname{res}(\partial^lP)\,dx.
$$

Thus this [Hamiltonian trace functional on monic differential operators](../../../../../../hamiltonian-trace-functional-on-monic-differential-operators.md) has the required form

$$
\boxed{l_P(L)=c+\sum_{l=0}^{m-1}\int a_l(x)u_l(x)\,dx,\qquad
c=\int p_{-m-1}(x)\,dx,\quad a_l=\operatorname{res}(\partial^lP).}
$$

To make each [coefficient](../../../../../../coefficient.md) explicit, expand $\partial^lp_j$ by the [Leibniz rule](../../../../../../leibniz-rule.md). A term with $k$ [derivatives](../../../../../../derivative.md) of $p_j$ contributes to the residue exactly when $l-k+j=-1$. Consequently,

$$
\boxed{a_l(x)=\sum_{k=0}^l\binom lk p_{k-l-1}^{(k)}(x).}
$$

These are [smooth functions](../../../../../../smooth-function.md) depending on $P$, not on the variable [coefficients](../../../../../../coefficient.md) of $L$. In particular $a_0=p_{-1}$ and $a_1=p_{-2}+p_{-1}'$. The [coefficient](../../../../../../coefficient.md) $a_0$ must be included: it appears in the displayed sum even though the printed [coefficient](../../../../../../coefficient.md) list starts at $a_1$.

The monic operators form an [affine space](../../../../../../affine-space.md), not a vector space. Accordingly $l_P$ is affine in the coordinates $u_l$, with constant $c$, and its differential is linear in variations. Its [variational derivatives](../../../../../../variational-derivative.md) are $\delta l_P/\delta u_l=a_l$. It is the restriction of a linear trace pairing on the full operator space, which explains the terminology without discarding the constant term.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
