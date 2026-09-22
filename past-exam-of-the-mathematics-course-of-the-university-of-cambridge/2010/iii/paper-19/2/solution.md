<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Fix a bounded tile in [Euclidean space](../../../../../euclidean-norm.md) $\Omega$ with labelled flat boundary faces. For each face label $s$, encode an assembly of $n$ copies by an involutive real symmetric [signed permutation matrix](../../../../../signed-permutation-matrix.md) $M_s$: a paired interface contributes a two-by-two swap, an unglued face with a [Neumann boundary condition](../../../../../neumann-boundary-condition.md) contributes $+1$ on the diagonal, and an unglued face with a [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) contributes $-1$. Use the same face-identification convention on each copy. If a second assembly has matrices $N_s$ and there is an invertible constant matrix $C$ satisfying

$$
\boxed{CM_s=N_sC\quad\hbox{for every face label }s,}
$$

then the map $u=(u_1,\ldots,u_n)\mapsto Cu$ is an isomorphism between corresponding [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) [eigenspaces](../../../../../eigenspace.md). This is the [transplantation theorem](../../../../../transplantation-theorem.md).

To prove it, restrict an [eigenfunction](../../../../../eigenfunction.md) to the tile copies and identify each copy with $\Omega$. Along a face, let $a$ be its vector of boundary values and $b$ its vector of outward [normal derivatives](../../../../../normal-derivative.md). At a glued interface the values agree and the outward derivatives are opposite. At an unglued face with a [Neumann boundary condition](../../../../../neumann-boundary-condition.md) the derivative vanishes, and at a face with a [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) the value vanishes. All three cases are encoded by

$$
M_sa=a,\qquad M_sb=-b.
$$

The intertwining identities give $N_s(Ca)=Ca$ and $N_s(Cb)=-Cb$, so the transplanted function satisfies the second assembly's interface and [boundary conditions](../../../../../boundary-condition.md). On each tile its [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) is the same constant linear combination of the original Laplacians, hence it has the same [eigenvalue](../../../../../eigenvalue.md). Across an interface, matching values and opposite [normal derivatives](../../../../../normal-derivative.md) make it a weak solution; [elliptic regularity](../../../../../elliptic-regularity.md), or the allowed reflection principle, makes it a genuine smooth solution there. At corners the operator is understood by its finite-energy, [Friedrichs extension](../../../../../friedrichs-extension.md); the same matching argument applies to its [quadratic form](../../../../../quadratic-form.md) domain. Applying $C^{-1}$ reverses the construction. Thus dimensions of all [eigenspaces](../../../../../eigenspace.md) agree, including [multiplicities](../../../../../multiplicity-mathematics.md), and the two specified boundary-value spectra coincide.

**The requested pair exists with explicitly specified mixed boundary conditions and polygonal boundary.** Take four copies $Q_0,Q_1,Q_2,Q_3$ of an octagonal [regular polygon](../../../../../regular-polygon.md) in [Euclidean space](../../../../../euclidean-norm.md). Label four alternate sides $a,b,c,d$ in cyclic order; the four intervening sides always have a [Neumann boundary condition](../../../../../neumann-boundary-condition.md). The labelled sides are disjoint even at their endpoints. Parameterize every side in the positive boundary direction of the reference octagon. When pairing same-labelled sides, identify equal parameters. This produces a locally flat [surface with boundary](../../../../../surface-with-boundary.md): a neighbourhood of an interior point of an interface consists of two half-disks glued along their diameters. All tile vertices remain boundary points, with boundary angles $3\pi/4$ or $3\pi/2$; there are no interior cone points.

Here are the complete gluing and [boundary conditions](../../../../../boundary-condition.md). An entry $ij$ pairs the corresponding sides of $Q_i,Q_j$. The indicated unpaired sides have a [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md); every other unpaired side has a [Neumann boundary condition](../../../../../neumann-boundary-condition.md).

