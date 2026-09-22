<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\delta=-A^2-A^{-2}$. Normalize the reduced [Kauffman bracket](../../../../../../kauffman-bracket.md) by $\langle\bigcirc\rangle=1$ and $\langle D\sqcup\bigcirc\rangle=\delta\langle D\rangle$. At a positive braid crossing choose the smoothing rule $R_i=A1+A^{-1}e_i$, where $1$ is the two parallel strands and $e_i$ joins the adjacent top endpoints and adjacent bottom endpoints. At its mirror crossing the coefficients are interchanged. This convention fixes the two smoothing labels. Equivalently, for a nonempty diagram,

$$
\boxed{\langle D\rangle=\sum_{s}A^{a(s)-b(s)}\delta^{c(s)-1},}
$$

where each [bracket smoothing state](../../../../../../bracket-smoothing-state.md) chooses one smoothing at each crossing, $a,b$ count the choices, and $c$ counts the resulting circles. It is a Laurent polynomial in $A$ and is independent of the order in which crossings are resolved.

We prove the local invariance needed for the [Jones polynomial](../../../../../../jones-polynomial.md). In the [Temperley-Lieb diagram algebra](../../../../../../temperley-lieb-diagram-algebra.md), stacking the smoothing tangles gives $e_i^2=\delta e_i$, $e_ie_{i+1}e_i=e_i$ and its reflected version. These identities follow just by following the planar strands; only the first removes an extra circle. The inverse crossing is $R_i^{-1}=A^{-1}1+Ae_i$, and

$$
R_iR_i^{-1}=1+(A^2+A^{-2}+\delta)e_i=1.
$$

Thus the second [Reidemeister move](../../../../../../reidemeister-move.md) preserves the bracket. Expanding three crossings gives

$$
R_1R_2R_1-R_2R_1R_2
=A^{-1}(A^2+\delta+A^{-2})(e_1-e_2)=0,
$$

so the third [Reidemeister move](../../../../../../reidemeister-move.md) does too; inverse versions follow by multiplying by inverse crossings. A positive curl resolves to $A\delta+A^{-1}=-A^3$ times the straight strand, and a negative curl gives $A^{-1}\delta+A=-A^{-3}$. Thus the first move changes the bracket by the indicated factor.

Orient the diagram and let $w(D)$ be its [writhe](../../../../../../writhe.md), the sum of the signed crossings. Define

$$
\boxed{V_D(t)=(-A^3)^{-w(D)}\langle D\rangle\big|_{t=A^{-4}}.}
$$

The first move changes $w$ by $+1$ or $-1$, exactly cancelling the bracket's curl factor. The other two moves leave [writhe](../../../../../../writhe.md) unchanged. Planar isotopy leaves both quantities unchanged. The Reidemeister theorem states that diagrams of ambient-isotopic tame oriented links are related by planar isotopy and these three local moves; therefore $V_D$ depends only on the oriented link.

This substitution really lies in $\mathbb Z[t^{1/2},t^{-1/2}]$. If there are $N$ crossings, each state exponent $a-b$ has parity $N$, and $w(D)$ also has parity $N$. Expanding each power of $\delta$ adds only even exponents, so every exponent of the normalized bracket has parity $N-3w(D)=0\pmod2$. Every even power of $A$ is an integral power of $t^{1/2}$. The normalization gives $V_{\mathrm{unknot}}=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
