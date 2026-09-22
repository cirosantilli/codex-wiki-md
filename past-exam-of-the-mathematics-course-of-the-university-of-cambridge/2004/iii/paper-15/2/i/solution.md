<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

One form of the [Theorem of the Cube](../../../../../../theorem-of-the-cube.md) is the cube principle: a [line bundle](../../../../../../line-bundle.md) $M$ on $E^3$ which is trivial on each of $E\times E\times\{O\}$, $E\times\{O\}\times E$, and $\{O\}\times E\times E$ is trivial. Here is a proof for a complex [elliptic curve](../../../../../../elliptic-curve.md).

Since $E$ is a real two-dimensional torus, its integral cohomology has no torsion. The [Künneth theorem](../../../../../../kunneth-theorem.md) decomposes

$$
H^2(E^3,\mathbb Z)=\bigoplus_{j=1}^3p_j^*H^2(E,\mathbb Z)\ \oplus\!\bigoplus_{i<j}H^1(E,\mathbb Z)\otimes H^1(E,\mathbb Z).
$$

Every single-factor summand is detected on a face containing that factor, and every cross summand is detected on the corresponding two-factor face. Restriction of $M$ to those faces is trivial, so its [First Chern class](../../../../../../first-chern-class.md) has zero component in every summand. Thus $c_1(M)=0$.

The [holomorphic exponential sequence](../../../../../../holomorphic-exponential-sequence.md) identifies the kernel of $c_1$ in the [holomorphic Picard group](../../../../../../holomorphic-picard-group.md) with $H^1(E^3,\mathcal O)/\operatorname{im}H^1(E^3,\mathbb Z)$. First cohomology decomposes factorwise here: $H^1(E^3,\mathcal O)=\bigoplus_jp_j^*H^1(E,\mathcal O)$ and likewise for integral first cohomology. Analytically the former decomposition says that the harmonic representatives of $(0,1)$-cohomology on the flat torus are the constant forms $d\overline z_j$, one from each factor. Consequently this kernel is $\operatorname{Pic}^0(E)^3$, and

$$
M\cong p_1^*M_1\otimes p_2^*M_2\otimes p_3^*M_3
$$

for degree-zero line bundles $M_j$ on $E$. Restrict to each coordinate axis. The hypothesis makes every $M_j$ trivial, so $M$ is trivial. This proves the [cohomological proof of the cube theorem for elliptic curves](../../../../../../cohomological-proof-of-the-cube-theorem-for-elliptic-curves.md); the holomorphic isomorphism is algebraic on these projective varieties by [GAGA](../../../../../../gaga-theorem.md).

To state its usual addition-map consequence, write $m_I:E^3\to E$ for summation of the coordinates indexed by $I$ and $p_j=m_{\{j\}}$. For any line bundle $L$ on $E$,

$$
\boxed{m_{123}^*L\otimes p_1^*L\otimes p_2^*L\otimes p_3^*L
\cong m_{12}^*L\otimes m_{13}^*L\otimes m_{23}^*L.}
$$

More canonically, include the inverse of the constant bundle with fibre $L_O$ in the alternating product. Its restriction to a zero-coordinate face has pairwise cancellations, leaving the trivial bundle. The cube principle proves its triviality, which gives the displayed isomorphism after choosing a trivialization of the constant fibre. Pullback along any triple of maps to $E$ gives the corresponding alternating identity for their seven nonempty sums.

A pointwise divisor version can also be seen directly from Question 1. For a divisor $D$ and fixed points $a,b,c$, the alternating translation divisor

$$
T_{a+b+c}^*D-T_{a+b}^*D-T_{a+c}^*D-T_{b+c}^*D+T_a^*D+T_b^*D+T_c^*D-D
$$

has degree zero and point sum zero: translation by $t$ subtracts $\deg(D)t$ from its point sum, and all the alternating terms cancel. The principality criterion proves that this divisor is principal.

Over a [number field](../../../../../../number-field.md) $K$, use algebraic line bundles and maps defined over $K$, and use Galois-invariant divisors rather than arbitrary individual complex points. **The geometric line-bundle cube identity itself is still exact over $K$.** To see descent in this setting, first pass to an algebraic closure, or an embedding in $\mathbb C$. The alternating bundle becomes trivial there by the preceding proof. Choose its nowhere-zero section with value one in a chosen $K$-basis at $(O,O,O)$. Any Galois conjugate of that section differs by an invertible global function, hence a constant on the connected projective variety; its normalized value at the rational origin forces that constant to be one. The section therefore descends, giving a $K$-defined trivialization.

For the arithmetic formulation used with heights, the necessary modification is a uniformly bounded error. A chosen [Weil height machine](../../../../../../weil-height-machine.md) representative $h_L$ satisfies

$$
\boxed{h_L(P+Q+R)-h_L(P+Q)-h_L(P+R)-h_L(Q+R)+h_L(P)+h_L(Q)+h_L(R)-h_L(O)=O(1),}
$$

uniformly for $P,Q,R\in E(K)$. Indeed, pullback and tensor product of line bundles correspond to composition and addition of heights only modulo bounded functions. This is the [arithmetic cube identity for Weil heights](../../../../../../arithmetic-cube-identity-for-weil-heights.md). Arbitrary naive heights do not satisfy an exact numerical cube identity; the [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md) removes the bounded error, as explained in Question 4. This arithmetic qualification does not weaken the exact geometric theorem.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
