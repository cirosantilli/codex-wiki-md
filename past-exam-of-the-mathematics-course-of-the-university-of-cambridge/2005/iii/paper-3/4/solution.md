<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use $[\lambda]$ for the ordinary [irreducible](../../../../../irreducible-representation.md) [character](../../../../../character-of-a-representation.md) of $S_{|\lambda|}$. Multiplication of different degrees is the product in the [induction ring of symmetric-group characters](../../../../../induction-ring-of-symmetric-group-characters.md): it induces an [external tensor product of group representations](../../../../../external-tensor-product-of-group-representations.md). For $\alpha\subseteq\nu$, the [skew Young diagram](../../../../../skew-young-diagram.md) $\nu/\alpha$ is the set of cells of $\nu$ outside $\alpha$. A filling of it is a [semistandard Young tableau](../../../../../semistandard-young-tableau.md) when entries weakly increase along rows and strictly increase down columns. Its content $\beta$ means that $i$ occurs $\beta_i$ times. Its reading word takes each row right to left and the rows top to bottom. A [lattice word](../../../../../lattice-word.md) has, in every initial segment, at least as many $i$'s as $(i+1)$'s for every $i$.

The [Littlewood–Richardson rule](../../../../../littlewood-richardson-rule.md) says

$$
[\alpha][\beta]=\sum_{\nu\vdash |\alpha|+|\beta|}c_{\alpha\beta}^\nu[\nu],
$$

where the [Littlewood–Richardson coefficient](../../../../../littlewood-richardson-coefficient.md) $c_{\alpha\beta}^\nu$ counts such skew semistandard fillings with content $\beta$ and lattice reading word. If $\alpha$ is not contained in $\nu$, the coefficient is zero. Over [characteristic zero](../../../../../characteristic-zero.md) this is an actual direct-sum multiplicity statement; over other [fields](../../../../../field.md) the analogous statement describes a [Specht filtration](../../../../../specht-filtration.md), not necessarily a decomposition into simple [modules](../../../../../module-mathematics.md).

For the required coefficient, the five skew cells are

$$
(1,4),(1,5),\quad(2,3),\quad(3,2),\quad(4,1).
$$

Their columns are all distinct. Content $(3,2)$ uses three $1$'s and two $2$'s. The first reading letter must be $1$ by the [lattice word](../../../../../lattice-word.md) condition, and row monotonicity forces both top cells to be $1$. The remaining three cells, in reading order, can then be filled by $122$, $212$, or $221$. The resulting words $11122$, $11212$, $11221$ all satisfy the lattice inequalities, and exhaust the possibilities. Thus

$$
\boxed{c_{(3,2,1),(3,2)}^{(5,3,2,1)}=3.}
$$

For the [determinantal form of a symmetric-group character](../../../../../determinantal-form-of-a-symmetric-group-character.md), set $[0]=1$ in degree zero and $[r]=0$ for $r<0$. The one-row [character](../../../../../character-of-a-representation.md) $[r]$ is trivial. The one-row specialization of the [Littlewood–Richardson rule](../../../../../littlewood-richardson-rule.md) is the [Pieri rule](../../../../../pieri-rule.md): multiplication by $[r]$ adds a [horizontal strip](../../../../../horizontal-strip.md) of $r$ cells, since all entries are $1$ and no column can contain two of them.

Here is an explicit [determinant](../../../../../determinant.md) argument, so that the desired form is genuinely deduced. Under the [Frobenius characteristic map](../../../../../frobenius-characteristic-map.md), $[r]$ corresponds to the [complete homogeneous symmetric polynomial](../../../../../complete-homogeneous-symmetric-polynomial.md) $h_r$, whose monomials enumerate weakly increasing sequences of $r$ entries. Fix $N$ variables and $l$ rows. Let a directed lattice path run right or up from $A_i=(-i,1)$ to $B_j=(\lambda_j-j,N)$, and assign weight $x_k$ to a horizontal step at height $k$ and weight one to a vertical step. The sum of its weights is $h_{\lambda_j-j+i}$. Expanding the [determinant](../../../../../determinant.md) of this path matrix sums signed families connecting the sources to a [permutation](../../../../../permutation.md) of the destinations.

Cancel intersecting families as follows. Choose the first intersection in a fixed order of vertices, and then the first pair of paths meeting there. Exchange their tails after that vertex. The total weight is unchanged, while the endpoint [permutation](../../../../../permutation.md) changes by a [transposition](../../../../../transposition-permutation.md), reversing the sign. Choosing the intersection in this fixed order makes the operation an involution. The surviving families are nonintersecting; the ordered sources and ordered destinations force the identity endpoint pairing. Record the heights of the horizontal steps of path $i$ as row $i$ of a tableau. Rows weakly increase, and nonintersection of successive paths is precisely strict increase down the shared columns. Conversely every [semistandard Young tableau](../../../../../semistandard-young-tableau.md) gives one surviving path family. Thus the [determinant](../../../../../determinant.md) has the semistandard-tableau generating function $s_\lambda$.

[Young's rule](../../../../../young-s-rule.md) identifies this generating function with the characteristic of $[\lambda]$: its coefficient at a monomial of weight $\mu$ is $K_{\lambda\mu}$, the multiplicity obtained by pairing with the [Young permutation module](../../../../../young-permutation-module.md) of type $\mu$. The [Frobenius characteristic map](../../../../../frobenius-characteristic-map.md) is injective and respects induction products. Transposing the path matrix does not change its [determinant](../../../../../determinant.md), so

$$
\boxed{[\lambda]=\det\bigl([\lambda_i+j-i]\bigr)_{1\le i,j\le l}.}
$$

This is the [character](../../../../../character-of-a-representation.md) version of the [Jacobi–Trudi identity](../../../../../jacobi-trudi-identity.md).

For the example the matrix is

$$
[3,2,2]=\det\begin{pmatrix}[3]&[4]&[5]\\{}[1]&[2]&[3]\\{}[0]&[1]&[2]\end{pmatrix}.
$$

Expanding gives the concise answer

$$
\boxed{[3,2,2]=[3][2]^2-[3]^2[1]-[4][1][2]+[4][3]+[5][1]^2-[5][2].}
$$

At the identity the six induction-product [dimensions](../../../../../dimension-vector-space.md) are $210,140,105,35,42,21$, respectively; their alternating sum is $21$, agreeing with the [hook-length formula](../../../../../hook-length-formula.md) for $(3,2,2)$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
