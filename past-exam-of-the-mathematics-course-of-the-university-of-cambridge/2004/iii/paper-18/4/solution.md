<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $T=\operatorname{PSL}(3,2)=\operatorname{GL}(3,\mathbb F_2)$, of order $(8-1)(8-2)(8-4)=168$. It acts on the seven points and seven lines of the [Fano plane](../../../../../fano-plane.md). Take $U_1$ to be a point stabilizer and $U_2$ to be a line stabilizer; both have index seven and order twenty-four. The fact that [point and hyperplane stabilizers are almost conjugate](../../../../../point-and-hyperplane-stabilizers-are-almost-conjugate.md) follows by comparing fixed-point counts: for a matrix $g$, the numbers of fixed nonzero vectors and fixed nonzero covectors are both

$$
2^{\dim\ker(g-I)}-1,
$$

because $g-I$ and its transpose have the same rank, and the dual action $g^{-T}$ has the same fixed space as $g^T$. Over $\mathbb F_2$, nonzero vectors represent points and nonzero covectors represent lines without any further scalar quotient. The two [permutation characters](../../../../../permutation-character.md) therefore agree. The coset-character formula

$$
\chi_{T/U_i}(g)=\frac{|C_T(g)|}{|U_i|}\,|U_i\cap[g]_T|
$$

then proves [Gassmann equivalence](../../../../../gassmann-equivalence.md). They are not conjugate: a point stabilizer has orbits of sizes one and six on points and hence preserves no three-point line. Its conjugates are again point stabilizers, whereas $U_2$ preserves its line. **The point and line stabilizers form the required nonconjugate Gassmann pair.**

We construct a family using the [Lambert quadrilateral construction of a cone torus](../../../../../lambert-quadrilateral-construction-of-a-cone-torus.md). Let $\alpha=\pi/14$. We use the elementary [hyperbolic tri-rectangle](../../../../../lambert-quadrilateral.md) fact that a quadrilateral with three right angles, remaining angle $\alpha$, and side lengths $x,y$ adjacent to the right-angle vertex opposite $\alpha$ exists uniquely for

$$
\sinh x\sinh y=\cos\alpha,\qquad x,y>0.
$$

Here $x,y$ are the sides at the opposite right-angle corner, not the sides incident to $\alpha$. Given any $x>0$, choose $y=\operatorname{arsinh}(\cos\alpha/\sinh x)$. Reflect four copies around the opposite right-angle vertex. The result is a symmetric hyperbolic quadrilateral with all four corner angles $\alpha$ and opposite sides of equal lengths. Pair opposite sides by the axis translations. The quotient is an oriented torus with one cone point, whose total angle is $4\alpha=2\pi/7$. Its two central axis loops $a,d$ are embedded closed [geodesics](../../../../../geodesic.md), of lengths $2x,2y$, intersecting once at right angles.

Cut this cone torus along $a$. The result is a hyperbolic pair of pants with two geodesic boundaries of length $\ell=2x$ and the cone point. Reglue those equal boundaries with a [Fenchel–Nielsen twist](../../../../../fenchel-nielsen-twist.md) $\tau\in\mathbb R$. This gives a two-parameter family $B_{\ell,\tau}$, with the same cone angle, and marked simple classes $a,d$ meeting once. Near any zero-twist member their geodesic representatives remain embedded, transverse and disjoint from the cone point. The length of $a$ remains $\ell$, and the right-angle matrix product gives

$$
\cosh\frac{\ell_d(\ell,\tau)}2=\cosh y(\ell)\cosh\frac\tau2.
$$

For example, the zero-twist holonomies are $\operatorname{diag}(e^x,e^{-x})$ and $\begin{pmatrix}\cosh y&\sinh y\\\sinh y&\cosh y\end{pmatrix}$; multiply the latter by $\operatorname{diag}(e^{\tau/2},e^{-\tau/2})$ to obtain the twist formula. Their commutator has trace $2-4\sinh^2x\sinh^2y=-2\cos(\pi/7)$, confirming exact elliptic order seven. The side-pairing construction supplies discreteness; the trace computation alone would not do so.

The [orbifold fundamental group](../../../../../orbifold-fundamental-group.md) is

$$
\Gamma=\langle a,d\mid[d,a]^7=1\rangle.
$$

Send $a$ to the supplied generator $A$ and $d$ to $D$. Their commutator $C=[D,A]$ has order seven, so this defines an epimorphism $\rho:\Gamma\to T$. Its kernel avoids all nontrivial cone stabilizers, which are conjugates of powers of $[d,a]$; therefore it is torsion-free. It defines a smooth closed regular hyperbolic cover $X_{\ell,\tau}\to B_{\ell,\tau}$ with deck group $T$. The subgroups $U_i$, of order twenty-four, also avoid every order-seven cone stabilizer. Thus

$$
S_i(\ell,\tau)=U_i\backslash X_{\ell,\tau}
$$

are smooth closed seven-sheeted covers of the cone torus. The [orbifold Euler characteristic](../../../../../orbifold-euler-characteristic.md) is $\chi_{\mathrm{orb}}(B)=-(1-1/7)=-6/7$, giving

$$
\chi(S_i)=7(-6/7)=-6,\qquad \boxed{g(S_i)=4.}
$$