$$
\begin{array}{c|c|c|c|c}
\text{face}&\text{pairs in }D&\text{Dirichlet tiles in }D&\text{pairs in }B&\text{Dirichlet tiles in }B\\ \hline
a&23&\varnothing&13&\varnothing\\
b&12&\varnothing&12&\varnothing\\
c&01&\{2,3\}&02&\{1,3\}\\
d&\varnothing&\{1,3\}&01,\ 23&\varnothing
\end{array}
$$

Both assemblies are compact and connected. The [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) is the nonnegative operator $P=-\Delta$ associated with the finite-energy [quadratic form](../../../../../quadratic-form.md) $\int|\nabla u|^2$, with zero [Sobolev trace](../../../../../trace-operator.md) on the specified Dirichlet arcs. Thus the [mixed boundary condition](../../../../../mixed-boundary-condition.md) is defined without requiring classical differentiability at a corner or at a Dirichlet–Neumann junction.

The four [signed permutation matrices](../../../../../signed-permutation-matrix.md) for $D$ are

$$
M_a=\begin{pmatrix}1&0&0&0\\0&1&0&0\\0&0&0&1\\0&0&1&0\end{pmatrix},\quad
M_b=\begin{pmatrix}1&0&0&0\\0&0&1&0\\0&1&0&0\\0&0&0&1\end{pmatrix},\quad
M_c=\begin{pmatrix}0&1&0&0\\1&0&0&0\\0&0&-1&0\\0&0&0&-1\end{pmatrix},\quad
M_d=\operatorname{diag}(1,-1,1,-1).
$$

For $B$ they are

$$
N_a=\begin{pmatrix}1&0&0&0\\0&0&0&1\\0&0&1&0\\0&1&0&0\end{pmatrix},\quad
N_b=M_b,\quad
N_c=\begin{pmatrix}0&0&1&0\\0&-1&0&0\\1&0&0&0\\0&0&0&-1\end{pmatrix},\quad
N_d=\begin{pmatrix}0&1&0&0\\1&0&0&0\\0&0&0&1\\0&0&1&0\end{pmatrix}.
$$

Use the [Hadamard matrix](../../../../../hadamard-matrix.md)

$$
\boxed{C=\begin{pmatrix}1&1&1&1\\1&-1&1&-1\\1&1&-1&-1\\1&-1&-1&1\end{pmatrix},\qquad C^{-1}=\frac14C.}
$$

The intertwining relations can be checked on all columns at once. Writing the columns of $C$ as $h_0,h_1,h_2,h_3$, direct application of the displayed $N_s$ gives

$$
\begin{aligned}
N_aC&=(h_0,h_1,h_3,h_2)=CM_a,\\
N_bC&=(h_0,h_2,h_1,h_3)=CM_b,\\
N_cC&=(h_1,h_0,-h_2,-h_3)=CM_c,\\
N_dC&=(h_0,-h_1,h_2,-h_3)=CM_d.
\end{aligned}
$$

For the four intervening faces both assemblies have the identity face matrix, so these intertwining relations hold as well. Also $C^TC=C^2=4I$. This [four-tile mixed-boundary transplantation between a disk and a nonorientable surface](../../../../../four-tile-mixed-boundary-transplantation-between-a-disk-and-a-nonorientable-surface.md) gives a bijection of every pair of [eigenspaces](../../../../../eigenspace.md), preserving [eigenvalues](../../../../../eigenvalue.md) and [multiplicities](../../../../../multiplicity-mathematics.md).

