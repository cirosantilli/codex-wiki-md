<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We use $[a,b]=a^{-1}b^{-1}ab$. To obtain a [Wirtinger presentation](../../../../../wirtinger-presentation.md), choose an oriented regular [knot diagram](../../../../../knot-diagram.md), cut its strands at undercrossings, and give each resulting arc a positively oriented [meridian of a knot](../../../../../meridian-of-a-knot.md). The complement of the arcs above the projection plane has a free [fundamental group](../../../../../fundamental-group.md) on these meridians. At a crossing, pushing an understrand meridian past the overstrand conjugates it by the overstrand meridian. Thus, if $a$ is the overstrand generator and $b,c$ are the incoming and outgoing understrand generators, the relation is $c=a^{\epsilon}ba^{-\epsilon}$, where $\epsilon$ is determined by the crossing orientation. Applying the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) while adjoining the crossing neighborhoods gives one such relation per crossing. The remaining three-dimensional region adds no fundamental-group relation. For a connected diagram one crossing relation is redundant. This derives a [group presentation](../../../../../group-presentation.md) from any tame knot diagram, rather than just specifying a recipe without its topological justification.

For the [Borromean rings](../../../../../borromean-rings.md), choose three meridians $x,y,z$ and call the other three arc meridians $x',y',z'$. Base paths and orientations can be chosen so the six crossing relations read

