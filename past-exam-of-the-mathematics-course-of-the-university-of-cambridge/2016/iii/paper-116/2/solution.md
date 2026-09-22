<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An index-$h$ handle is $D^h\times D^{n-h}$, attached along $S^{h-1}\times D^{n-h}$. Its [attaching sphere](../../../../../attaching-sphere.md) is $S^{h-1}\times\{0\}$ with its attaching [framing of an embedded sphere](../../../../../framing-of-an-embedded-sphere.md), and its [belt sphere](../../../../../belt-sphere.md) in the new boundary is $\{0\}\times S^{n-h-1}$. A [handle decomposition](../../../../../handle-decomposition.md) is an ordered sequence of such [handle attachments](../../../../../handle-attachment.md).

A [handle slide](../../../../../handle-slide.md) of one $h$-handle over another replaces its framed [attaching sphere](../../../../../attaching-sphere.md) by a [band sum](../../../../../band-sum.md) with a parallel framed copy of the second [attaching sphere](../../../../../attaching-sphere.md), along a band in the boundary of the previously attached handles. The second handle stays fixed. The band transports the [framing of an embedded sphere](../../../../../framing-of-an-embedded-sphere.md). The union of the two handles and their attaching collars can be reidentified by a [diffeomorphism](../../../../../diffeomorphism.md), so this changes the decomposition, rather than the underlying [manifold](../../../../../topological-manifold.md). A sequence of these moves, allowing the usual isotopies of attaching data, gives handle decompositions related by slides. Reading the decomposition backwards interchanges [attaching spheres](../../../../../attaching-sphere.md) and [belt spheres](../../../../../belt-sphere.md); a slide of dual handles is a slide of the corresponding original handles.

For the standard handle-calculus assertion, take $1\leq k\leq n-2$, so both the relevant attaching and belt spheres are connected. We need the local geometric move behind [handle-slide isolation of a cancelling pair](../../../../../handle-slide-isolation-of-a-cancelling-pair.md). Write $p=A_1\cap B_1$. If $q$ is an intersection of some $A_j$, $j>1$, with $B_1$, choose an arc on $B_1$ from $q$ to $p$, and take a narrow parallel band to the unique sheet of $A_1$ at $p$. Slide $A_j$ over an appropriate parallel copy of $A_1$. Choose the copy's orientation so that the new sheet at $p$ has the opposite local [smooth intersection number](../../../../../smooth-intersection-number.md) to the sheet at $q$.

Within a thin neighbourhood of the arc, the old sheet at $q$ and the added sheet at $p$ are the two ends of one band. An isotopy pushes that band through the neighbourhood of $B_1$ and removes both ends. Outside this neighbourhood the original $A_j$ is unchanged, apart from the added copy of the parts of $A_1$ away from $B_1$. Since $A_1$ meets $B_1$ only at $p$, this copy contributes no further intersections with $B_1$. Thus **one slide followed by an isotopy removes one original geometric intersection with $B_1$**. This is a local band move, not an appeal to handle cancellation or to an algebraic cancellation of signs.

The arcs and bands may be chosen one at a time; in the one-dimensional sphere case, start with an intersection adjacent to $p$, so that the arc interior contains no other intersection. Perturb to make all intersections transverse. The relevant spheres are compact, so there are only finitely many intersections. Repeating the move for every $j>1$ leaves $A_1$ and $B_1$ fixed and gives

$$
\boxed{A'_1\cap B'_1=\{p\},\qquad A'_j\cap B'_1=\varnothing\quad(j>1).}
$$

The bands can avoid the remaining attaching data; any consequent change to intersections with other [belt spheres](../../../../../belt-sphere.md) is allowed at this stage.

For the second stage, view the same interface from the dual decomposition. Now $B'_i$ are [attaching spheres](../../../../../attaching-sphere.md) and $A'_j$ are [belt spheres](../../../../../belt-sphere.md). Apply the same local move to each intersection of $B'_i$, $i>1$, with $A'_1$, sliding that dual handle over the one with attaching sphere $B'_1$. This changes the original $k$-handles. It keeps $A'_1$ and $B'_1$ fixed, while removing the unwanted intersections with $A'_1$. The parallel copies and bands may be taken disjoint from all $A'_j$, $j>1$, because those spheres are already disjoint from $B'_1$ and from $A'_1$. Hence their intersections with $B'_1$ remain empty. We obtain

$$
\boxed{A''_1\cap B''_1=\{p\},\qquad A''_j\cap B''_1=\varnothing\ (j>1),\qquad A''_1\cap B''_i=\varnothing\ (i>1).}
$$

No handle has been removed.

There is an implicit index-range qualification in this geometric assertion. If arbitrary zero-handles are included, the second conclusion need not hold: two zero-handles joined by one one-handle have an attaching zero-sphere with one endpoint on each zero-handle belt sphere. Slides preserving this handle inventory cannot make its second endpoint avoid both belts. The dual obstruction occurs for top-index handles. Thus the argument uses the customary intermediate-index setting of the handle-slide lemma; the unqualified assertion at the extreme indices would require additional hypotheses or additional moves.

For the numerical formula, fix coherent [orientations](../../../../../orientation-of-a-simplex.md) for the integer [smooth intersection numbers](../../../../../smooth-intersection-number.md), and let

$$
m_{ji}=A_j\cdot B_i,\qquad\delta=m_{11}\in\{1,-1\}.
$$

Keep the orientation at the surviving point, so its number remains $\delta$. A slide of a $(k+1)$-handle adds or subtracts the first row of the intersection matrix. Removing all geometric intersections in the first column has net row operation

$$
R'_j=R_j-\frac{m_{j1}}{\delta}R_1\quad(j>1),\qquad R'_1=R_1.
$$

Even if opposite-sign intersections require extra slides, their net signed coefficient is the displayed one. In particular,

$$
m'_{ji}=m_{ji}-\frac{m_{j1}m_{1i}}{\delta}\quad(j>1),\qquad m'_{1i}=m_{1i}.
$$

The dual slides then perform the column operations

$$
C''_i=C'_i-\frac{m_{1i}}{\delta}C'_1\quad(i>1),\qquad C''_1=C'_1.
$$

Since $C'_1=(\delta,0,\ldots,0)^T$, these operations leave the lower-right block unchanged. Thus the final answer, including both stages of slides, is

$$
\boxed{A''_l\cdot B''_k=
\begin{cases}
\delta,&l=k=1,\\
0,&l=1<k\text{ or }k=1<l,\\
m_{lk}-m_{l1}m_{1k}/\delta,&l>1,\ k>1.
\end{cases}}
$$

The remaining block is the [Schur complement](../../../../../schur-complement.md) of the unit pivot $\delta$. If the original orientation is chosen so that $\delta=1$, it is simply $m_{lk}-m_{l1}m_{1k}$. For unoriented handles use intersection numbers modulo $2$, with the same formula interpreted in $\mathbb F_2$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 116](../../paper-116-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