There is also a direct argument on the [quadratic form](../../../../../quadratic-form.md) domains that handles all boundary corners. The [orthogonal matrix](../../../../../orthogonal-matrix.md) $U=C/2$ acts on tile restrictions, preserves their [L2 inner product](../../../../../l2-inner-product.md) and the sum of their [Dirichlet energies](../../../../../dirichlet-energy.md), and commutes with taking a [Sobolev trace](../../../../../trace-operator.md). The condition $M_su=u$ on each face encodes equality of the two traces at a paired interface and vanishing trace at an unpaired Dirichlet face. Intertwining takes these conditions exactly to $N_s(Uu)=Uu$. Consequently $U$ maps the whole form domain onto the other form domain and preserves its [quadratic form](../../../../../quadratic-form.md). The associated [self-adjoint operators](../../../../../self-adjoint-operator.md) are unitarily equivalent, proving isospectrality for the stated [mixed boundary conditions](../../../../../mixed-boundary-condition.md) without any assumption of smoothness at a Dirichlet–Neumann junction.

We now verify the actual topology using the [topology of disk tiles glued along disjoint boundary arcs](../../../../../topology-of-disk-tiles-glued-along-disjoint-boundary-arcs.md). Because the gluing arcs in each tile are disjoint, the resulting [surface with boundary](../../../../../surface-with-boundary.md) is a thickening of its gluing [graph](../../../../../graph-split.md), with one vertex for each [closed disc](../../../../../closed-disc.md) tile and one edge for each paired arc. One can construct this [homotopy equivalence](../../../../../homotopy-equivalence.md) by taking a small central [closed disc](../../../../../closed-disc.md) in each tile and narrow strips to its paired arcs. What remains is a [collar neighbourhood](../../../../../collar-neighbourhood.md) of the boundary, which retracts onto this connected system of [closed discs](../../../../../closed-disc.md) and strips. Shrinking each central [closed disc](../../../../../closed-disc.md) and each strip then gives the gluing [graph](../../../../../graph-split.md). Equivalently, begin with a [spanning tree](../../../../../spanning-tree.md) of the gluing [graph](../../../../../graph-split.md): its [closed disc](../../../../../closed-disc.md) tiles joined along boundary arcs form one [closed disc](../../../../../closed-disc.md), and every remaining pair of boundary arcs adds one band. Thus for $n$ tiles and $e$ paired arcs the [fundamental group](../../../../../fundamental-group.md) is a [free group](../../../../../free-group.md) of rank $e-n+1$, and the [Euler characteristic](../../../../../euler-characteristic.md) is $n-e$.

For $D$, the gluing [graph](../../../../../graph-split.md) is the path

$$
0\xrightarrow{c}1\xrightarrow{b}2\xrightarrow{a}3.
$$

Gluing a new [closed disc](../../../../../closed-disc.md) to a [closed disc](../../../../../closed-disc.md) along one boundary arc again gives a [closed disc](../../../../../closed-disc.md); applying this three times proves that $D$ is homeomorphic to a [closed disc](../../../../../closed-disc.md). In particular

$$
\boxed{D\text{ is orientable and simply connected},\qquad\chi(D)=1,\qquad\pi_1(D)=\{1\}.}
$$

For $B$, the five paired arcs give the [graph](../../../../../graph-split.md) edges $13,12,02,01,23$. It is connected, and hence

$$
\boxed{\chi(B)=4-5=-1,\qquad\pi_1(B)\cong F_2.}
$$

Here $F_2$ is the [free group](../../../../../free-group.md) on two generators, so $B$ is not [simply connected](../../../../../simply-connected-space.md). To decide [orientation of a surface](../../../../../orientation-of-a-surface.md), give every reference tile its counterclockwise [orientation](../../../../../orientation-of-a-simplex.md). Our same-parameter gluing preserves boundary directions, so a global [orientation](../../../../../orientation-of-a-simplex.md) requires opposite orientation signs on paired tiles: the two induced boundary orientations at an interior interface must be opposite. Such signs exist exactly when the gluing [graph](../../../../../graph-split.md) is [bipartite](../../../../../bipartite-graph.md). In $B$ the cycle

$$
1\xrightarrow{b}2\xrightarrow{d}3\xrightarrow{a}1
$$