Equivalently there is one preimage of the cone point, with local degree seven, and its lifted angle is $2\pi$. The [Sunada theorem](../../../../../sunada-theorem.md), in the free-subgroup-action form proved above, makes $S_1(\ell,\tau)$ and $S_2(\ell,\tau)$ isospectral for every parameter.

Nonisometry requires further work. A cycle of length $r$ in the [monodromy permutation](../../../../../monodromy-permutation.md) of a simple base [geodesic](../../../../../geodesic.md) gives a primitive simple lifted geodesic of length $r$ times the base length. From the supplied $A$ action, each cover has one lift of $a$ of length $\ell$ and two of length $3\ell$. From the supplied $D$ action, each has one lift of $d$ of each length $\ell_d,2\ell_d,4\ell_d$. Let $\beta_i$ be the unique two-cycle lift of $d$, and let $\alpha_{i,1},\alpha_{i,2}$ be the two three-cycle lifts of $a$. The fact that [cycle intersections count intersections of lifted curves](../../../../../cycle-intersections-count-intersections-of-lifted-curves.md) gives their intersection numbers: the seven crossings above the one base crossing are labelled by the sheets, so a crossing belongs to both lifted components exactly when its sheet lies in both cycles. Consequently

$$
\{i(\alpha_{1,1},\beta_1),i(\alpha_{1,2},\beta_1)\}=\{0,1\},\qquad
\{i(\alpha_{2,1},\beta_2),i(\alpha_{2,2},\beta_2)\}=\{0,2\}.
$$

Indeed, in the first cover the two three-cycles have supports $\{1,2,5\},\{3,6,4\}$ and the two-cycle has support $\{0,3\}$; in the second they have supports $\{1,4,3\},\{2,5,6\}$ and $\{2,5\}$. The lifted curves intersect only over the single base crossing, so these are actual intersection counts of the geodesics, not merely abstract sheet-incidence numbers.

To make this a test against every [isometry](../../../../../isometry.md), we must identify these curves intrinsically, rather than require the isometry to respect the covering map. We use [generic isolation of lifted simple geodesics](../../../../../generic-isolation-of-lifted-simple-geodesics.md), and give the needed genericity argument. Lengths of closed geodesics are real-analytic functions of the cone-torus length and twist parameters. For a primitive hyperbolic class $w$ and an integer $1\leq r\leq7$, consider the equalities

$$
r\ell_w(\ell,\tau)=3\ell\quad\text{or}\quad r\ell_w(\ell,\tau)=2\ell_d(\ell,\tau).
$$

Apart from $w=a,r=3$ or $w=d,r=2$, none is an identity on the full two-parameter family. To see this for the first equality, pinch the simple curve $a$ while keeping the cone angle fixed. The [collar lemma](../../../../../collar-lemma.md) makes every class crossing $a$ long. A class disjoint from $a$ lies in the cut pair of pants; its limiting holonomy has positive translation length unless it is a power of one of the new cusp loops, which are conjugate to $a$ in the torus group. Cone-peripheral classes are elliptic and do not represent closed geodesics. Thus the only primitive class with length tending to zero in this degeneration is $a$, up to inversion and conjugacy. This excludes an identity with a positive multiple of $\ell$. Pinching $d$ proves the corresponding assertion for $\ell_d$. The argument uses the usual hyperbolic collar and cusp degeneration facts, obtainable by the right-angle quadrilateral formulas; the cone angle $2\pi/7<\pi$ remains fixed. Analytic continuation on the connected length-twist parameter space shows that the same identities cannot hold on a small open neighbourhood of a zero-twist member.

There are countably many class equations, and each nontrivial real-analytic equation has a closed zero set with empty interior. The [Baire category theorem](../../../../../baire-category-theorem.md) therefore gives a parameter $(\ell_0,\tau_0)$ in that small neighbourhood at which both target lengths are attained only by the prescribed lift components. This isolation persists on a smaller open neighbourhood. Indeed, near a fixed compact hyperbolic metric there are uniformly only finitely many primitive geodesic classes below a fixed length bound, by discreteness of the covering group and a compact fundamental region; nearby metrics are uniformly bilipschitz. Only finitely many classes can therefore approach the two fixed finite target lengths. Their strict inequalities persist under a sufficiently small parameter change.

Now keep $\tau=\tau_0$ and let $\ell$ vary in a sufficiently small interval $I$ around $\ell_0$. For each $\ell\in I$, the only primitive geodesics of length $3\ell$ in either cover are the two $\alpha$ components, and the only primitive geodesic of length $2\ell_d$ is $\beta$. An [isometry](../../../../../isometry.md) would have to preserve these length classes and their intersection-count multiset, contradicting $\{0,1\}\ne\{0,2\}$. Hence

$$
\boxed{\bigl(S_1(\ell,\tau_0),S_2(\ell,\tau_0)\bigr),\quad\ell\in I,}
$$

is an interval-parametrized family of isospectral nonisometric hyperbolic [Riemann surfaces](../../../../../riemann-surfaces.md) of genus four. Shrink $I$ again so a small length window around $3\ell_0$ contains only those two components for every parameter. Their common length $3\ell$ varies strictly, so members at distinct parameters cannot all be the same surface in different markings. The spectra agree within each pair; this construction does not assert a nontrivial continuously isospectral deformation of one hyperbolic surface.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
