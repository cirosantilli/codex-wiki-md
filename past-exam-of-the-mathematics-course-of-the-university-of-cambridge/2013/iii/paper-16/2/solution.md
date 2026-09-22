<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Construct the [Euclidean lattices](../../../../../euclidean-lattice.md) in an orthogonal coordinate system whose squared axis lengths are

$$
(a_1,a_2,a_3,a_4)=(1,\sqrt2,\sqrt3,\sqrt6).
$$

Thus an integer coordinate vector $z$ has squared [norm](../../../../../norm.md) $\sum_i a_i z_i^2$. These four numbers are [linearly independent](../../../../../linear-independence.md) over $\mathbb Q$: the four sign changes of $\sqrt2,\sqrt3$ in their [field extension](../../../../../field-extension.md) isolate the four coefficients of a rational relation. The independence will distinguish the two [flat tori](../../../../../flat-torus.md); equality of their [length spectra](../../../../../length-spectrum.md) will hold for every positive choice of axis weights.

Let

$$
S=\begin{pmatrix}0&1&1&1\\-1&0&-1&1\\-1&1&0&-1\\-1&-1&1&0\end{pmatrix},\qquad A_+=3I+S,\qquad A_-=-3I+S,
\qquad L_\pm=A_\pm\mathbb Z^4.
$$

Here and below these integer coordinates are interpreted in the weighted orthogonal axes. Direct multiplication gives $S^T=-S$, $S^2=-3I$, and

$$
A_\pm^T A_\pm=12I,\qquad |\det A_\pm|=144.
$$

In particular both $L_\pm$ are full-rank [Euclidean lattices](../../../../../euclidean-lattice.md). Denote their four generator columns by $v_i^\pm$. Modulo $3$ the two matrices have the same columns, and the nonzero words of the given [ternary tetracode](../../../../../tetracode.md) $T$ are exactly

$$
\pm(0,1,1,1),\quad\pm(1,0,1,-1),\quad\pm(1,-1,0,1),\quad\pm(1,1,-1,0).
$$

These are the reductions of $\pm v_i^\pm$, respectively. The first and fourth displayed words are the specified generators, and the middle two arise from their sum and difference, up to sign. Thus reduction modulo $3$ maps either [Euclidean lattice](../../../../../euclidean-lattice.md) onto precisely $T$.

To construct a length-preserving correspondence, find the kernels $M_\pm=L_\pm\cap3\mathbb Z^4$ of this reduction. The inverse matrix is $A_\pm^{-1}=A_\pm^T/12$. Hence $3w\in L_\pm$ exactly when $A_\pm^Tw\equiv0\pmod4$. These congruences are equivalent to

$$
\begin{aligned}
M_+&=\{3w: w_1\equiv w_2\equiv w_3\equiv w_4\pmod2,\quad w_1+w_2+w_3+w_4\equiv0\pmod4\},\\
M_-&=\{3w: w_1\equiv w_2\equiv w_3\equiv w_4\pmod2,\quad w_1+w_2+w_3+w_4\equiv2w_1\pmod4\}.
\end{aligned}
$$

For clarity, the first $+$ congruence is $-(w_1+w_2+w_3+w_4)=0\pmod4$; subtracting the others gives evenness of each required pair sum. For the $-$ matrix the first congruence is $2w_1-(w_1+w_2+w_3+w_4)=0\pmod4$; the remaining congruences again give equality of the four parities. Substitution proves the converse in each case.

Let $R_i$ be the [orthogonal reflection](../../../../../reflection-in-a-hyperplane.md) changing only coordinate $i$. If the coordinates of $w$ are even, this changes their sum by a multiple of $4$; if all are odd, it changes the sum by $2$ modulo $4$. Therefore

$$
R_i M_+=M_-\quad\hbox{for every }i,\qquad R_i v_i^+=v_i^-.
$$

Each [Euclidean lattice](../../../../../euclidean-lattice.md) is the disjoint union of its kernel and the eight [cosets](../../../../../coset.md) $\pm v_i^\pm+M_\pm$, since $T$ has nine words. Define a map $\Phi:L_+\to L_-$ by using $R_1$ on $M_+$ and $R_i$ on each of $v_i^++M_+$ and $-v_i^++M_+$. Each piece maps bijectively onto the corresponding $-$ coset. Thus $\Phi$ is a [bijection](../../../../../bijection.md) satisfying

$$
\boxed{|\Phi(z)_i|=|z_i|\quad(1\le i\le4),\qquad\|\Phi(z)\|=\|z\|.}
$$

It also commutes with $z\mapsto-z$. The [closed geodesics](../../../../../closed-geodesic.md) of a [flat torus](../../../../../flat-torus.md) have lengths $\|z\|$ for nonzero translation vectors $z$ in its [Euclidean lattice](../../../../../euclidean-lattice.md). Consequently the two [length spectra](../../../../../length-spectrum.md) agree, including the multiplicities of translation classes and with either consistent orientation convention. If only primitive [closed geodesics](../../../../../closed-geodesic.md) are counted, the same conclusion follows by removing iterates in increasing order of length: the total multiplicity at $\ell$ is the sum of primitive multiplicities at $\ell/k$, and there are only finitely many such contributions below any fixed length. The correspondence need not itself preserve primitiveness to give this conclusion.

It remains to prove **the two flat tori are not isometric**. An [isometry](../../../../../isometry.md) of [flat tori](../../../../../flat-torus.md) lifts to an affine [Euclidean isometry](../../../../../euclidean-isometry.md); its [linear part of an affine map](../../../../../linear-part-of-an-affine-map.md) must carry $L_+$ onto $L_-$. In integer coordinates write this part as $B$. For every $z\in L_+$, both $z$ and $Bz$ have integer coordinates and have equal squared [norms](../../../../../norm.md). Rational independence of the $a_i$ implies

$$
(Bz)_i^2=z_i^2\quad\hbox{for every }i\hbox{ and every }z\in L_+.
$$

Apply this to $z=A_+n$ for all $n\in\mathbb Z^4$. Two squared linear forms agreeing on all integer points agree as [polynomials](../../../../../polynomial-split.md); their difference factors, so one form is the other or its negative. Since $A_+$ is invertible, $B$ is consequently a diagonal sign change $D=\operatorname{diag}(\varepsilon_1,\ldots,\varepsilon_4)$.

Modulo $3$, such a $D$ must preserve $T$. Each nonzero word of $T$ has exactly three nonzero coordinates, and for each choice of zero coordinate there are just two such words, differing by an overall sign. Preserving these words forces the three signs on each support to agree. The four overlapping supports then force $\varepsilon_1=\varepsilon_2=\varepsilon_3=\varepsilon_4$. Thus only $D=I$ and $D=-I$ are possible. Neither changes $L_+$.

Finally $v_1^+\notin L_-$: it has the same ternary word as $v_1^-$, but their difference is $6e_1=3(2,0,0,0)$, which fails the congruence defining $M_-$. Hence $L_+\ne L_-$ and no such [linear isometry](../../../../../linear-isometry-of-hilbert-spaces.md) exists. This completes the [tetracode length-isospectral lattice construction](../../../../../tetracode-length-isospectral-lattice-construction.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