has length three. Following it forces the sign to reverse three times and return to its starting tile with the opposite sign. This proves that $B$ is a [nonorientable surface](../../../../../non-orientable-surface.md). It has nonempty boundary because every intervening octagon side remains unpaired. Thus **$D$ is a simply-connected orientable surface with boundary, whereas its isospectral partner $B$ is neither simply connected nor orientable**, exactly as required, for the specified mixed boundary problem.

The boundary qualification is essential. With smooth boundary and the same pure [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) or pure [Neumann boundary condition](../../../../../neumann-boundary-condition.md) on both surfaces, the following existing obstruction applies. Polygonal corners and the [mixed boundary conditions](../../../../../mixed-boundary-condition.md) in the construction above place it outside that obstruction.

With the interpretation of compact smooth [Riemannian surfaces](../../../../../riemannian-surface.md) with the same pure [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) or pure [Neumann boundary condition](../../../../../neumann-boundary-condition.md), the printed simply-connected/nonorientable pair cannot exist. The two-dimensional [heat trace](../../../../../heat-trace.md) has the following expansion (the smooth-boundary coefficients are given in [the heat-coefficient formulas, Theorems 5.1–5.2](https://pages.uoregon.edu/gilkey/dirPDF/E27Handbook.pdf)):

$$
\operatorname{Tr}(e^{-tP})
=\frac{A}{4\pi t}\mp\frac{L}{8\sqrt{\pi t}}
+\frac1{12\pi}\left(\int_M K\,dA+\int_{\partial M}\kappa\,ds\right)+O(t^{1/2}),
$$

where the boundary sign is minus for Dirichlet and plus for Neumann. The [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) identifies the constant term with $\chi(M)/6$. Isospectrality therefore forces equal [Euler characteristics](../../../../../euler-characteristic.md). A compact connected simply-connected surface with boundary is a disk and has $\chi=1$. A connected nonorientable surface with $c\geq1$ crosscaps and $b\geq1$ boundary components has $\chi=2-c-b\leq0$. Thus **no such smooth pure-Dirichlet or pure-Neumann pair exists**. This is the [Euler characteristic from the heat trace of a bordered surface](../../../../../euler-characteristic-from-the-heat-trace-of-a-bordered-surface.md).

Piecewise-smooth boundaries introduce corner terms, and mixed [boundary conditions](../../../../../boundary-condition.md) change the heat coefficients, as the explicit construction above demonstrates. Moreover, in the usual pure-Neumann polygonal reflection-transplantation setup, the [pure Neumann reflection transplantation preserves Euler characteristic](../../../../../pure-neumann-reflection-transplantation-preserves-euler-characteristic.md) argument applies even with corners. The numbers of tiles agree. For each face label the number of edge classes is $(n+\operatorname{tr}M_s)/2$, so these agree too. For each tile-vertex label, vertex classes are orbits of the [subgroup](../../../../../subgroup.md) generated by incident-face involutions. Their number is the [dimension](../../../../../dimension-vector-space.md) of invariant vectors in that permutation representation, which is unchanged by the intertwiner. Hence the numbers of vertices agree, proving equal $V-E+F$. Thus this standard tiled construction also cannot supply a disk on one side and a nonorientable surface on the other.

For comparison, the following existing construction gives an [orientable](../../../../../orientable-surface.md) and a nonorientable pair with the same [spectrum](../../../../../spectrum-functional-analysis.md) for the pure [Neumann boundary condition](../../../../../neumann-boundary-condition.md). Both have nontrivial [fundamental groups](../../../../../fundamental-group.md); this is a separate example, not the construction used to meet the simply-connected requirement above. This [eight-tile Neumann transplantation across orientability](../../../../../eight-tile-neumann-transplantation-across-orientability.md) makes the comparison explicit. The finite seed is the affine modulo-eight example in [the original orientability construction](https://arxiv.org/pdf/2008.12498); the intertwiner and the topology checks are derived below. Take eight copies of a regular Euclidean hexagon and label three pairwise nonadjacent sides $\sigma,t,u$. Every remaining side is a side with a [Neumann boundary condition](../../../../../neumann-boundary-condition.md). Index the copies by $j\in\mathbb Z/8\mathbb Z$. For the first assembly pair same-labelled faces according to

$$
\sigma(j)=1-j,\qquad t(j)=-j,\qquad u_1(j)=3j;
$$

for the second, use

$$
\sigma(j)=1-j,\qquad t(j)=-j,\qquad u_2(j)=3j+4,
$$

with all arithmetic modulo eight. A fixed point means an unglued side with a [Neumann boundary condition](../../../../../neumann-boundary-condition.md). Pair faces by the reflection convention, matching the same endpoint parameter in the reference tiles. The distinguished sides are disjoint, so no interior vertex singularities are created; the resulting surfaces have polygonal boundary corners.

Let $R e_j=e_{j+1}$ on the eight-dimensional tile-index space and set

$$
\boxed{C=I+R^4+2(R+R^{-1}).}
$$

It commutes with the [permutation matrices](../../../../../permutation-matrix.md) for $t$ and $\sigma$, because its coefficients are invariant under reversing cyclic order. For $u_1,u_2$, write $C_{ij}=c_{i-j}$, where $c_0=c_4=1$, $c_1=c_7=2$, and all other $c_r$ vanish. The required relation $CM_{u_1}=M_{u_2}C$ is exactly $c_r=c_{3r+4}$, verified from these four nonzero entries. Thus all three intertwining relations hold.

The cyclic Fourier vectors diagonalize $C$. Its [eigenvalues](../../../../../eigenvalue.md) are

$$
1+(-1)^k+4\cos(\pi k/4),\qquad0\leq k\leq7,
$$

namely $6,2\sqrt2,2,-2\sqrt2,-2,-2\sqrt2,2,2\sqrt2$. None is zero, so $C$ is invertible and the two assemblies are [isospectral manifolds](../../../../../isospectral-manifolds.md) for the [Neumann boundary condition](../../../../../neumann-boundary-condition.md).

We prove their topology as well. Their gluing graphs are connected: the first contains the spanning path $0,1,3,6,2,7,5,4$, and the second contains the spanning cycle $0,1,7,2,6,3,5,4,0$. Each has eight tile vertices and ten paired-face edges. Since tiles are disks and gluing arcs are disjoint, each surface retracts up to [homotopy](../../../../../homotopy.md) to this multigraph; thus its [Euler characteristic](../../../../../euler-characteristic.md) is $8-10=-2$ and its [fundamental group](../../../../../fundamental-group.md) is a [free group](../../../../../free-group.md) of rank three.

An [orientation](../../../../../orientation-of-a-simplex.md) assigns a sign to each reference tile, and a reflection gluing requires opposite signs at the ends of every graph edge. The second graph admits this assignment: take sign $+$ on $\{0,5,6,7\}$ and sign $-$ on $\{1,2,3,4\}$. Every paired face joins opposite signs, proving orientability. In the first graph the cycle

$$
1\xrightarrow{u_1}3\xrightarrow{\sigma}6\xrightarrow{t}2
\xrightarrow{\sigma}7\xrightarrow{t}1
$$

has odd length. Transporting [orientation](../../../../../orientation-of-a-simplex.md) around it reverses the initial sign, proving nonorientability. Hence the first surface is also not [simply connected](../../../../../simply-connected-space.md). The second surface is [orientable](../../../../../orientable-surface.md) but likewise not [simply connected](../../../../../simply-connected-space.md); the disk required in the question is supplied instead by the four-tile mixed-boundary construction above.

The four-tile construction resolves the printed simply-connected requirement under explicit [mixed boundary conditions](../../../../../mixed-boundary-condition.md). The eight-tile comparison only concerns [orientation of a surface](../../../../../orientation-of-a-surface.md) under a pure [Neumann boundary condition](../../../../../neumann-boundary-condition.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
