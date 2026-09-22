<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The given two-dimensional ternary subspace is the [tetracode](../../../../../tetracode.md). Its nonzero words form four one-dimensional subspaces, represented by

$$
(0,1,1,1),\quad(1,1,-1,0),\quad(1,-1,0,1),\quad(-1,0,-1,1).
$$

Every nonzero word has exactly three nonzero coordinates; in particular every codeword has a zero coordinate. We use this zero coordinate to construct a length-preserving reflection, but then choose unequal coordinate weights to rule out a global [isometry](../../../../../isometry.md).

The [parity congruence description of tetracode lattices](../../../../../parity-congruence-description-of-tetracode-lattices.md) is especially convenient. Define integer [Euclidean lattices](../../../../../euclidean-lattice.md)

$$
\begin{aligned}
\Gamma_+&=\{x\in\mathbb Z^4:x\bmod3\in T,\ x_1\equiv x_2\equiv x_3\equiv x_4\pmod2,\ \textstyle\sum_jx_j\equiv0\pmod4\},\\
\Gamma_-&=\{x\in\mathbb Z^4:x\bmod3\in T,\ x_1\equiv x_2\equiv x_3\equiv x_4\pmod2,\ \textstyle\sum_jx_j-2x_1\equiv0\pmod4\}.
\end{aligned}
$$

These congruences define additive subgroups of $\mathbb Z^4$ containing $12\mathbb Z^4$, so they are discrete and have full rank. For all-even vectors the last conditions coincide. For all-odd vectors they require respectively coordinate sum zero or two modulo four.

For an explicit basis, set

$$
S=\begin{pmatrix}0&1&1&1\\-1&0&-1&1\\-1&1&0&-1\\-1&-1&1&0\end{pmatrix},\qquad B_\pm=\pm3I+S.
$$

Their columns reduce to $T$ modulo three and satisfy the stated parity congruences, so $B_\pm\mathbb Z^4\subseteq\Gamma_\pm$. Since $S^2=-3I$, $|\det B_\pm|=144$. Conversely, the modulo-three condition has index nine, while each allowed set of residues modulo four has sixteen elements out of $4^4$: eight all-even and eight all-odd residues. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) therefore gives $[\mathbb Z^4:\Gamma_\pm]=9\cdot16=144$. The inclusions have equal index and are equalities.

For any $x\in\Gamma_+$, choose the first coordinate $j$ for which $x_j\equiv0\pmod3$, and reflect that coordinate:

$$
F(x)=x-2x_je_j.
$$

Such a coordinate always exists by the codeword description. Its reflection preserves $x\bmod3\in T$ and the common coordinate parity. If $x$ is odd, its sum changes by two modulo four, taking the plus condition to the minus condition. If $x$ is even, the sum changes by zero modulo four, and the two conditions already coincide. The set of coordinates divisible by three is unchanged, so applying the same rule again recovers $x$. This proves a bijection $F:\Gamma_+\to\Gamma_-$ preserving each absolute coordinate, the [coordinate reflection bijection for tetracode lattices](../../../../../coordinate-reflection-bijection-for-tetracode-lattices.md).

Now choose positive weights linearly independent over $\mathbb Q$, for instance

$$
(a_1,a_2,a_3,a_4)=(1,\sqrt2,\sqrt3,\sqrt6),\qquad D=\operatorname{diag}(\sqrt{a_1},\ldots,\sqrt{a_4}),\qquad L_\pm=D\Gamma_\pm.
$$

The [Euclidean lattices](../../../../../euclidean-lattice.md) $L_+$ and $L_-$ have the same multiset of vector lengths, because $\|Dx\|^2=\sum_j a_jx_j^2$ is preserved by $F$. A closed [geodesic](../../../../../geodesic.md) of a [flat torus](../../../../../flat-torus.md) is the projection of a straight line with displacement a lattice vector. Thus the two tori have identical [length spectra](../../../../../length-spectrum.md), including multiplicities of lattice displacements. Primitive lengths can also be recovered by subtracting proper iterates successively, so they agree as well.

Suppose a torus [isometry](../../../../../isometry.md) existed. Its lift to $\mathbb R^4$ is affine with orthogonal linear part $R$ taking $L_+$ onto $L_-$. Put $A=D^{-1}RD$, so $A\Gamma_+=\Gamma_-$. Since $12e_i\in\Gamma_+$, its image is an integer vector $y$ satisfying

$$
\sum_j a_jy_j^2=144a_i.
$$

Rational independence of the weights forces $y_j^2=144\,1_{j=i}$. Hence $Ae_i=\pm e_i$ for every $i$: the [rationally independent axis weights obstruct a lattice isometry](../../../../../rationally-independent-axis-weights-obstruct-a-lattice-isometry.md) by forcing it to be a diagonal sign change.

Such a sign change would preserve $T$ modulo three. The code has a unique nonzero projective word supported on each triple of coordinates, so preserving each of its four support sets forces the three signs on each triple to agree. All four signs therefore agree, leaving only $A=I$ or $A=-I$. Both preserve $\Gamma_+$ rather than exchanging it with $\Gamma_-$. These lattices are distinct: $(3,-1,-1,-1)\in\Gamma_+$ is odd and has sum zero, so is not in $\Gamma_-$. This contradiction proves

$$
\boxed{\mathbb R^4/L_+\text{ and }\mathbb R^4/L_-\text{ have equal length spectra and are not isometric}.}
$$

The choice of weights is essential; setting all four equal would make the displayed bases orthogonal with equal lengths and would not prove nonisometry.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
