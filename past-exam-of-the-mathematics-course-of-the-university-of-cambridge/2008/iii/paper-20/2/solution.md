<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the following [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md), whose columns reduce modulo three to four of the specified nonzero [tetracode](../../../../../tetracode.md) words:

$$
S=\begin{pmatrix}0&1&1&1\\-1&0&-1&1\\-1&1&0&-1\\-1&-1&1&0\end{pmatrix},\qquad S^T=-S,\qquad S^2=-3I.
$$

Set $B_+=3I+S$, $B_-=-3I+S$, and define the full [Euclidean lattices](../../../../../euclidean-lattice.md) $L_\pm^0=B_\pm\mathbb Z^4$. Their determinants have absolute value $144$, since

$$
B_+^{-1}=\frac{3I-S}{12},\qquad B_-^{-1}=\frac{-3I-S}{12}.
$$

For arbitrary positive real numbers $a_1,\ldots,a_4$, put $D=\operatorname{diag}(\sqrt{a_1},\ldots,\sqrt{a_4})$ and $L_\pm=DL_\pm^0$. This is the [tetracode length-isospectral lattice construction](../../../../../tetracode-length-isospectral-lattice-construction.md). We prove equality of the length multisets by an explicit [bijection](../../../../../bijection.md), not just equality of the shortest lengths.

Modulo three, both [lattices](../../../../../lattice.md) have image $\operatorname{im}S=T$. The [matrix](../../../../../matrix.md) $S$ has rank two over $\mathbb F_3$; its four column lines are precisely the four lines in $T$. Also $S^2=0$ modulo three, so $\ker S=\operatorname{im}S=T$. Each nonzero [tetracode](../../../../../tetracode.md) word has exactly one zero coordinate. Every $v\in L_\pm^0$ therefore has some coordinate divisible by three. Moreover, all four coordinates of $v$ have the same parity, because every entry of either $B_\pm$ is odd.

For $v\in L_+^0$, choose the least index $i$ with $3\mid v_i$ and set $w=v-2v_ie_i$. The [coordinate reflection bijection for tetracode lattices](../../../../../coordinate-reflection-bijection-for-tetracode-lattices.md) will show that $w\in L_-^0$. First, $w\equiv v\pmod3$, so $Sw\equiv0\pmod3$. Second, positive-lattice membership implies $Sv\equiv3v\equiv-v\pmod4$. Hence

$$
(I-S)w\equiv2\bigl(v-v_ie_i+v_iSe_i\bigr)\pmod4.
$$

The expression in parentheses has $i$th coordinate zero and every other coordinate $v_j+v_iS_{ji}$ even, by the common parity and $S_{ji}=\pm1$. Thus $(I-S)w\equiv0\pmod4$. Together the congruences modulo three and four say $(-3I-S)w\equiv0\pmod{12}$, which is precisely $B_-^{-1}w\in\mathbb Z^4$.

Conversely, if $v\in L_-^0$, the same reflection has unchanged reduction modulo three, and now $Sv\equiv v\pmod4$. Thus

$$
(3I-S)(v-2v_ie_i)\equiv2\bigl(v+v_ie_i+v_iSe_i\bigr)\pmod4.
$$

Its $i$th coordinate is $4v_i$ and its other coordinates are even multiples of two, so it vanishes modulo four; it vanishes modulo three as well. The reflected vector is in $L_+^0$. The chosen index is unchanged by reflection, including for vectors reducing to zero, so this map is an [involution](../../../../../involution.md) between the two [lattices](../../../../../lattice.md). It preserves every $|v_j|$ and therefore preserves $\|Dv\|^2=\sum_j a_jv_j^2$. **The two lattices have the same length spectrum, including every multiplicity, for every positive choice of weights.**

To prove a genuine failure of [isometry](../../../../../isometry.md), choose

$$
(a_1,a_2,a_3,a_4)=(1,\sqrt2,\sqrt3,\sqrt5).
$$

These four numbers are linearly independent over $\mathbb Q$: changing the signs of the independent square roots in the [multiquadratic field](../../../../../multiquadratic-field.md) $\mathbb Q(\sqrt2,\sqrt3,\sqrt5)$ isolates each coefficient of a rational relation. If an [orthogonal transformation](../../../../../orthogonal-transformation.md) $O$ maps $L_+$ to $L_-$, then

$$
P=D^{-1}OD=B_-UB_+^{-1}\in\operatorname{GL}_4(\mathbb Q),\qquad U\in\operatorname{GL}_4(\mathbb Z),
$$

and $P^T\operatorname{diag}(a_j)P=\operatorname{diag}(a_j)$. Comparing rational coefficients of the independent $a_j$ in the diagonal entries gives $P_{ji}^2=\delta_{ji}$. Consequently $P$ is diagonal with entries $\pm1$.

Such a coordinate sign change must preserve $T$ modulo three. For each zero coordinate $i$, there are exactly two opposite nonzero [tetracode](../../../../../tetracode.md) words. Preserving their line requires the other three signs to be equal. Taking two different zero coordinates forces all four signs to be equal. Thus $P=I$ or $P=-I$, either of which would imply $L_+^0=L_-^0$. But

$$
v=B_+e_1=(3,-1,-1,-1)^T,\qquad B_-^{-1}v=(-1/2,1/2,1/2,1/2)^T\notin\mathbb Z^4.
$$

This contradiction proves **$L_+$ and $L_-$ are not isometric**. Allowing affine [isometries](../../../../../isometry.md) changes nothing: translating the image of zero back to zero reduces them to the orthogonal case.

For the [flat tori](../../../../../flat-torus.md), take period lattices equal to the [dual lattices](../../../../../dual-lattice.md):

$$
X_\pm=\mathbb R^4/L_\pm^\vee.
$$

The standard [spectrum of a flat torus](../../../../../spectrum-of-a-flat-torus.md) lemma states that its [characters of a real torus](../../../../../characters-of-a-real-torus.md) are indexed by the dual of its period lattice. Here they are $e^{2\pi i\langle v,x\rangle}$ for $v\in L_\pm$, with [Laplacian](../../../../../laplacian.md) [eigenvalue](../../../../../eigenvalue.md) $4\pi^2\|v\|^2$. These [characters](../../../../../character-of-a-representation.md) give a complete orthogonal basis, so our length-preserving [bijection](../../../../../bijection.md) proves that $X_+$ and $X_-$ are [isospectral manifolds](../../../../../isospectral-manifolds.md). The second standard lemma is that an [isometry](../../../../../isometry.md) of [flat tori](../../../../../flat-torus.md) lifts to an affine [isometry](../../../../../isometry.md) of their Euclidean universal covers. Its orthogonal part maps the period lattices to one another, and therefore maps their [dual lattices](../../../../../dual-lattice.md) to one another. This would give the impossible [isometry](../../../../../isometry.md) $L_+\cong L_-$. Hence **$X_+$ and $X_-$ are isospectral non-isometric flat four-dimensional tori**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