$$
\begin{aligned}
x'&=zxz^{-1},&y'&=xyx^{-1},&z'&=yzy^{-1},\\
x'&=z'x(z')^{-1},&y'&=x'y(x')^{-1},&z'&=y'z(y')^{-1}.
\end{aligned}
$$

Eliminate the primed generators with the first row. The second row says respectively that $x$ commutes with $(z')^{-1}z=[y^{-1},z]$, that $y$ commutes with $(x')^{-1}x=[z^{-1},x]$, and that $z$ commutes with $(y')^{-1}y=[x^{-1},y]$. The last relation is redundant, just as one crossing relation is redundant in the [Wirtinger presentation](../../../../../wirtinger-presentation.md). Alternatively the [Hall-Witt identity](../../../../../hall-witt-identity.md), after conjugating its three factors, shows that any two of these cyclic relations imply the third. Hence the [Borromean link group](../../../../../borromean-link-group.md) is

$$
\boxed{G=\langle x,y,z\mid [x,[y^{-1},z]]=1,\ [y,[z^{-1},x]]=1\rangle.}
$$

Both relators have zero exponent sum in each generator. Passing from the free [group](../../../../../group-split.md) to its [abelianization](../../../../../abelianization.md) therefore imposes no relations beyond commutation, and

$$
\boxed{G/[G,G]\cong\mathbb Z^3.}
$$

Equivalently the three linking-number maps to $\mathbb Z$ independently detect the three meridians.

Here is an explicit representation, followed by a faithfulness argument:

$$
X=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad
Y=\begin{pmatrix}1&0\\2i&1\end{pmatrix},\qquad
Z=\begin{pmatrix}i&1\\2i&2-i\end{pmatrix},\qquad
\rho(x)=X,\quad\rho(y)=Y,\quad\rho(z)=Z.
$$

Each [determinant](../../../../../determinant.md) is one. Direct multiplication verifies the two relators. For example $[Y^{-1},Z]=\begin{pmatrix}-1&2i\\0&-1\end{pmatrix}$, which commutes with $X$. Merely checking those relators would not prove faithfulness, so we identify the image's complete [group presentation](../../../../../group-presentation.md).

Write $B=PSL_2(\mathbb Z[i])$, the [Gaussian Bianchi group](../../../../../gaussian-bianchi-group.md), and use its four generators $T,U,L,A$ from the allowed presentation. In $B$ the three proposed generators are

$$
X=T,\qquad Y=AU^{-2}A^{-1},\qquad Z=AT^{-2}A^{-1}LU^{-1}.
$$

The last equality is in $PSL_2$, so an overall minus sign in matrix multiplication is immaterial. Reduce matrices modulo $4$ in $\mathbb Z[i]$, and then quotient by $\{\pm I\}$. The finite image $Q$ has order $1536$: the residue field is $\mathbb F_2$, $SL_2(\mathbb F_2)$ has order six, and each of the three subsequent local-ring layers has a kernel of order $2^3$, before the final quotient by $\{\pm I\}$. Elementary elimination over this local ring shows that the images of $T,U,A$ generate it. The subgroup $\bar H=\langle\bar X,\bar Y,\bar Z\rangle$ has order $64$, as multiplication in this finite ring verifies. Let $K$ be its inverse image in $B$; then $[B:K]=24$.

For completeness the following gives the coset computation needed to check the subgroup presentation explicitly. Cosets are right cosets $K r$; columns record right multiplication by $T,U,L,A$. Representatives are words in the allowed generators.

$$
\begin{array}{c|c|rrrr}
j&r_j&T&U&L&A\\\hline
0&1&0&1&2&3\\
1&U&1&0&4&5\\
2&L&2&4&0&6\\
3&A&7&8&6&0\\
4&UL&4&2&1&9\\
5&UA&10&11&9&1\\
6&LA&12&13&3&2\\
7&AT&9&14&10&15\\
8&AU&14&3&13&16\\
9&ULA&15&16&5&4\\
10&UAT&6&17&7&12\\
11&UAU&17&5&16&13\\
12&LAT&5&18&15&10\\
13&LAU&18&6&8&11\\
14&ATU&16&7&17&19\\
15&ATA&3&20&12&7\\
16&AUA&20&9&11&8\\
17&UATU&13&10&14&21\\
18&LATU&11&12&20&22\\
19&ATUA&19&22&21&14\\
20&ATAU&8&15&18&23\\
21&UATUA&21&23&19&17\\
22&LATUA&22&19&23&18\\
23&ATAUA&23&21&22&20
\end{array}
$$

Apply the [Reidemeister–Schreier theorem](../../../../../reidemeister-schreier-theorem.md): for a transition $j\mathrel{\mathop{\longrightarrow}^{g}}k$, use generator $r_jg r_k^{-1}$, omitting the 23 tree transitions. Rewrite each of the eight allowed ambient relators starting at each of the 24 rows. There are 73 remaining Schreier generators. Adjoin the names $x=T$, $y=AU^{-2}A^{-1}$, $z=AT^{-2}A^{-1}LU^{-1}$ and eliminate the Schreier generators using relations in which they occur once. The remaining relations, with an uppercase letter denoting the inverse of the corresponding lowercase one, are the words

$$
\begin{aligned}
p&=ZYxyXzxYXy,\\
q&=ZYzXZxyXzx,\\
w&=ZxYXzXZxyXzxYxyX.
\end{aligned}
$$

This table and the rewriting rule determine every relation without an appeal to a guessed presentation. In this notation cyclically reduced versions of the two desired relators are $r=ZYzXZyzYxy$ and $q$. Elementary substitutions of relator segments, with cyclic reduction at each step, give

$$
p\ \longrightarrow\ r\ \longrightarrow\ 1,\qquad
w\ \longrightarrow\ ZYzXXZxyXzxYxy\ \longrightarrow\ q\ \longrightarrow\ 1
$$

using $r,q$; conversely $r\longrightarrow p\longrightarrow1$ using $p,q$. These substitutions show equality of the two normal closures. For example the first substitution replaces $xyX$ in the cyclic rotation of $p$ by $zxZyzXZ$, as allowed by $q$, and then the initial $ZYz$ is replaced by $YXyZYzx$ using $r$. Thus $K$ has exactly the presentation of $G$, with $x,y,z$ represented by $X,Y,Z$. In particular these three matrices generate $K$, and

$$
\boxed{\rho:G\hookrightarrow PSL_2(\mathbb C)\text{ is faithful and has discrete image of index }24\text{ in }B.}
$$

To identify the actual link complement as a [hyperbolic three-manifold](../../../../../hyperbolic-three-manifold.md), rather than only on a manifold with an isomorphic [group](../../../../../group-split.md), cut along the projection-plane regions, making the usual small crossing detours above and below. The octahedral projection graph has eight triangular regions. The upper and lower pieces are ideal octahedra; corresponding faces are matched with one-third-turn corner permutations, with opposite directions on adjacent checkerboard faces. Reversing these cuts reconstructs the link complement. Give both pieces the regular ideal [hyperbolic space](../../../../../hyperbolic-space.md) octahedron metric. All triangular face maps are [isometries](../../../../../isometry.md) and each edge cycle has four dihedral angles $\pi/2$, so the metric has no edge singularity. Equal horospherical truncations match in Euclidean squares and assemble into three flat [tori](../../../../../torus.md), giving complete [torus](../../../../../torus.md) cusps. The compact truncated remainder and these cusps show completeness and finite volume. Thus **the Borromean complement is a complete finite-volume hyperbolic three-manifold**. This also supplies a geometric discrete faithful holonomy, independently of the subgroup calculation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
