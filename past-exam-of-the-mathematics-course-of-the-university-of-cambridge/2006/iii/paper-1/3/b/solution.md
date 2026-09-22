<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take curves $g(s),h(t)$ through the identity with tangent vectors $X,Y$. Form the local group [commutator](../../../../../../commutator.md) $c(s,t)=g(s)h(t)g(s)^{-1}h(t)^{-1}$. In a smooth coordinate chart at the identity, its leading mixed term defines the [Lie bracket](../../../../../../lie-bracket.md):

$$
[X,Y]=\partial_s\partial_t c(s,t)\big|_{s=t=0}
$$

for a matrix group, where the identity's constant term has zero derivative. More generally take this derivative in the chart with the identity sent to zero. Since the first derivatives vanish on the coordinate axes, changing charts changes the mixed coefficient only by the tangent-space coordinate transformation, so the definition is intrinsic.

For the displayed nilpotent matrices choose $g(s)=I+sX$ and $h(t)=I+tY$, which lie in $\mathrm{SL}_2$. Their inverses are $I-sX$ and $I-tY$. Direct multiplication gives

$$
g(s)h(t)g(s)^{-1}h(t)^{-1}
=\begin{pmatrix}1+st+s^2t^2&-s^2t\\st^2&1-st\end{pmatrix}.
$$

Its mixed derivative is therefore

$$
\boxed{[X,Y]=\begin{pmatrix}1&0\\0&-1\end{pmatrix}=H.}
$$

Interchanging the two curves gives

$$
h(t)g(s)h(t)^{-1}g(s)^{-1}
=\begin{pmatrix}1-st&s^2t\\-st^2&1+st+s^2t^2\end{pmatrix},
$$

whose mixed derivative is $-H$. Thus **$[X,Y]=-[Y,X]$** directly from the curve definition. The general matrix expansion likewise gives the [commutator](../../../../../../commutator.md) $XY-YX$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
