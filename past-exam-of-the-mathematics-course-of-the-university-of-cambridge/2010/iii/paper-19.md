# Paper 19

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper19.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper19.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
  - [1](#5/1)
    - [Solution](#5/1/solution)
  - [2](#5/2)
    - [Solution](#5/2/solution)
  - [3](#5/3)
    - [Solution](#5/3/solution)

## 1

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

We use $\Delta=\operatorname{div}\nabla$, whose [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) on a [compact manifold](../../../differential-geometry.md#compact-manifold) is nonpositive; write $P=-\Delta$ for the [positive Laplace-Beltrami operator](../../../differential-geometry.md#positive-laplace-beltrami-operator). This convention will also make the [heat operator](../../../diffusion-equation.md#heat-operator) in Question 3 equal to $\partial_t-\Delta$.

Let $e_1,\ldots,e_d$ be an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $T_pM$, and let $\gamma_i$ be the unit-speed [geodesic](../../../riemannian-geometry.md#geodesic) with $\gamma_i(0)=p$ and $\dot\gamma_i(0)=e_i$. Since a [geodesic](../../../riemannian-geometry.md#geodesic) has vanishing acceleration for the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection), differentiation twice along it gives the [Riemannian Hessian](../../../riemannian-geometry.md#riemannian-hessian):

$$
\left.\frac{d^2}{dt^2}f(\gamma_i(t))\right|_{t=0}
=\operatorname{Hess}_g f(e_i,e_i).
$$

Taking its [metric trace](../../../linear-algebra.md#metric-trace) yields the [geodesic trace formula for the Laplace-Beltrami operator](../../../differential-geometry.md#geodesic-trace-formula-for-the-laplace-beltrami-operator)

$$
\boxed{\Delta f(p)=\sum_{i=1}^d\left.\frac{d^2}{dt^2}f(\gamma_i(t))\right|_{t=0}.}
$$

The positive-sign convention $P$ puts a minus sign in front of this sum.

For the unit [sphere](../../../geometry-and-topology.md#sphere), take $p\in S^d$ and tangent unit vectors $e_i$ orthogonal to $p$. Its [great circle](../../../geometry-and-topology.md#great-circle) [geodesics](../../../riemannian-geometry.md#geodesic) are $\gamma_i(t)=p\cos t+e_i\sin t$. For a smooth ambient function $F$ near the [sphere](../../../geometry-and-topology.md#sphere), the ordinary [chain rule](../../../calculus.md#chain-rule) gives

$$
\left.\frac{d^2}{dt^2}F(\gamma_i(t))\right|_0
=D^2F_p(e_i,e_i)-DF_p(p).
$$

The ambient [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) is $e_1,\ldots,e_d,p$. Thus, writing $F_r(p)=\partial_rF(rp)|_{r=1}$ and similarly for $F_{rr}$,

$$
\boxed{\Delta_{S^d}(F|_{S^d})
=(\widetilde\Delta F)|_{S^d}-F_{rr}|_{r=1}-dF_r|_{r=1}.}
$$

This proves the [ambient restriction formula for the spherical Laplacian](../../../riemannian-geometry.md#ambient-restriction-formula-for-the-spherical-laplacian) and shows why ambient derivatives normal to the [sphere](../../../geometry-and-topology.md#sphere) must be subtracted. The equivalent formula in [spherical coordinates](../../../calculus.md#spherical-coordinate-system) is

$$
\widetilde\Delta F=F_{rr}+\frac d rF_r+\frac1{r^2}\Delta_{S^d}(F(r,\cdot)).
$$

Let $\mathcal P_\ell$ be the [vector space](../../../vector-space.md) of [homogeneous polynomials](../../../algebra.md#homogeneous-polynomial) of degree $\ell$ in $d+1$ variables, and $\mathcal H_\ell=\ker\widetilde\Delta\cap\mathcal P_\ell$ its [harmonic polynomials](../../../partial-differential-equation.md#harmonic-polynomial). If $H\in\mathcal H_\ell$, [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) scaling gives $H(r\omega)=r^\ell H(\omega)$. Substitution into the [spherical coordinates](../../../calculus.md#spherical-coordinate-system) formula gives

$$
\boxed{P_{S^d}(H|_{S^d})=\ell(\ell+d-1)H|_{S^d}.}
$$

The restrictions are the degree-$\ell$ [spherical harmonics](../../../analysis.md#spherical-harmonic). A [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) vanishing on the [sphere](../../../geometry-and-topology.md#sphere) vanishes on every nonzero ray and hence identically, so restriction is injective on $\mathcal H_\ell$.

We prove the [harmonic decomposition of homogeneous polynomials](../../../partial-differential-equation.md#harmonic-decomposition-of-homogeneous-polynomials) that both counts these [eigenfunctions](../../../linear-operator-theory.md#eigenfunction) and establishes completeness. For an ambient harmonic [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) $H_m$ of degree $m$ and $j\geq1$, the [spherical coordinates](../../../calculus.md#spherical-coordinate-system) formula gives

$$
\widetilde\Delta(r^{2j}H_m)
=2j(2m+2j+d-1)r^{2j-2}H_m.
$$

For $d\geq1$ its coefficient is nonzero. Inductively assume [homogeneous polynomials](../../../algebra.md#homogeneous-polynomial) of degree $\ell-2$ have been decomposed into sums of $r^{2j}H_m$. Apply this decomposition to $\widetilde\Delta Q$ for $Q\in\mathcal P_\ell$, and lift each summand by multiplying by $r^2$ and dividing by the displayed nonzero coefficient. The resulting $R\in r^2\mathcal P_{\ell-2}$ satisfies $\widetilde\Delta R=\widetilde\Delta Q$, so $Q-R\in\mathcal H_\ell$. The same coefficient formula shows that no nonzero element of $r^2\mathcal P_{\ell-2}$ can be harmonic. Starting at degrees zero and one therefore proves the direct decomposition

$$
\mathcal P_\ell=\mathcal H_\ell\oplus r^2\mathcal P_{\ell-2}.
$$

Since $\dim\mathcal P_\ell=\binom{\ell+d}{d}$, the [multiplicity](../../../polynomial.md#multiplicity-mathematics) is

$$
\boxed{m_\ell=\binom{\ell+d}{d}-\binom{\ell+d-2}{d},}
$$

where the second term is zero for $\ell<2$.

On $r=1$, iterating the decomposition writes every [polynomial](../../../polynomial.md) restriction as a finite sum of [spherical harmonics](../../../analysis.md#spherical-harmonic). The [Stone-Weierstrass theorem](../../../functional-analysis.md#stone-weierstrass-theorem) makes these [polynomial](../../../polynomial.md) restrictions dense in $C(S^d)$, since coordinate functions separate points and constants are included; they are consequently dense in $L^2(S^d)$. [Integration by parts](../../../calculus.md#integration-by-parts) makes $P$ symmetric on smooth functions and gives orthogonality between distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue). Normalizing within each finite-dimensional [eigenspace](../../../linear-operator-theory.md#eigenspace) gives a complete [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis) $Y_{\ell a}$. To check the full operator [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis), let $c_{\ell a}=\langle f,Y_{\ell a}\rangle$. For smooth $f$, [integration by parts](../../../calculus.md#integration-by-parts) gives the coefficients of $Pf$ as $\lambda_\ell c_{\ell a}$. Therefore finite harmonic partial sums approximate both $f$ and $Pf$ in $L^2$, hence approximate in the [graph norm](../../../functional-analysis.md#graph-norm). Conversely every coefficient sequence with $\sum_{\ell,a}\lambda_\ell^2|c_{\ell a}|^2<\infty$ is the [graph norm](../../../functional-analysis.md#graph-norm) limit of its finite harmonic sums. Thus the closure of $P$ has exactly this [operator domain](../../../vector-space.md#operator-domain) and is the real diagonal [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) with entries $\lambda_\ell=\ell(\ell+d-1)$. If $z$ is not one of these entries, the inverse has entries $(\lambda_\ell-z)^{-1}$ and is bounded because $\lambda_\ell\to\infty$. This proves that there are no missing spectral values. The [spectrum of the Laplacian on a sphere](../../../riemannian-geometry.md#spectrum-of-the-laplacian-on-a-sphere) is

$$
\boxed{\sigma(P)=\{\ell(\ell+d-1):\ell=0,1,2,\ldots\},}
$$

with the above [multiplicities](../../../polynomial.md#multiplicity-mathematics); for $\Delta$, negate every [eigenvalue](../../../linear-operator-theory.md#eigenvalue). For example $S^1$ has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\ell^2$, with [multiplicities](../../../polynomial.md#multiplicity-mathematics) one at zero and two for $\ell\geq1$, and $S^2$ has [multiplicity](../../../polynomial.md#multiplicity-mathematics) $2\ell+1$. The zero-dimensional sphere consists of two isolated points and has only the zero [eigenvalue](../../../linear-operator-theory.md#eigenvalue), with [multiplicity](../../../polynomial.md#multiplicity-mathematics) two.

## 2

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Fix a bounded tile in [Euclidean space](../../../functional-analysis.md#euclidean-norm) $\Omega$ with labelled flat boundary faces. For each face label $s$, encode an assembly of $n$ copies by an involutive real symmetric [signed permutation matrix](../../../vector-space.md#signed-permutation-matrix) $M_s$: a paired interface contributes a two-by-two swap, an unglued face with a [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) contributes $+1$ on the diagonal, and an unglued face with a [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) contributes $-1$. Use the same face-identification convention on each copy. If a second assembly has matrices $N_s$ and there is an invertible constant matrix $C$ satisfying

$$
\boxed{CM_s=N_sC\quad\hbox{for every face label }s,}
$$

then the map $u=(u_1,\ldots,u_n)\mapsto Cu$ is an isomorphism between corresponding [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator) [eigenspaces](../../../linear-operator-theory.md#eigenspace). This is the [transplantation theorem](../../../riemannian-geometry.md#transplantation-theorem).

To prove it, restrict an [eigenfunction](../../../linear-operator-theory.md#eigenfunction) to the tile copies and identify each copy with $\Omega$. Along a face, let $a$ be its vector of boundary values and $b$ its vector of outward [normal derivatives](../../../differential-geometry.md#normal-derivative). At a glued interface the values agree and the outward derivatives are opposite. At an unglued face with a [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) the derivative vanishes, and at a face with a [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) the value vanishes. All three cases are encoded by

$$
M_sa=a,\qquad M_sb=-b.
$$

The intertwining identities give $N_s(Ca)=Ca$ and $N_s(Cb)=-Cb$, so the transplanted function satisfies the second assembly's interface and [boundary conditions](../../../differential-equation.md#boundary-condition). On each tile its [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator) is the same constant linear combination of the original Laplacians, hence it has the same [eigenvalue](../../../linear-operator-theory.md#eigenvalue). Across an interface, matching values and opposite [normal derivatives](../../../differential-geometry.md#normal-derivative) make it a weak solution; [elliptic regularity](../../../distribution-theory.md#elliptic-regularity), or the allowed reflection principle, makes it a genuine smooth solution there. At corners the operator is understood by its finite-energy, [Friedrichs extension](../../../linear-operator-theory.md#friedrichs-extension); the same matching argument applies to its [quadratic form](../../../linear-algebra.md#quadratic-form) domain. Applying $C^{-1}$ reverses the construction. Thus dimensions of all [eigenspaces](../../../linear-operator-theory.md#eigenspace) agree, including [multiplicities](../../../polynomial.md#multiplicity-mathematics), and the two specified boundary-value spectra coincide.

**The requested pair exists with explicitly specified mixed boundary conditions and polygonal boundary.** Take four copies $Q_0,Q_1,Q_2,Q_3$ of an octagonal [regular polygon](../../../geometry-and-topology.md#regular-polygon) in [Euclidean space](../../../functional-analysis.md#euclidean-norm). Label four alternate sides $a,b,c,d$ in cyclic order; the four intervening sides always have a [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition). The labelled sides are disjoint even at their endpoints. Parameterize every side in the positive boundary direction of the reference octagon. When pairing same-labelled sides, identify equal parameters. This produces a locally flat [surface with boundary](../../../topology.md#surface-with-boundary): a neighbourhood of an interior point of an interface consists of two half-disks glued along their diameters. All tile vertices remain boundary points, with boundary angles $3\pi/4$ or $3\pi/2$; there are no interior cone points.

Here are the complete gluing and [boundary conditions](../../../differential-equation.md#boundary-condition). An entry $ij$ pairs the corresponding sides of $Q_i,Q_j$. The indicated unpaired sides have a [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition); every other unpaired side has a [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition).

$$
\begin{array}{c|c|c|c|c}
\text{face}&\text{pairs in }D&\text{Dirichlet tiles in }D&\text{pairs in }B&\text{Dirichlet tiles in }B\\ \hline
a&23&\varnothing&13&\varnothing\\
b&12&\varnothing&12&\varnothing\\
c&01&\{2,3\}&02&\{1,3\}\\
d&\varnothing&\{1,3\}&01,\ 23&\varnothing
\end{array}
$$

Both assemblies are compact and connected. The [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator) is the nonnegative operator $P=-\Delta$ associated with the finite-energy [quadratic form](../../../linear-algebra.md#quadratic-form) $\int|\nabla u|^2$, with zero [Sobolev trace](../../../sobolev-space.md#trace-operator) on the specified Dirichlet arcs. Thus the [mixed boundary condition](../../../differential-equation.md#mixed-boundary-condition) is defined without requiring classical differentiability at a corner or at a Dirichlet–Neumann junction.

The four [signed permutation matrices](../../../vector-space.md#signed-permutation-matrix) for $D$ are

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

Use the [Hadamard matrix](../../../vector-space.md#hadamard-matrix)

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

For the four intervening faces both assemblies have the identity face matrix, so these intertwining relations hold as well. Also $C^TC=C^2=4I$. This [four-tile mixed-boundary transplantation between a disk and a nonorientable surface](../../../riemannian-geometry.md#four-tile-mixed-boundary-transplantation-between-a-disk-and-a-nonorientable-surface) gives a bijection of every pair of [eigenspaces](../../../linear-operator-theory.md#eigenspace), preserving [eigenvalues](../../../linear-operator-theory.md#eigenvalue) and [multiplicities](../../../polynomial.md#multiplicity-mathematics).

There is also a direct argument on the [quadratic form](../../../linear-algebra.md#quadratic-form) domains that handles all boundary corners. The [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) $U=C/2$ acts on tile restrictions, preserves their [L2 inner product](../../../measure-theory.md#l2-inner-product) and the sum of their [Dirichlet energies](../../../differential-geometry.md#dirichlet-energy), and commutes with taking a [Sobolev trace](../../../sobolev-space.md#trace-operator). The condition $M_su=u$ on each face encodes equality of the two traces at a paired interface and vanishing trace at an unpaired Dirichlet face. Intertwining takes these conditions exactly to $N_s(Uu)=Uu$. Consequently $U$ maps the whole form domain onto the other form domain and preserves its [quadratic form](../../../linear-algebra.md#quadratic-form). The associated [self-adjoint operators](../../../linear-operator-theory.md#self-adjoint-operator) are unitarily equivalent, proving isospectrality for the stated [mixed boundary conditions](../../../differential-equation.md#mixed-boundary-condition) without any assumption of smoothness at a Dirichlet–Neumann junction.

We now verify the actual topology using the [topology of disk tiles glued along disjoint boundary arcs](../../../topology.md#topology-of-disk-tiles-glued-along-disjoint-boundary-arcs). Because the gluing arcs in each tile are disjoint, the resulting [surface with boundary](../../../topology.md#surface-with-boundary) is a thickening of its gluing [graph](../../../graph.md), with one vertex for each [closed disc](../../../topology.md#closed-disc) tile and one edge for each paired arc. One can construct this [homotopy equivalence](../../../algebraic-topology.md#homotopy-equivalence) by taking a small central [closed disc](../../../topology.md#closed-disc) in each tile and narrow strips to its paired arcs. What remains is a [collar neighbourhood](../../../differential-geometry.md#collar-neighbourhood) of the boundary, which retracts onto this connected system of [closed discs](../../../topology.md#closed-disc) and strips. Shrinking each central [closed disc](../../../topology.md#closed-disc) and each strip then gives the gluing [graph](../../../graph.md). Equivalently, begin with a [spanning tree](../../../combinatorics.md#spanning-tree) of the gluing [graph](../../../graph.md): its [closed disc](../../../topology.md#closed-disc) tiles joined along boundary arcs form one [closed disc](../../../topology.md#closed-disc), and every remaining pair of boundary arcs adds one band. Thus for $n$ tiles and $e$ paired arcs the [fundamental group](../../../algebraic-topology.md#fundamental-group) is a [free group](../../../geometric-group-theory.md#free-group) of rank $e-n+1$, and the [Euler characteristic](../../../homology.md#euler-characteristic) is $n-e$.

For $D$, the gluing [graph](../../../graph.md) is the path

$$
0\xrightarrow{c}1\xrightarrow{b}2\xrightarrow{a}3.
$$

Gluing a new [closed disc](../../../topology.md#closed-disc) to a [closed disc](../../../topology.md#closed-disc) along one boundary arc again gives a [closed disc](../../../topology.md#closed-disc); applying this three times proves that $D$ is homeomorphic to a [closed disc](../../../topology.md#closed-disc). In particular

$$
\boxed{D\text{ is orientable and simply connected},\qquad\chi(D)=1,\qquad\pi_1(D)=\{1\}.}
$$

For $B$, the five paired arcs give the [graph](../../../graph.md) edges $13,12,02,01,23$. It is connected, and hence

$$
\boxed{\chi(B)=4-5=-1,\qquad\pi_1(B)\cong F_2.}
$$

Here $F_2$ is the [free group](../../../geometric-group-theory.md#free-group) on two generators, so $B$ is not [simply connected](../../../algebraic-topology.md#simply-connected-space). To decide [orientation of a surface](../../../differential-geometry.md#orientation-of-a-surface), give every reference tile its counterclockwise [orientation](../../../algebraic-topology.md#orientation-of-a-simplex). Our same-parameter gluing preserves boundary directions, so a global [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) requires opposite orientation signs on paired tiles: the two induced boundary orientations at an interior interface must be opposite. Such signs exist exactly when the gluing [graph](../../../graph.md) is [bipartite](../../../graph-theory.md#bipartite-graph). In $B$ the cycle

$$
1\xrightarrow{b}2\xrightarrow{d}3\xrightarrow{a}1
$$

has length three. Following it forces the sign to reverse three times and return to its starting tile with the opposite sign. This proves that $B$ is a [nonorientable surface](../../../topology.md#non-orientable-surface). It has nonempty boundary because every intervening octagon side remains unpaired. Thus **$D$ is a simply-connected orientable surface with boundary, whereas its isospectral partner $B$ is neither simply connected nor orientable**, exactly as required, for the specified mixed boundary problem.

The boundary qualification is essential. With smooth boundary and the same pure [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) or pure [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) on both surfaces, the following existing obstruction applies. Polygonal corners and the [mixed boundary conditions](../../../differential-equation.md#mixed-boundary-condition) in the construction above place it outside that obstruction.

With the interpretation of compact smooth [Riemannian surfaces](../../../riemannian-geometry.md#riemannian-surface) with the same pure [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) or pure [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition), the printed simply-connected/nonorientable pair cannot exist. The two-dimensional [heat trace](../../../riemannian-geometry.md#heat-trace) has the following expansion (the smooth-boundary coefficients are given in [the heat-coefficient formulas, Theorems 5.1–5.2](https://pages.uoregon.edu/gilkey/dirPDF/E27Handbook.pdf)):

$$
\operatorname{Tr}(e^{-tP})
=\frac{A}{4\pi t}\mp\frac{L}{8\sqrt{\pi t}}
+\frac1{12\pi}\left(\int_M K\,dA+\int_{\partial M}\kappa\,ds\right)+O(t^{1/2}),
$$

where the boundary sign is minus for Dirichlet and plus for Neumann. The [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) identifies the constant term with $\chi(M)/6$. Isospectrality therefore forces equal [Euler characteristics](../../../homology.md#euler-characteristic). A compact connected simply-connected surface with boundary is a disk and has $\chi=1$. A connected nonorientable surface with $c\geq1$ crosscaps and $b\geq1$ boundary components has $\chi=2-c-b\leq0$. Thus **no such smooth pure-Dirichlet or pure-Neumann pair exists**. This is the [Euler characteristic from the heat trace of a bordered surface](../../../riemannian-geometry.md#euler-characteristic-from-the-heat-trace-of-a-bordered-surface).

Piecewise-smooth boundaries introduce corner terms, and mixed [boundary conditions](../../../differential-equation.md#boundary-condition) change the heat coefficients, as the explicit construction above demonstrates. Moreover, in the usual pure-Neumann polygonal reflection-transplantation setup, the [pure Neumann reflection transplantation preserves Euler characteristic](../../../riemannian-geometry.md#pure-neumann-reflection-transplantation-preserves-euler-characteristic) argument applies even with corners. The numbers of tiles agree. For each face label the number of edge classes is $(n+\operatorname{tr}M_s)/2$, so these agree too. For each tile-vertex label, vertex classes are orbits of the [subgroup](../../../group.md#subgroup) generated by incident-face involutions. Their number is the [dimension](../../../vector-space.md#dimension-vector-space) of invariant vectors in that permutation representation, which is unchanged by the intertwiner. Hence the numbers of vertices agree, proving equal $V-E+F$. Thus this standard tiled construction also cannot supply a disk on one side and a nonorientable surface on the other.

For comparison, the following existing construction gives an [orientable](../../../differential-geometry.md#orientable-surface) and a nonorientable pair with the same [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) for the pure [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition). Both have nontrivial [fundamental groups](../../../algebraic-topology.md#fundamental-group); this is a separate example, not the construction used to meet the simply-connected requirement above. This [eight-tile Neumann transplantation across orientability](../../../riemannian-geometry.md#eight-tile-neumann-transplantation-across-orientability) makes the comparison explicit. The finite seed is the affine modulo-eight example in [the original orientability construction](https://arxiv.org/pdf/2008.12498); the intertwiner and the topology checks are derived below. Take eight copies of a regular Euclidean hexagon and label three pairwise nonadjacent sides $\sigma,t,u$. Every remaining side is a side with a [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition). Index the copies by $j\in\mathbb Z/8\mathbb Z$. For the first assembly pair same-labelled faces according to

$$
\sigma(j)=1-j,\qquad t(j)=-j,\qquad u_1(j)=3j;
$$

for the second, use

$$
\sigma(j)=1-j,\qquad t(j)=-j,\qquad u_2(j)=3j+4,
$$

with all arithmetic modulo eight. A fixed point means an unglued side with a [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition). Pair faces by the reflection convention, matching the same endpoint parameter in the reference tiles. The distinguished sides are disjoint, so no interior vertex singularities are created; the resulting surfaces have polygonal boundary corners.

Let $R e_j=e_{j+1}$ on the eight-dimensional tile-index space and set

$$
\boxed{C=I+R^4+2(R+R^{-1}).}
$$

It commutes with the [permutation matrices](../../../vector-space.md#permutation-matrix) for $t$ and $\sigma$, because its coefficients are invariant under reversing cyclic order. For $u_1,u_2$, write $C_{ij}=c_{i-j}$, where $c_0=c_4=1$, $c_1=c_7=2$, and all other $c_r$ vanish. The required relation $CM_{u_1}=M_{u_2}C$ is exactly $c_r=c_{3r+4}$, verified from these four nonzero entries. Thus all three intertwining relations hold.

The cyclic Fourier vectors diagonalize $C$. Its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are

$$
1+(-1)^k+4\cos(\pi k/4),\qquad0\leq k\leq7,
$$

namely $6,2\sqrt2,2,-2\sqrt2,-2,-2\sqrt2,2,2\sqrt2$. None is zero, so $C$ is invertible and the two assemblies are [isospectral manifolds](../../../riemannian-geometry.md#isospectral-manifolds) for the [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition).

We prove their topology as well. Their gluing graphs are connected: the first contains the spanning path $0,1,3,6,2,7,5,4$, and the second contains the spanning cycle $0,1,7,2,6,3,5,4,0$. Each has eight tile vertices and ten paired-face edges. Since tiles are disks and gluing arcs are disjoint, each surface retracts up to [homotopy](../../../algebraic-topology.md#homotopy) to this multigraph; thus its [Euler characteristic](../../../homology.md#euler-characteristic) is $8-10=-2$ and its [fundamental group](../../../algebraic-topology.md#fundamental-group) is a [free group](../../../geometric-group-theory.md#free-group) of rank three.

An [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) assigns a sign to each reference tile, and a reflection gluing requires opposite signs at the ends of every graph edge. The second graph admits this assignment: take sign $+$ on $\{0,5,6,7\}$ and sign $-$ on $\{1,2,3,4\}$. Every paired face joins opposite signs, proving orientability. In the first graph the cycle

$$
1\xrightarrow{u_1}3\xrightarrow{\sigma}6\xrightarrow{t}2
\xrightarrow{\sigma}7\xrightarrow{t}1
$$

has odd length. Transporting [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) around it reverses the initial sign, proving nonorientability. Hence the first surface is also not [simply connected](../../../algebraic-topology.md#simply-connected-space). The second surface is [orientable](../../../differential-geometry.md#orientable-surface) but likewise not [simply connected](../../../algebraic-topology.md#simply-connected-space); the disk required in the question is supplied instead by the four-tile mixed-boundary construction above.

The four-tile construction resolves the printed simply-connected requirement under explicit [mixed boundary conditions](../../../differential-equation.md#mixed-boundary-condition). The eight-tile comparison only concerns [orientation of a surface](../../../differential-geometry.md#orientation-of-a-surface) under a pure [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition).

## 3

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Retain $\Delta=\operatorname{div}\nabla$ and define the [heat operator](../../../diffusion-equation.md#heat-operator) by $L=\partial_t-\Delta_q$. A [Riemannian heat kernel](../../../diffusion-equation.md#riemannian-heat-kernel) $H(p,q,t)$ satisfies $L_qH=0$ for $t>0$ and has the delta initial limit

$$
\lim_{t\downarrow0}\int_M H(p,q,t)f(q)\,dV_q=f(p).
$$

On standard [Euclidean space](../../../functional-analysis.md#euclidean-norm) the kernel is

$$
\boxed{g(p,q,t)=(4\pi t)^{-d/2}\exp\left(-\frac{|p-q|^2}{4t}\right).}
$$

On the [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold), the [Gaussian function](../../../calculus.md#gaussian-function) factor in the local construction uses $r(p,q)=\operatorname{dist}(p,q)$ in place of $|p-q|$.

Choose an open neighbourhood $\mathcal U$ of the diagonal such that every pair $(p,q)\in\mathcal U$ is joined by a unique short minimizing [geodesic](../../../riemannian-geometry.md#geodesic) and $q=\exp_p x$ with the inverse [exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry) smooth in both variables. It can be obtained from [normal coordinates](../../../general-relativity.md#normal-coordinates) tubes of radius smaller than the local [injectivity radius](../../../riemannian-geometry.md#injectivity-radius), or from normal neighbourhoods with [geodesic convexity](../../../riemannian-geometry.md#geodesic-convexity). Then $r^2$ is smooth on $\mathcal U$. Write the [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form) in [normal coordinates](../../../general-relativity.md#normal-coordinates) as $dV_q=J(p,x)\,dx$, where $J>0$ is smooth and $J(p,0)=1$.

For fixed $p$, radial divergence in [normal coordinates](../../../general-relativity.md#normal-coordinates) gives

$$
\Delta_qr=\frac{d-1}{r}+\partial_r\log J,
\qquad
\Delta_qr^2=2d+2r\partial_r\log J.
$$

For $g=(4\pi t)^{-d/2}e^{-r^2/(4t)}$, use $|\nabla r|=1$ away from the diagonal and the [product rule](../../../calculus.md#product-rule) to obtain

$$
L(g t^i w)=g\left[t^{i-1}\left(r\partial_r+i+\frac r2\partial_r\log J\right)w-t^i\Delta_qw\right].
$$

The identities extend smoothly in the expressions involving $r\partial_r$, even though $r$ itself is not smooth on the diagonal. The singular powers cancel if

$$
\left(r\partial_r+\frac r2\partial_r\log J\right)w_0=0,
\qquad
\left(r\partial_r+i+\frac r2\partial_r\log J\right)w_i=\Delta_qw_{i-1}\quad(i\geq1).
$$

The correct initial normalization is $w_0(p,p)=1$. These [heat-kernel transport equations](../../../diffusion-equation.md#heat-kernel-transport-equations) have the explicit solutions

$$
\boxed{w_0(p,\exp_p x)=J(p,x)^{-1/2},}
$$

and, recursively,

$$
\boxed{w_i(p,\exp_p x)
=J(p,x)^{-1/2}\int_0^1 s^{i-1}J(p,sx)^{1/2}
(\Delta_qw_{i-1})(p,\exp_p(sx))\,ds.}
$$

To derive the integral, multiply the radial equation by $r^{i-1}J^{1/2}$ and integrate the derivative of $r^iJ^{1/2}w_i$ from zero to $r$. The zero integration constant is forced by smoothness when $i\geq1$. Changing variables from radial distance to $s\in[0,1]$ gives the displayed nonsingular expression. Its integrand is smooth in $(p,x,s)$, so differentiation under the integral proves inductively that every $w_i$ is smooth across the diagonal. In particular $w_i(p,p)=(\Delta_qw_{i-1})(p,p)/i$.

Summing the product-rule identity makes adjacent terms telescope. For $S_k=g\sum_{i=0}^kt^iw_i$, the only term remaining is

$$
\boxed{LS_k=-g t^k\Delta_qw_k.}
$$

This also fixes the sign convention: with the nonnegative [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator) $P=-\Delta$, the right-hand side would instead be $+g t^kP_qw_k$.

A [heat parametrix](../../../diffusion-equation.md#heat-parametrix) is an approximate kernel with the same delta initial limit and an error under $L$ that is sufficiently regular, or flat, at $t=0$ to be corrected by time convolution. On a closed [compact manifold](../../../differential-geometry.md#compact-manifold) choose a smooth cutoff $\chi(p,q)$ equal to one near the diagonal and supported in $\mathcal U$. A finite-order explicit parametrix is

$$
P_N(p,q,t)=\chi(p,q)(4\pi t)^{-d/2}e^{-r^2/(4t)}\sum_{i=0}^N t^i w_i(p,q).
$$

Near the diagonal its error is $-\chi g t^N\Delta_qw_N$. Derivatives of $\chi$ produce errors supported a positive distance from the diagonal, where $e^{-r^2/(4t)}$ decays faster than every power of $t$. Taking $N$ large makes the whole error as regular at time zero as any specified finite number of derivatives requires. Its initial delta limit follows from $J(p,0)=w_0(p,p)=1$ and the Euclidean [Gaussian function](../../../calculus.md#gaussian-function) change of variables $x=\sqrt t\,y$.

One may obtain a smooth error flat at zero by summing all coefficients with time cutoffs. Let $\rho\in C^\infty([0,\infty))$ equal one near zero and zero for arguments at least one, and choose $\epsilon_i\downarrow0$ sufficiently fast. Set

$$
P(p,q,t)=\chi(p,q)g(p,q,t)\sum_{i=0}^{\infty}\rho(t/\epsilon_i)t^i w_i(p,q).
$$

For each $t>0$ the sum is locally finite. Choosing $\epsilon_i$ successively so that the $i$th term and its derivatives through order $\lfloor i/2\rfloor$ have bounds $2^{-i}$ on their cutoff transition regions gives the usual smooth asymptotic sum. For any fixed derivative order, its tail is then smaller than an arbitrarily high power of $t$; the transport identities cancel all earlier orders. Consequently $R=L_qP$ extends smoothly and flatly to $t=0$.

Here is the [Volterra parametrix correction](../../../diffusion-equation.md#volterra-parametrix-correction), with the order of the [Volterra convolution of kernels](../../../analysis.md#volterra-convolution-of-kernels) factors specified. Define

$$
(A*B)(p,q,t)=\int_0^t\!\int_M A(p,z,s)B(z,q,t-s)\,dV_z\,ds.
$$

Since $L$ acts in the second spatial variable and $P$ has the delta initial limit, $L_q(Q*P)=Q+Q*R$. Thus

$$
\boxed{Q=\sum_{j=1}^{\infty}(-1)^jR^{*j},\qquad H=P+Q*P.}
$$

Indeed, $Q+R+Q*R=0$ by the geometric-series cancellation, whence $L_qH=0$. If $|R|\leq C$ on a bounded time interval and $v=\operatorname{vol}(M)$, then

$$
|R^{*j}|\leq C^jv^{j-1}\frac{t^{j-1}}{(j-1)!}.
$$

This proves convergence; the smooth flat error permits the corresponding derivative estimates. The correction has zero initial limit, so $H$ retains the delta initial condition. Uniqueness of the [heat equation](../../../diffusion-equation.md#heat-equation) on a closed [compact manifold](../../../differential-geometry.md#compact-manifold) identifies this kernel with the global [Riemannian heat kernel](../../../diffusion-equation.md#riemannian-heat-kernel).

The local coefficient construction requires no [compactness](../../../topology.md#compact-space). The global uniformly bounded convolution argument just given uses a closed [compact manifold](../../../differential-geometry.md#compact-manifold), the usual spectral-geometry setting. For noncompact or incomplete [Riemannian manifolds](../../../riemannian-geometry.md#riemannian-manifold) one must specify the heat realization and justify global convergence separately; a canonical choice is the minimal kernel obtained as the increasing limit of Dirichlet kernels on a smooth relatively compact exhaustion. This gives the minimal heat semigroup rather than asserting an unqualified uniqueness statement at infinity or at a missing boundary.

## 4

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Here a [nowhere locally homogeneous metric](../../../differential-geometry.md#nowhere-locally-homogeneous-metric) means a smooth [Riemannian metric](../../../differential-geometry.md#riemannian-metric) with no nonidentity [local isometry](../../../differential-geometry.md#local-isometry): an [isometry](../../../riemannian-geometry.md#isometry) between open subsets must fix every point of its domain. This is the strong local-rigidity meaning of “bumpy” used in this question, not the different convention about nondegenerate closed [geodesics](../../../riemannian-geometry.md#geodesic). [Sunada's local isometry lemma](../../../differential-geometry.md#sunada-local-isometry-lemma) states that, on a closed [smooth manifold](../../../differential-geometry.md#smooth-manifold) of [dimension](../../../vector-space.md#dimension-vector-space) at least two, such [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) form a residual subset of the space of smooth [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) and are dense in its $C^\infty$ topology. In [dimension](../../../vector-space.md#dimension-vector-space) one this conclusion is false: arclength coordinates give local translations for every [Riemannian metric](../../../differential-geometry.md#riemannian-metric).

For maps $M^m\to N^n$, the [jet bundle of maps](../../../differential-geometry.md#jet-bundle-of-maps) $J^k(M,N)$ records the source point, the target value and all derivatives through order $k$. There are $\binom{m+k}{k}$ monomials of total degree at most $k$ in $m$ variables. Hence

$$
\boxed{\dim J^k(M,N)=m+n\binom{m+k}{k}.}
$$

Over $(x,y)\in M\times N$, the value is already fixed, so the fibre has [dimension](../../../vector-space.md#dimension-vector-space)

$$
\boxed{n\left(\binom{m+k}{k}-1\right).}
$$

In local coordinates it is the space of [Taylor series](../../../calculus.md#taylor-series) coefficients of orders one through $k$, represented by a [direct sum](../../../vector-space.md#direct-sum) of [symmetric powers](../../../linear-algebra.md#symmetric-power), $\bigoplus_{r=1}^k\operatorname{Sym}^r(T_x^*M)\otimes T_yN$. This [direct sum](../../../vector-space.md#direct-sum) identification is coordinate-dependent for $k>1$: higher derivatives mix with lower ones under nonlinear coordinate changes. Intrinsically, the truncation to order $k-1$ is an [affine bundle](../../../fiber-bundle.md#affine-bundle) modeled on $\operatorname{Sym}^k(T_x^*M)\otimes T_yN$. For $k=1$ the fibre is canonically $\operatorname{Hom}(T_xM,T_yN)$.

For the density assertion as printed, an [isometry](../../../riemannian-geometry.md#isometry) $\overline U_i\to\overline U_j$ is a bijective Riemannian [isometry](../../../riemannian-geometry.md#isometry). A [localized volume perturbation](../../../differential-geometry.md#localized-volume-perturbation) suffices; it is not necessary to prove the stronger generic local-rigidity lemma afresh. We take the coordinate-ball basis without repetitions, and each $U_i$ as the interior of its smooth closed-ball closure. Distinct such domains have a nonempty open difference in at least one direction. Indeed, if both were contained in the other's closure, their regular-open property $U=\operatorname{int}\overline U$ would make them equal.

Fix any [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $g$. If the two domains have unequal volumes, they cannot be isometric, so $g$ already lies in the desired complement. Otherwise, after interchanging the two indices if necessary, choose a nonnegative nonzero [smooth bump function](../../../partial-differential-equation.md#smooth-bump-function) $\psi$ supported in $U_i\setminus\overline U_j$, and set

$$
g_\epsilon=e^{2\epsilon\psi}g.
$$

These are positive-definite smooth [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) tending to $g$ in the $C^\infty$ topology as $\epsilon\to0$. Their [Riemannian volume forms](../../../differential-geometry.md#riemannian-volume-form) satisfy $dV_{g_\epsilon}=e^{m\epsilon\psi}dV_g$. The [Riemannian metric](../../../differential-geometry.md#riemannian-metric) and volume on $U_j$ are unchanged, whereas

$$
\left.\frac d{d\epsilon}\operatorname{vol}_{g_\epsilon}(U_i)\right|_{\epsilon=0}
=m\int_{U_i}\psi\,dV_g>0.
$$

For every sufficiently small $\epsilon>0$, the volumes differ. Thus no [isometry](../../../riemannian-geometry.md#isometry) of the two closed domains exists, proving

$$
\boxed{\mathcal C\mathcal S_{ij}\text{ is dense in the space of smooth metrics}.}
$$

The volume difference is continuous in the smooth topology, so the unequal-volume [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) even form an open dense subset of this complement. The regular-open assumption is also needed to justify this literal closed-domain assertion. As written, requiring only that each closure be a closed ball permits two distinct basis members with the same closure. For example in $\mathbb R^m$, adjoin $U=B(0,1)$ and $V=B(0,1)\setminus\{0\}$ to a countable [basis of a topology](../../../topology.md#basis-of-a-topology) of coordinate balls. Both are open and both closures are the same closed ball. The identity is an [isometry](../../../riemannian-geometry.md#isometry) of those closures for every [Riemannian metric](../../../differential-geometry.md#riemannian-metric), so the indicated complement is empty. Thus the conclusion needs distinct closures, as in the usual basis of genuine coordinate balls used above. The no-repetitions convention is necessary as well: if the indexed basis repeats a domain, its identity map is always an [isometry](../../../riemannian-geometry.md#isometry) and the asserted complement for those two indices is empty. This volume argument concerns [isometries](../../../riemannian-geometry.md#isometry) onto the specified whole domains; the stronger assertion excluding arbitrary [local isometries](../../../differential-geometry.md#local-isometry) is the separate Sunada lemma stated above.

## 5

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

[Sunada's theorem](../../../riemannian-geometry.md#sunada-theorem) states that if a [finite group](../../../group.md#finite-group) $T$ acts isometrically on a closed [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) $X$, and two [Gassmann equivalent](../../../representation-theory.md#gassmann-equivalence) [subgroups](../../../group.md#subgroup) $H_1,H_2$ act freely, then $H_1\backslash X$ and $H_2\backslash X$ are isospectral for the function [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator). [Gassmann equivalence](../../../representation-theory.md#gassmann-equivalence) means $|H_1\cap C|=|H_2\cap C|$ for every [conjugacy class](../../../group-theory.md#conjugacy-class) $C$ of $T$. For each [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator) [eigenspace](../../../linear-operator-theory.md#eigenspace) $E_\lambda$, its [invariant subspace](../../../representation-theory.md#invariant-subspace) has [dimension](../../../vector-space.md#dimension-vector-space)

$$
\dim E_\lambda^{H_i}=\frac1{|H_i|}\sum_{h\in H_i}\operatorname{tr}(h|E_\lambda).
$$

The [character of a representation](../../../representation-theory.md#character-of-a-representation) is a [class function](../../../representation-theory.md#class-function), so the two [multiplicities](../../../polynomial.md#multiplicity-mathematics) agree. A necessary condition for nonisometry is that the [subgroups](../../../group.md#subgroup) are not conjugate in $T$: conjugation by an ambient deck transformation would induce an [isometry](../../../riemannian-geometry.md#isometry). This is not sufficient when the common covering has additional geometric symmetries.

Use the oriented [hyperbolic triangle group](../../../geometric-group-theory.md#hyperbolic-triangle-group)

$$
\Gamma=\langle a,b:a^3=b^3=(ab)^6=1\rangle
$$

and the epimorphism $\rho:\Gamma\to T$ given by $a\mapsto s$, $b\mapsto d$. Its base [orbifold](../../../geometry-and-topology.md#orbifold) is the doubled hyperbolic triangle with angles $\pi/3,\pi/3,\pi/6$, having signature $(0;3,3,6)$. Let $K=\ker\rho$ and $K_i=\rho^{-1}(H_i)$.

The groups $K_i$ are torsion free. Indeed, [torsion elements](../../../group-theory.md#torsion-element) in an oriented triangle [group](../../../group.md) are conjugate to nontrivial powers of its three vertex rotations. Such powers map either to elements of order three, which cannot lie in a [subgroup](../../../group.md#subgroup) of order $96/12=8$, or to the order-two cube $z=(sd)^3$. The latter is central and absent from both $H_i$, so it is absent from every conjugate as well. Thus the degree-twelve [orbifold](../../../geometry-and-topology.md#orbifold) covers

$$
N_i=K_i\backslash\mathbb H^2
$$

are smooth, closed, connected [orientable](../../../differential-geometry.md#orientable-surface) surfaces. The common cover $X=K\backslash\mathbb H^2$ is smooth too; $H_i$ act freely on it. [Orbifold](../../../geometry-and-topology.md#orbifold) [Euler characteristic](../../../homology.md#euler-characteristic) gives

$$
\boxed{\chi(N_i)=12\left(\frac13+\frac13+\frac16-1\right)=-2,\qquad\operatorname{genus}(N_i)=2.}
$$

For example, this formula follows by triangulating the base and weighting a vertex of order $r$ by $1/r$ before multiplying by the cover degree. Equivalently, each doubled triangle has hyperbolic area $\pi/3$, so $N_i$ has area $4\pi$ and [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) gives the same [genus](../../../topology.md#genus-of-a-surface).

There is one extra issue in obtaining the same hyperbolic limit on a single marked surface: the two limiting hyperbolic covers must themselves be isometric. Nonconjugacy and the displayed element orders alone do not prove this. An explicit realization of the supplied example resolves the issue. The [group](../../../group.md) seed is recorded in [the original genus-two construction](https://arxiv.org/pdf/math/0512519); the following coset actions and reflection identities give a direct verification. Label the twelve sheets so that the two right-coset actions of $s,d$ are

$$
\begin{aligned}
s_1&=(1\ 3\ 6)(2\ 11\ 7)(4\ 8\ 9)(5\ 10\ 12),\\
d_1&=(1\ 12\ 8)(2\ 3\ 7)(4\ 5\ 10)(6\ 9\ 11),\\
s_2&=(1\ 6\ 12)(2\ 8\ 11)(3\ 7\ 10)(4\ 5\ 9),\\
d_2&=(1\ 6\ 10)(2\ 8\ 9)(3\ 5\ 11)(4\ 7\ 12).
\end{aligned}
$$

These are concrete permutation data for an order-$96$ realization with the required two [subgroups](../../../group.md#subgroup). The permutation

$$
P=(1\ 3\ 10\ 2)(4\ 9)(5\ 8)(6\ 7)(11\ 12)
$$

satisfies, by direct substitution,

$$
Ps_1=s_2^{-1}P,\qquad Pd_1=d_2^{-1}P.
$$

Reflection of the doubled triangle reverses both vertex rotations. Apply this reflection on every [fundamental domain](../../../group-theory.md#fundamental-domain) and relabel sheets by $P$. The two identities ensure that identified edges go to identified edges, so this descends to a hyperbolic [isometry](../../../riemannian-geometry.md#isometry) $F_0:N_1\to N_2$. Fix $N=N_1$, let $g$ be its [hyperbolic metric](../../../geometry-and-topology.md#hyperbolic-metric), and use $F_0$ to mark $N_2$ by the same smooth surface. Thus both pulled-back limiting [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) are exactly $g$. The explicit reversed-action check is what makes the common limit justified, rather than treating it as a consequence of [Sunada's theorem](../../../riemannian-geometry.md#sunada-theorem).

Choose smooth [orbifold](../../../geometry-and-topology.md#orbifold) [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) $h_k$ on the base converging to its [hyperbolic metric](../../../geometry-and-topology.md#hyperbolic-metric) $h_0$, with no nonidentity [local isometry](../../../differential-geometry.md#local-isometry) on the regular part. The density assertion in [Sunada's local isometry lemma](../../../differential-geometry.md#sunada-local-isometry-lemma) applies in [orbifold](../../../geometry-and-topology.md#orbifold) charts as well: use equivariant perturbations at the finitely many cone points and ordinary local perturbations elsewhere. Smoothness here is [orbifold](../../../geometry-and-topology.md#orbifold) smoothness, so the lifted [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) on $X$ and the two smooth covers are ordinary smooth [Riemannian metrics](../../../differential-geometry.md#riemannian-metric). Such choices can be made in successively smaller smooth neighbourhoods of $h_0$; cone orders and the topological coverings stay fixed.

For [area separation of convergent Sunada families](../../../riemannian-geometry.md#area-separation-of-convergent-sunada-families), adjust each $h_k$ by a constant positive factor so that

$$
\operatorname{area}(h_k)=\operatorname{area}(h_0)(1+2^{-k}).
$$

Explicitly, multiply the initially chosen [Riemannian metric](../../../differential-geometry.md#riemannian-metric) by the ratio of the desired area to its actual area. In [dimension](../../../vector-space.md#dimension-vector-space) two this ratio is exactly the area multiplier. The ratios tend to one, so smooth convergence persists, and constant scaling preserves the absence of [local isometries](../../../differential-geometry.md#local-isometry). Lift these adjusted [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) to $N_i$ and pull them back by the fixed markings to obtain $g_{ik}$, for $i=1,2$. The three required properties follow below.

<h3 id="5/1">1</h3>

↑ **Parent:** [5](#5)

<h4 id="5/1/solution">Solution</h4>

↑ **Parent:** [1](#5/1)

For each fixed $k$, the two quotient [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) are not isometric. If an [isometry](../../../riemannian-geometry.md#isometry) $F:N_1\to N_2$ existed, choose a small open set avoiding the finite preimages of cone points and their inverse images under $F$. Composing $F$ with the local inverse of the first base projection and the second base projection gives a [local isometry](../../../differential-geometry.md#local-isometry) of the base [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $h_k$. Local rigidity forces this map to be the identity. Hence $p_2F=p_1$ on a dense open set, and by [continuity](../../../calculus.md#continuous-function) everywhere.

The alleged [isometry](../../../riemannian-geometry.md#isometry) would therefore be an isomorphism of the two [orbifold](../../../geometry-and-topology.md#orbifold) covers over the same base. Covering-space classification makes $K_1,K_2$ conjugate in $\Gamma$, and applying $\rho$ makes $H_1,H_2$ conjugate in $T$, contrary to the supplied hypothesis. Thus $g_{1k},g_{2k}$ are nonisometric.

For $k\ne\ell$, the surface areas are different:

$$
\boxed{\operatorname{area}(N,g_{ik})=4\pi(1+2^{-k}).}
$$

Area is preserved by [isometries](../../../riemannian-geometry.md#isometry), so no surface from the $k$th pair is isometric to a surface from the $\ell$th pair. Together these arguments prove the full pairwise nonisometry assertion.

<h3 id="5/2">2</h3>

↑ **Parent:** [5](#5)

<h4 id="5/2/solution">Solution</h4>

↑ **Parent:** [2](#5/2)

For each $k$, the lifted [Riemannian metric](../../../differential-geometry.md#riemannian-metric) on $X$ is $T$-invariant and the two [subgroups](../../../group.md#subgroup) still act freely. [Sunada's theorem](../../../riemannian-geometry.md#sunada-theorem) therefore gives

$$
\boxed{\operatorname{Spec}(N,g_{1k})=\operatorname{Spec}(N,g_{2k}).}
$$

To rule out any other equalities, the leading diagonal [heat kernel expansion](../../../diffusion-equation.md#heat-kernel-expansion) from Question 3 gives, on a closed surface,

$$
\operatorname{Tr}(e^{-tP})=\frac{\operatorname{area}(N)}{4\pi t}+O(1)\quad(t\downarrow0).
$$

Thus the function [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) determines area: multiply the [heat trace](../../../riemannian-geometry.md#heat-trace) by $4\pi t$ and take the limit. Since the chosen areas are distinct for distinct $k$, no cross-pair spectra can agree. This proves exactly the prescribed spectral coincidences.

<h3 id="5/3">3</h3>

↑ **Parent:** [5](#5)

<h4 id="5/3/solution">Solution</h4>

↑ **Parent:** [3](#5/3)

The base [Riemannian metrics](../../../differential-geometry.md#riemannian-metric) satisfy $h_k\to h_0$ in the smooth topology, and the fixed smooth [covering maps](../../../algebraic-topology.md#covering-space) pull this convergence back to both $N_i$. Although the base has cone points, each lifted chart is an ordinary smooth chart, so convergence holds there as well. The fixed [isometry](../../../riemannian-geometry.md#isometry) $F_0$ used to mark the second limit gives

$$
\boxed{g_{1k}\longrightarrow g,\qquad g_{2k}\longrightarrow g\quad\hbox{in }C^\infty(N).}
$$

The area normalizations multiply by constants tending to one and therefore do not change these limits. There are precisely two sequences, indexed by $i=1,2$; the appearance of $i=1,2,3,\ldots$ in the printed last condition is a redundant indexing error, not a requirement for additional families. The common limit is isometric even though every finite pair is nonisometric, because the hyperbolic limit recovers the reflection symmetry broken by the locally rigid perturbations.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
