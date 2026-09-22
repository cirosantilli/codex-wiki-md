# Paper 19

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper19.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper19.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Put $\delta=-A^2-A^{-2}$. The reduced [Kauffman bracket](../../../knot-theory.md#kauffman-bracket) is the [Laurent polynomial](../../../polynomial.md#laurent-polynomial) determined by $\langle\bigcirc\rangle=1$, $\langle D\sqcup\bigcirc\rangle=\delta\langle D\rangle$, and the crossing expansion $\langle D\rangle=A\langle D_A\rangle+A^{-1}\langle D_B\rangle$. Fix the A smoothing so that a positive curl has multiplier $-A^3$; rotating the local crossing interchanges the smoothing descriptions. Equivalently, its [bracket smoothing states](../../../knot-theory.md#bracket-smoothing-state) give

$$
\boxed{\langle D\rangle=\sum_sA^{a(s)-b(s)}\delta^{|s|-1},}
$$

where $a(s)$ and $b(s)$ count its A and B smoothings and $|s|$ is the number of state [circles](../../../topology.md#circle). Resolving all crossings proves that the recursive rules define the same [polynomial](../../../polynomial.md) independently of the order of expansion.

Under a positive [Reidemeister move](../../../knot-theory.md#reidemeister-move) of type I, the two resolutions give $A\delta+A^{-1}=-A^3$ times the straight strand; the negative curl gives $A^{-1}\delta+A=-A^{-3}$. Thus the bracket itself is not an unframed [link invariant](../../../knot-theory.md#link-invariant). For type II, use the adjacent cap-cup generator $e$ of the [Temperley-Lieb algebra](../../../knot-theory.md#temperley-lieb-diagram-algebra), with $e^2=\delta e$. The crossing and its inverse are $R=A1+A^{-1}e$ and $R^{-1}=A^{-1}1+Ae$, and

$$
RR^{-1}=1+(A^2+A^{-2}+\delta)e=1.
$$

For type III, $e_ie_{i+1}e_i=e_i$ and the analogous reversed relation give

$$
R_iR_{i+1}R_i-R_{i+1}R_iR_{i+1}=A^{-1}(A^2+\delta+A^{-2})(e_i-e_{i+1})=0.
$$

Hence the bracket is invariant under types II and III.

For an oriented diagram, let $w(D)$ be its [writhe of a link diagram](../../../knot-theory.md#writhe-of-a-link-diagram), the sum of its signed crossings. Types II and III preserve [writhe of a link diagram](../../../knot-theory.md#writhe-of-a-link-diagram), while a positive or negative curl changes it by one or minus one. The [Jones polynomial](../../../knot-theory.md#jones-polynomial) is therefore

$$
\boxed{V_L(t)=(-A^3)^{-w(D)}\langle D\rangle,\qquad t=A^{-4},\qquad V_{\bigcirc}=1.}
$$

The normalization cancels type I, so all [Reidemeister moves](../../../knot-theory.md#reidemeister-move) preserve it. It is a [Laurent polynomial](../../../polynomial.md#laurent-polynomial) in $t^{1/2}$; its breadth means the largest occurring t exponent minus the smallest, including half-integral exponents for [links](../../../knot-theory.md#link).

The [Jones polynomial skein relation](../../../knot-theory.md#jones-polynomial-skein-relation) follows directly from the same normalization. Write $S$ for the bracket of the [oriented smoothing](../../../knot-theory.md#oriented-smoothing) and $H$ for the other smoothing. The local expansions are $\langle D_+\rangle=AS+A^{-1}H$ and $\langle D_-\rangle=A^{-1}S+AH$, while $w(D_\pm)=w(D_0)\pm1$. Consequently

$$
A^4V_{L_+}-A^{-4}V_{L_-}=(-A^3)^{-w(D_0)}(A^{-2}-A^2)S.
$$

Substituting $t=A^{-4}$ gives

$$
\boxed{t^{-1}V_{L_+}-tV_{L_-}+(t^{-1/2}-t^{1/2})V_{L_0}=0.}
$$

The other smoothing has cancelled, so the identity applies with exactly the oriented local convention in the PDF.

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

**True.** In a [connected sum of knots](../../../knot-theory.md#connected-sum-of-knots), a [bracket smoothing state](../../../knot-theory.md#bracket-smoothing-state) from each summand contributes a state of the joined diagram. Joining the two distinguished state [circles](../../../topology.md#circle) reduces their total count by one, so the factors $\delta^{s-1}$ multiply. The smoothing weights also multiply and the [writhe of a link diagram](../../../knot-theory.md#writhe-of-a-link-diagram) adds. Thus the [Jones polynomial of a connected sum](../../../knot-theory.md#jones-polynomial-of-a-connected-sum) is

$$
\boxed{V_{K_1\#K_2}(t)=V_{K_1}(t)V_{K_2}(t).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

**False.** The zero [polynomial](../../../polynomial.md) is already a counterexample. The [Jones polynomial evaluation at one](../../../knot-theory.md#jones-polynomial-evaluation-at-one) of a nonempty [link](../../../knot-theory.md#link) with $\ell$ components is

$$
V_L(1)=(-2)^{\ell-1}\ne0.
$$

To prove this, specialize the [Jones polynomial skein relation](../../../knot-theory.md#jones-polynomial-skein-relation) at $t=1$: switching a crossing preserves the value. Switch crossings until the diagram is an [unlink](../../../knot-theory.md#unlink) without changing its component count. The [Kauffman bracket](../../../knot-theory.md#kauffman-bracket) loop rule, equivalently the [Jones polynomial of a split union](../../../knot-theory.md#jones-polynomial-of-a-split-union), gives the displayed evaluation. Hence arbitrary Laurent [polynomials](../../../polynomial.md) cannot occur.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**False as written for arbitrary links.** The two-component [unlink](../../../knot-theory.md#unlink) has a diagram with no crossings but

$$
\boxed{V_{U\sqcup U}(t)=-(t^{1/2}+t^{-1/2}),\qquad\operatorname{br}V_{U\sqcup U}=1>0.}
$$

The correct connected-diagram statement does hold, in particular for every [knot diagram](../../../knot-theory.md#knot-diagram). If $s_A,s_B$ count the all-$A$ and all-$B$ [bracket smoothing state](../../../knot-theory.md#bracket-smoothing-state) [circles](../../../topology.md#circle), changing $j$ smoothings increases the circle count by at most $j$. The maximum and minimum $A$ exponents therefore lie between $n+2s_A-2$ and $-n-2s_B+2$. This gives the [Kauffman bracket breadth bound](../../../knot-theory.md#kauffman-bracket-breadth-bound) $\operatorname{br}_A\langle D\rangle\leq2n+2s_A+2s_B-4$. For a connected projection, the [Turaev surface](../../../knot-theory.md#turaev-surface) has [Euler characteristic](../../../homology.md#euler-characteristic) $s_A+s_B-n\leq2$, so the bound is $4n$. [Writhe of a link diagram](../../../knot-theory.md#writhe-of-a-link-diagram) normalization changes only a [monomial](../../../polynomial.md#monomial), and $t=A^{-4}$ divides the breadth by four, giving $\operatorname{br}V_L\leq n$.

For a diagram with $k$ projection components, sum the same [Euler characteristic](../../../homology.md#euler-characteristic) inequality over the components. Then $s_A+s_B\leq n+2k$ and the [Jones polynomial breadth bound for a disconnected diagram](../../../knot-theory.md#jones-polynomial-breadth-bound-for-a-disconnected-diagram) is $\operatorname{br}V_L\leq n+k-1$. The extra $k-1$ is indispensable, as the [unlink](../../../knot-theory.md#unlink) shows.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

**True with the stated Conway normalization.** Fix $t^{1/2}=i$ at $t=-1$. The [Jones polynomial skein relation](../../../knot-theory.md#jones-polynomial-skein-relation) becomes

$$
V_{L_+}(-1)-V_{L_-}(-1)=-2iV_{L_0}(-1).
$$

The [Conway polynomial](../../../knot-theory.md#conway-polynomial-knot-theory) satisfies $\nabla_{L_+}(z)-\nabla_{L_-}(z)=z\nabla_{L_0}(z)$. Put $W_L=(-1)^{\ell(L)-1}\nabla_L(2i)$. An [oriented smoothing](../../../knot-theory.md#oriented-smoothing) changes the number of components by one, so these quantities satisfy precisely $W_{L_+}-W_{L_-}=-2iW_{L_0}$. Both $W$ and $V(-1)$ are one on the [unknot](../../../knot-theory.md#unknot) and zero on every multi-component [unlink](../../../knot-theory.md#unlink): for $V$, the split-union factor vanishes at this substitution.

These [skein relations](../../../knot-theory.md#skein-relation) and [unlink](../../../knot-theory.md#unlink) values determine the invariants uniquely. Switching a first undesired crossing gives a diagram closer to a descending diagram, while the smoothing term has fewer crossings; induction first on crossing count and then on undesired crossings reduces everything to [unlinks](../../../knot-theory.md#unlink). Thus $W_L=V_L(-1)$. For a [knot](../../../knot-theory.md#knot) there is one component and the [Conway-normalized Alexander polynomial](../../../knot-theory.md#conway-normalized-alexander-polynomial) gives

$$
\boxed{V_K(-1)=\nabla_K(2i)=\Delta_K(-1).}
$$

This is the [signed Jones evaluation at minus one](../../../knot-theory.md#signed-jones-evaluation-at-minus-one). Replacing $\Delta_K$ by an arbitrary [Laurent unit](../../../commutative-algebra.md#unit-of-a-laurent-polynomial-ring) multiple would destroy the signed conclusion.

## 2

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

To form the [connected sum of knots](../../../knot-theory.md#connected-sum-of-knots) $K_1\#K_2$, remove a short unknotted arc from each oriented [knot](../../../knot-theory.md#knot) in two disjoint balls and join the remaining endpoints by a pair of parallel arcs respecting the orientations. Equivalently, a [sphere](../../../geometry-and-topology.md#sphere) meeting a [knot](../../../knot-theory.md#knot) in two points cuts it into two one-string [tangles](../../../knot-theory.md#tangle); close each by an arc in the [sphere](../../../geometry-and-topology.md#sphere) to recover its summands. Sliding the small joining balls along the [knots](../../../knot-theory.md#knot) shows that the [isotopy](../../../differential-geometry.md#isotopy) type does not depend on these choices. The [unknot](../../../knot-theory.md#unknot) is the identity for this operation. A [prime knot](../../../knot-theory.md#prime-knot) is a nontrivial [knot](../../../knot-theory.md#knot) such that every expression $K=K_1\#K_2$ has an [unknot](../../../knot-theory.md#unknot) summand.

The [Seifert algorithm](../../../knot-theory.md#seifert-algorithm) supplies a [Seifert surface](../../../knot-theory.md#seifert-surface) for every oriented [knot](../../../knot-theory.md#knot): smooth the crossings in their oriented directions, span the resulting [Seifert circles](../../../knot-theory.md#seifert-circle) by disks at different heights, and restore each crossing with a half-twisted band. If needed, join components by tubes away from the boundary. Thus the set of surface genera is a nonempty subset of the [nonnegative integers](../../../arithmetic.md#natural-number) and has a minimum, so $g_s(K)$ exists.

We first prove [additivity of Seifert genus](../../../knot-theory.md#additivity-of-seifert-genus), which also supplies a terminating measure for decomposition. Joining minimal [Seifert surfaces](../../../knot-theory.md#seifert-surface) along their boundary arcs gives $g_s(K_1\#K_2)\leq g_s(K_1)+g_s(K_2)$. For the reverse inequality, let $F$ be a minimal-genus [Seifert surface](../../../knot-theory.md#seifert-surface) for the sum and $S$ a [splitting sphere of a knot](../../../knot-theory.md#splitting-sphere-of-a-knot). Arrange transverse intersection so that $F\cap S$ consists of one arc joining the two boundary-intersection points and some [circles](../../../topology.md#circle), with the number of [circles](../../../topology.md#circle) minimal among genus-minimizing [surfaces](../../../topology.md#topological-surface).

Each [circle](../../../topology.md#circle) separates the [sphere](../../../geometry-and-topology.md#sphere) into two disks; since it is disjoint from the intersection arc, one disk contains neither marked endpoint. Choose an innermost such [circle](../../../topology.md#circle) and its disk $D\subset S$, whose interior misses $F$. If its boundary were essential in $F$, compressing $F$ along $D$ would lower the genus of its component with boundary K: for a nonseparating curve genus drops by one, and for a separating essential curve the removed boundaryless side has positive genus. This contradicts minimal genus. Its boundary therefore bounds a disk in $F$. Replace that disk by a small push-off of $D$, removing the intersection [circle](../../../topology.md#circle) without changing genus or boundary, again contradicting minimal intersection. Thus no [circles](../../../topology.md#circle) remain.

Cutting $F$ along its single intersection arc gives two connected [surfaces](../../../topology.md#topological-surface) with boundaries the two summand [knots](../../../knot-theory.md#knot) after the closing arcs are added. [Euler characteristic](../../../homology.md#euler-characteristic) shows that their genera add to $g(F)$. Each genus is at least the minimum genus of its summand, so

$$
\boxed{g_s(K_1\#K_2)=g_s(K_1)+g_s(K_2).}
$$

Genus zero means that the [knot](../../../knot-theory.md#knot) bounds a disk and is the [unknot](../../../knot-theory.md#unknot). Every nontrivial [knot](../../../knot-theory.md#knot) therefore has positive genus. Induct on this nonnegative integer: a nontrivial nonprime [knot](../../../knot-theory.md#knot) splits into two nontrivial summands, each with strictly smaller genus by the equality above, and induction decomposes both into primes. This proves **every [knot](../../../knot-theory.md#knot) is a finite connected sum of [prime knots](../../../knot-theory.md#prime-knot)**, with the [unknot](../../../knot-theory.md#unknot) the empty sum.

The same induction does not follow from the three suggested replacements. For [crossing number of a knot](../../../knot-theory.md#crossing-number-of-a-knot), joining minimal diagrams gives only subadditivity; a reverse inequality giving strict descent for every nontrivial summand is not provided by this argument. The [Jones polynomial of a connected sum](../../../knot-theory.md#jones-polynomial-of-a-connected-sum) does make its [breadth of a Laurent polynomial](../../../polynomial.md#breadth-of-a-laurent-polynomial) additive, but the needed implication that zero breadth forces the [unknot](../../../knot-theory.md#unknot) is the [Jones unknot detection problem](../../../knot-theory.md#jones-unknot-detection-problem). For the [Alexander polynomial](../../../knot-theory.md#alexander-polynomial), even this implication is false: nontrivial untwisted [Whitehead doubles](../../../knot-theory.md#whitehead-double) have [Alexander polynomial](../../../knot-theory.md#alexander-polynomial) one and hence breadth zero. The decisive genus property is both additivity and the exact characterization $g_s(K)=0$ if and only if $K$ is the [unknot](../../../knot-theory.md#unknot).

For uniqueness use complete [decomposing sphere systems for a knot](../../../knot-theory.md#decomposing-sphere-system-for-a-knot). Cut each system and cap the marked boundary [spheres](../../../geometry-and-topology.md#sphere) with straight arcs; the resulting oriented factors are [prime knots](../../../knot-theory.md#prime-knot). Compare two systems in transverse position, and use the [prime-ball exchange lemma](../../../knot-theory.md#prime-ball-exchange-lemma) to simplify their intersection. Choose an innermost intersection [circle](../../../topology.md#circle) bounding a disk in a sphere of one system and lying in a prime-factor ball of the other. If the disk misses the knotted arc it cuts off an empty ball. If it meets the arc once it cuts the prime factor into two [knots](../../../knot-theory.md#knot), so one is an [unknot](../../../knot-theory.md#unknot). Replace the old ball by the side carrying the same prime factor, perturb its boundary slightly, and remove that intersection circle. This preserves the unordered factors: the discarded empty or trivial ball merely changes the joining arc, and any intervening capped boundaries still carry their original factors. If the chosen disk contains both marked points, take another innermost disk without marked points, or the complementary disk when the intersection circle is the only one.

Iteration yields an innermost prime-factor ball disjoint from both systems. Its arc has no nontrivial further decomposition, so it represents one factor in each. The boundary can be included in both systems using the same ball exchange; replace its arc by a straight boundary arc and remove this common factor. Induction on the number of factors matches the remaining factors. When the systems already have no intersections, start directly with an innermost ball and the same removal step. All replacements preserve the arc [orientation](../../../algebraic-topology.md#orientation-of-a-simplex), so the match is of oriented [knots](../../../knot-theory.md#knot), not only unoriented types. Hence the [prime decomposition of knots](../../../knot-theory.md#prime-decomposition-of-knots) is unique up to reordering and oriented [link isotopy](../../../knot-theory.md#link-isotopy).

## 3

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $F$ be an oriented [Seifert surface](../../../knot-theory.md#seifert-surface) of [genus](../../../topology.md#genus-of-a-surface) $g$ for $K$, and choose a basis $a_1,\ldots,a_{2g}$ of $H_1(F;\mathbb Z)$. Push a representative curve slightly in the positive normal direction to obtain $a_i^+$. The [Seifert matrix](../../../knot-theory.md#seifert-matrix) in our row convention is

$$
V_{ij}=\operatorname{lk}(a_i^+,a_j).
$$

The difference $V-V^T$ is the [intersection form](../../../homology.md#intersection-form) of F, up to the convention for its [orientation](../../../algebraic-topology.md#orientation-of-a-simplex); in a symplectic basis it is a direct sum of unimodular two-by-two skew blocks.

Write $X=S^3\setminus\operatorname{int}N(K)$ for the [knot exterior](../../../knot-theory.md#knot-exterior). Linking number with K gives the epimorphism $\pi_1(X)\to\mathbb Z$ sending a positive meridian to one. Let $\widetilde X$ be the associated [infinite cyclic cover](../../../knot-theory.md#infinite-cyclic-cover-of-a-knot-exterior), with [deck transformation](../../../algebraic-topology.md#deck-transformation) t. The [Alexander module of a knot](../../../knot-theory.md#alexander-module-of-a-knot) is $\mathcal A_K=H_1(\widetilde X;\mathbb Z)$, regarded as a [module](../../../module-theory.md#module-mathematics) over the [Laurent polynomial ring](../../../commutative-algebra.md#laurent-polynomial-ring) $\Lambda=\mathbb Z[t,t^{-1}]$. Its order, the greatest common divisor of the maximal presentation minors, is the [Alexander polynomial of a knot](../../../knot-theory.md#alexander-polynomial), defined up to $\pm t^k$. Equivalently these minors generate its zeroth [Fitting ideal](../../../module-theory.md#fitting-ideal); we will obtain a square presentation, so its [determinant](../../../linear-algebra.md#determinant) gives the order. No assertion that $\Lambda$ is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain) is needed.

Here is the [Seifert-matrix presentation of the Alexander module](../../../knot-theory.md#seifert-matrix-presentation-of-the-alexander-module) with its topological justification. Cut X along F, obtaining a connected manifold Y with two boundary copies $F^+$ and $F^-$. Up to collars this is the complement of a thickening of F in $S^3$. [Alexander duality](../../../cohomology.md#alexander-duality) gives $H_1(Y;\mathbb Z)\cong\mathbb Z^{2g}$ and the perfect linking pairing with $H_1(F;\mathbb Z)$. Choose generators $b_j$ satisfying $\operatorname{lk}(b_j,a_i)=\delta_{ij}$. This [homology](../../../homology.md) statement does not require Y to be a handlebody. The two inclusions satisfy

$$
i_+(a_i)=\sum_jV_{ij}b_j,\qquad i_-(a_i)=\sum_jV_{ji}b_j.
$$

Indeed the first coefficients are the defining positive [linking numbers](../../../knot-theory.md#linking-number); for the second, moving the two curves to opposite sides and using symmetry of linking gives $\operatorname{lk}(a_i^-,a_j)=\operatorname{lk}(a_j^+,a_i)$.

Stack copies of Y, identifying the positive copy of F in one layer with the negative copy in the next. This is $\widetilde X$. The [Mayer–Vietoris sequence](../../../algebraic-topology.md#mayer-vietoris-sequence), with all translates collected into Laurent [modules](../../../module-theory.md#module-mathematics), contains

$$
H_1(F)\otimes\Lambda\xrightarrow{\,t i_+-i_-\,}H_1(Y)\otimes\Lambda\longrightarrow\mathcal A_K\longrightarrow H_0(F)\otimes\Lambda\xrightarrow{\,t-1\,}H_0(Y)\otimes\Lambda.
$$

The last map is injective because $\Lambda$ is an [integral domain](../../../commutative-algebra.md#integral-domain). Thus the entire [Alexander module](../../../knot-theory.md#alexander-module-of-a-knot) is presented by the row relations $tV-V^T$ (transpose the [matrix](../../../vector-space.md#matrix) if using column vectors). At $t=1$ its [determinant](../../../linear-algebra.md#determinant) is $\det(V-V^T)=1$, so the [determinant](../../../linear-algebra.md#determinant) is nonzero and the [module](../../../module-theory.md#module-mathematics) is a [torsion module](../../../module-theory.md#torsion-module). Consequently

$$
\boxed{\Delta_K(t)\doteq\det(tV-V^T),\qquad\operatorname{br}\Delta_K\leq2g_s(K),}
$$

where $\doteq$ denotes equality up to a [Laurent unit](../../../commutative-algebra.md#unit-of-a-laurent-polynomial-ring). The second conclusion follows because a [determinant](../../../linear-algebra.md#determinant) of size $2g$ with entries linear in t has breadth at most $2g$; minimize over [Seifert surfaces](../../../knot-theory.md#seifert-surface).

For the displayed diagram, start on the outer lower arc near the lower left undercrossing and follow the arc through the lower outer loop toward the upper right undercrossing. Number successive undercrossings $0,\ldots,9$, and let $x_i$ label the incoming arc at crossing $i$. Reading the overpassing arcs and the conjugation exponents in a consistent meridian convention gives

$$
(o_0,\ldots,o_9)=(6,0,7,6,9,1,3,0,4,8),\qquad(\varepsilon_0,\ldots,\varepsilon_9)=(-1,1,-1,-1,-1,-1,-1,-1,-1,-1).
$$

Thus the [Wirtinger presentation](../../../knot-theory.md#wirtinger-presentation) relations are $x_{i+1}=x_{o_i}^{\varepsilon_i}x_ix_{o_i}^{-\varepsilon_i}$, with indices modulo ten. Their [Fox derivatives](../../../geometric-group-theory.md#fox-derivative) after [abelianization](../../../group-theory.md#abelianization) give row relations

$$
t^{\varepsilon_i}z_i-z_{i+1}+(1-t^{\varepsilon_i})z_{o_i}=0.
$$

Delete the redundant last relation and the last column, setting $z_9=0$. This is a nine-generator presentation of the [Alexander module](../../../knot-theory.md#alexander-module-of-a-knot). The cofactor [determinant](../../../linear-algebra.md#determinant) is $t^{-6}(t^4+t^3-3t^2+t+1)$; here is a smaller elimination check. Retain $z_1,z_4$. Seven relations solve the other generators as

$$
\begin{aligned}
z_8&=(1-t)z_4,&z_5&=t^{-1}z_4,&z_6&=t^{-2}z_4+(1-t^{-1})z_1,\\
z_0&=tz_1-(t-1)z_6,&z_2&=tz_1+(1-t)z_0,&z_3&=tz_4-(t-1)z_6,\\
z_7&=t^{-1}z_6+(1-t^{-1})z_3.
\end{aligned}
$$

The two remaining rows, at undercrossings two and seven, are the [matrix](../../../vector-space.md#matrix)

$$
N=\begin{pmatrix}(t^2-t+1)/t^2&-(2t^3-2t^2+1)/t^3\\(t^2-1)/t^2&(t^4-2t^2+t+1)/t^3\end{pmatrix}.
$$

Its [determinant](../../../linear-algebra.md#determinant) is $t^{-3}(t^4+t^3-3t^2+t+1)$, differing from the original cofactor only by a [Laurent unit](../../../commutative-algebra.md#unit-of-a-laurent-polynomial-ring). Consequently

$$
\boxed{\Delta_K(t)\doteq t^4+t^3-3t^2+t+1.}
$$

The factor has value one at $t=1$ and is reciprocal, as required. Its [Conway-normalized Alexander polynomial](../../../knot-theory.md#conway-normalized-alexander-polynomial) is $t^2+t-3+t^{-1}+t^{-2}$, and its [knot determinant](../../../knot-theory.md#knot-determinant) is three.

For the genus upper bound, the over/under [Gauss code](../../../knot-theory.md#gauss-code) from the same traversal is

$$
7_O\ 1_O\ 0_U\ 5_O\ 1_U\ 2_U\ 6_O\ 3_U\ 8_O\ 4_U\ 5_U\ 0_O\ 3_O\ 6_U\ 2_O\ 7_U\ 9_O\ 8_U\ 4_O\ 9_U.
$$

Number these visits $0,\ldots,19$. The [oriented smoothing permutation of a Gauss code](../../../knot-theory.md#oriented-smoothing-permutation-of-a-gauss-code) has cycles

$$
(0,16),\ (1,5,15),\ (2,12,8,18,10,4),\ (3,11),\ (6,14),\ (7,13),\ (9,19,17).
$$

There are seven [Seifert circles](../../../knot-theory.md#seifert-circle), so the [Seifert algorithm](../../../knot-theory.md#seifert-algorithm) gives ten bands and seven disks: $1-2g=7-10$, hence $g=2$. The [Alexander breadth bound on Seifert genus](../../../knot-theory.md#alexander-breadth-bound-on-seifert-genus) supplies the matching lower bound from breadth four. Therefore $\boxed{g_s(K)=2}$.

Modulo two, the primitive Alexander [polynomial](../../../polynomial.md) becomes $t^4+t^3+t^2+t+1$. It has neither zero nor one as a root, and it is not $(t^2+t+1)^2=t^4+t^2+1$, the only possible product of irreducible monic quadratics over $\mathbb F_2$. It is therefore irreducible over $\mathbb F_2$, hence over $\mathbb Q$ and $\mathbb Z$ by [Gauss lemma for polynomials](../../../commutative-algebra.md#gauss-lemma-for-polynomials). The [full-degree irreducible Alexander polynomial implies a prime knot](../../../knot-theory.md#full-degree-irreducible-alexander-polynomial-implies-a-prime-knot) criterion now applies, since its breadth is exactly twice the genus. Thus **the knot is prime**. The full-degree condition is needed to rule out a nontrivial summand with unit [Alexander polynomial](../../../knot-theory.md#alexander-polynomial).

To test reflection, calculate the [Jones polynomial](../../../knot-theory.md#jones-polynomial) from the same crossing data. The diagram has nine positive crossings and one negative crossing, so its [writhe of a link diagram](../../../knot-theory.md#writhe-of-a-link-diagram) is eight. Enumerate the $2^{10}$ [bracket smoothing states](../../../knot-theory.md#bracket-smoothing-state), join their smoothed ends, and weight each state by $A^{a-b}(-A^2-A^{-2})^{s-1}$. Correct by $(-A^3)^{-8}$ and put $t=A^{-4}$. This gives

$$
\boxed{V_K(t)=t^2+t^7-t^8+t^9-t^{10}.}
$$

As checks, $V_K(1)=1$ and $V_K(-1)=-3=\Delta_K(-1)$. The [Jones polynomial of a mirror](../../../knot-theory.md#jones-polynomial-of-a-mirror) is $V_K(t^{-1})$, which differs from this [polynomial](../../../polynomial.md). Therefore **the knot is not equivalent to its reflection**. Reversing all crossing conventions reciprocates the displayed [Jones polynomial](../../../knot-theory.md#jones-polynomial) and leaves the conclusion unchanged.

<a id="3/image-jones-polynomial-coefficients-of-the-knot-and-its-mirror-occupy-different-exponent-ranges"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-19-jones-reflection.png)

**[Figure 1](#3/image-jones-polynomial-coefficients-of-the-knot-and-its-mirror-occupy-different-exponent-ranges). Jones polynomial coefficients of the knot and its mirror occupy different exponent ranges**.

## 4

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Wirtinger presentation](../../../knot-theory.md#wirtinger-presentation) assigns a meridian generator to each arc between undercrossings. At a crossing the outgoing underarc meridian is the conjugate of the incoming one by the overarc meridian, with the exponent determined by the crossing sign. One crossing relation is redundant for a connected [knot](../../../knot-theory.md#knot) diagram. This gives a presentation of the [knot group](../../../knot-theory.md#knot-group), the [fundamental group](../../../algebraic-topology.md#fundamental-group) of its exterior.

For the [trefoil knot](../../../knot-theory.md#trefoil-knot), choose three arcs x,y,z so that two crossing relations are $z=xyx^{-1}$ and $x=yzy^{-1}$. The third follows from these. Substituting for z gives $xyx=yxy$, hence

$$
\boxed{\pi_1(S^3\setminus T)=\langle x,y\mid xyx=yxy\rangle.}
$$

We use the relator $r=xyxy^{-1}x^{-1}y^{-1}$.

Here is the [Fox free differential calculus](../../../geometric-group-theory.md#fox-calculus), including its connection with the covering-space chain complex. Let F be the [free group](../../../geometric-group-theory.md#free-group) on $x_1,\ldots,x_n$, let $\mathbb ZF$ be its [group ring](../../../commutative-algebra.md#group-ring), and let $\varepsilon:\mathbb ZF\to\mathbb Z$ be augmentation. Define additive maps $D_j:\mathbb ZF\to\mathbb ZF$ by

$$
D_j(x_i)=\delta_{ij},\qquad D_j(ab)=D_j(a)\varepsilon(b)+aD_j(b),\qquad D_j(1)=0.
$$

For [group](../../../group.md) words u,v the product rule reads $D_j(uv)=D_j(u)+uD_j(v)$. Differentiating $x_ix_i^{-1}=1$ forces $D_j(x_i^{-1})=-\delta_{ij}x_i^{-1}$. Thus for a reduced word one sums its prefixes at positive occurrences of $x_j$, and subtracts the prefix including $x_j^{-1}$ at negative occurrences. Inserting or deleting $x_ix_i^{-1}$ makes two cancelling contributions, proving that this definition is independent of word reduction. Linear extension proves the group-ring product rule and uniqueness.

The fundamental identity is

$$
w-1=\sum_{j=1}^nD_j(w)(x_j-1).
$$

It holds on generators and inverses. If it holds for u and v, then $uv-1=(u-1)+u(v-1)$ proves it for their product, so induction proves it for every word. These [Fox derivatives](../../../geometric-group-theory.md#fox-derivative) form the [matrix](../../../vector-space.md#matrix) $\big(D_jr_i\big)_{i,j}$ for any chosen presentation.

Let $\phi:G\to\mathbb Z$ be knot-group [abelianization](../../../group-theory.md#abelianization) and put $a_j=\phi(x_j)$. Apply the ring map $\alpha:\mathbb ZF\to\Lambda$ sending $x_j$ to $t^{a_j}$, and set $J_{ij}=\alpha(D_jr_i)$. Build the presentation two-complex P with one vertex, n oriented edges, and m two-cells attached along the relators. Its [infinite cyclic cover](../../../knot-theory.md#infinite-cyclic-cover-of-a-knot-exterior) has [cellular chain complex](../../../homology.md#cellular-chain-complex)

$$
\Lambda^m\xrightarrow{\,J^T\,}\Lambda^n\xrightarrow{\,d_1\,}\Lambda,\qquad d_1(e_j)=t^{a_j}-1.
$$

To verify the second boundary, lift an attaching word starting at deck level zero. An occurrence $x_j$ after prefix u traverses the jth edge at level $\phi(u)$, contributing $t^{\phi(u)}e_j$. An occurrence $x_j^{-1}$ traverses it backwards starting at level $\phi(ux_j^{-1})$, contributing $-t^{\phi(ux_j^{-1})}e_j$. Their sum is exactly the evaluated Fox derivative. The fundamental identity, with $\alpha(r_i)=1$, gives $d_1J^T=0$.

The cover of P and the cover of the [knot exterior](../../../knot-theory.md#knot-exterior) both have [fundamental group](../../../algebraic-topology.md#fundamental-group) $\ker\phi$. Their first [homology](../../../homology.md) is the [abelianization](../../../group-theory.md#abelianization) of that [group](../../../group.md), with the same deck action induced by conjugation. Thus no assumption that the presentation complex is aspherical is needed, and the complete relation with the [Alexander module of a knot](../../../knot-theory.md#alexander-module-of-a-knot) is

$$
\boxed{\mathcal A_K\cong\ker d_1/\operatorname{im}J^T.}
$$

For meridian generators all $a_j=1$. Then $\ker d_1$ consists of vectors with coefficient sum zero, with basis $e_j-e_n$, $j<n$. Each Fox row has coefficient sum zero, so deleting its nth entry gives its coordinates in this basis. Deleting one column of J therefore presents the [Alexander module](../../../knot-theory.md#alexander-module-of-a-knot); if a Wirtinger relator is redundant it can also be deleted. This proves the [matrix](../../../vector-space.md#matrix) procedure used for the displayed [knot](../../../knot-theory.md#knot) above. For arbitrary generators, the exponent vector is primitive because the generators map onto $\mathbb Z$; elementary changes of free generators implement the Euclidean algorithm and reduce it to $(1,0,\ldots,0)$. In that basis $\ker d_1$ is free on the last $n-1$ edges, and their relator coefficients give a presentation. This explains the general case rather than treating the full Fox cokernel as the [Alexander module](../../../knot-theory.md#alexander-module-of-a-knot).

For the trefoil relator, with $\alpha(x)=\alpha(y)=t$, direct differentiation gives

$$
\alpha(D_xr)=1-t+t^2=f(t),\qquad\alpha(D_yr)=t-t^2-1=-f(t).
$$

The first boundary is $(t-1,t-1)$, whose kernel is generated by $(1,-1)$. The relator boundary is $f(t)(1,-1)$, whence

$$
\boxed{\mathcal A_T\cong\Lambda/(t^2-t+1),\qquad\Delta_T(t)\doteq t^2-t+1.}
$$

For a [connected sum of knots](../../../knot-theory.md#connected-sum-of-knots), join [Seifert surfaces](../../../knot-theory.md#seifert-surface) in separated balls. Their [Seifert matrix](../../../knot-theory.md#seifert-matrix) is block diagonal, so the [Alexander module of a connected sum](../../../knot-theory.md#alexander-module-of-a-connected-sum) is a direct sum. Thus $\mathcal A_{T\#T}\cong(\Lambda/(f))^2$.

This [module](../../../module-theory.md#module-mathematics) is not cyclic. The [polynomial](../../../polynomial.md) f is irreducible modulo two, since it has no root in $\mathbb F_2$, so $\mathfrak m=(2,f)$ is a [maximal ideal](../../../commutative-algebra.md#maximal-ideal) of $\Lambda$ with [residue field](../../../commutative-algebra.md#residue-field) $\mathbb F_4$. The quotient $\mathcal A_{T\#T}/\mathfrak m\mathcal A_{T\#T}$ has dimension two over that field, whereas the corresponding quotient of a [cyclic module](../../../module-theory.md#cyclic-module) has dimension at most one.

Every two-generator [knot group](../../../knot-theory.md#knot-group), however, has a cyclic [Alexander module](../../../knot-theory.md#alexander-module-of-a-knot), regardless of its number of relators. Indeed its primitive [abelianization](../../../group-theory.md#abelianization) vector can be changed to $(1,0)$ as above. The covering boundary is then $(t-1,0)$; its kernel is the free rank-one [module](../../../module-theory.md#module-mathematics) on the second edge, and any quotient by lifted relators is cyclic. This proves the [two-generator knot groups have cyclic Alexander modules](../../../knot-theory.md#two-generator-knot-groups-have-cyclic-alexander-modules) obstruction. Consequently **the [group](../../../group.md) of the connected sum of two trefoils cannot even be generated by two elements**, and in particular it has no two-generator, one-relator presentation.

## 5

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For an oriented three-manifold M with prescribed framed boundary endpoints P, the [relative Kauffman bracket skein module](../../../knot-theory.md#relative-kauffman-bracket-skein-module) is the complex vector space generated by properly embedded framed [tangles](../../../knot-theory.md#tangle), modulo framed [isotopy](../../../differential-geometry.md#isotopy) and the local bracket relations. A crossing resolves with coefficients A and $A^{-1}$, and adjoining an unknotted [circle](../../../topology.md#circle) multiplies by $\delta=-A^2-A^{-2}$. We now use the full bracket convention: the empty diagram has value one and a [circle](../../../topology.md#circle) has value $\delta$. For a nonempty uncolored [link](../../../knot-theory.md#link) this full bracket is $\delta$ times the reduced bracket used earlier. Fixing this normalization is essential for the [quantum dimensions](../../../category-theory.md#quantum-dimension). Gluing compatible boundary pieces composes skeins; disjoint union gives [tensor products](../../../linear-algebra.md#tensor-product). With no endpoints this is the [Kauffman bracket skein module](../../../knot-theory.md#kauffman-bracket-skein-module). Framing is retained, so a Reidemeister-I curl is a framing change rather than an allowed [isotopy](../../../differential-geometry.md#isotopy).

For $A\ne0$, the [Temperley-Lieb algebra](../../../knot-theory.md#temperley-lieb-diagram-algebra) $\mathrm{TL}_n(A)$ is the skein algebra of a rectangle cylinder with n marked endpoints on each horizontal side, multiplication being vertical stacking. Resolve crossings to get a basis of crossing-free matchings of its $2n$ endpoints, with every closed [circle](../../../topology.md#circle) removed with factor $\delta$. There are $\frac1{n+1}\binom{2n}{n}$ such matchings. Conversely multiplication of these matchings by joining endpoints defines an algebra satisfying the skein relations, which proves their independence. Writing $e_i$ for an adjacent cap-cup and 1 for the n vertical strands gives

$$
e_i^2=\delta e_i,\qquad e_ie_{i\pm1}e_i=e_i,\qquad e_ie_j=e_je_i\quad(|i-j|>1).
$$

Every crossing-free matching other than 1 contains a turnback; removing an outermost cap successively expresses it in these generators. Thus these diagram rules give the usual generator presentation as well.

Put $[m]=(A^{2m}-A^{-2m})/(A^2-A^{-2})$, interpreted as the Laurent sum $\sum_{s=0}^{m-1}A^{2(m-1-2s)}$ if its denominator vanishes. Set $\Delta_j=(-1)^j[j+1]$. These [quantum integers](../../../algebra.md#quantum-integer) satisfy $\Delta_0=1$, $\Delta_1=\delta$, and $\Delta_j=\delta\Delta_{j-1}-\Delta_{j-2}$. The [Jones-Wenzl idempotent](../../../knot-theory.md#jones-wenzl-idempotent) $f_n$ is characterized by identity-matching coefficient one and

$$
f_n^2=f_n,\qquad e_if_n=f_ne_i=0\quad(1\leq i<n).
$$

Starting with $f_0=1$, $f_1=1$, set $F=f_{n-1}\otimes1$ and $C=Fe_{n-1}F$. Whenever the denominators are nonzero the recursion is

$$
\boxed{f_n=F-\frac{\Delta_{n-2}}{\Delta_{n-1}}C.}
$$

Here is the induction proving its properties. Closing the last strand of $f_{n-1}$ gives $(\Delta_{n-1}/\Delta_{n-2})f_{n-2}$. Consequently stacking two copies of C, and straightening the middle cap-cup, gives $C^2=\mu C$, where $\mu=\Delta_{n-1}/\Delta_{n-2}$. Also $FC=CF=C$. Expanding $(F-\mu^{-1}C)^2$ proves [idempotence](../../../algebra.md#idempotence). The earlier turnbacks are killed by F; the last is killed because the same cap-cup calculation gives $Ce_{n-1}=\mu Fe_{n-1}$ and its reflected identity. Only F contributes to the identity matching, with coefficient one.

For completeness, the partial-closure formula used in that induction follows from the recursion itself. Closing the last strand of F gives $\delta f_{n-1}$; closing the last strand of C straightens its cap-cup to $f_{n-1}$. Hence partial closure of $f_n$ is $(\delta-\Delta_{n-2}/\Delta_{n-1})f_{n-1}=(\Delta_n/\Delta_{n-1})f_{n-1}$. Starting at $f_1$, this proves both the inductive formula and total closure $\operatorname{tr}(f_n)=\Delta_n$. Finally, any nonidentity matching is in the turnback ideal. If two normalized projectors kill that ideal, multiplying them gives each of them, proving uniqueness. Their normalization also gives absorption of smaller projectors on consecutive substrands. At exceptional A one must check the denominators; the recursion does not assert existence of every projector there.

A positive framing twist of an n-strand projected cable consists of n individual positive curls and $n(n-1)$ positive braid crossings. Each curl contributes $-A^3$. A crossing is $A1+A^{-1}e_i$, so it acts on $f_n$ as A because the turnback vanishes. This proves the depicted [Jones-Wenzl twist eigenvalue](../../../knot-theory.md#jones-wenzl-twist-eigenvalue) identity, including its exponent:

$$
\boxed{\theta_n f_n=(-1)^nA^{n(n+2)}f_n.}
$$

A negative framing twist acts by the inverse scalar.

Choose $A=e^{\pi i/(2r)}$, with an integer $r\geq3$. Then $[r]=0$ but $[1],\ldots,[r-1]$ are nonzero. The projector $f_{r-1}$ exists and has trace zero. Pass to the [reduced Temperley-Lieb skein theory](../../../knot-theory.md#reduced-temperley-lieb-skein-theory) by setting it to zero, including every diagram containing it. The surviving colors are $j=0,\ldots,r-2$, with dimensions and twists

$$
d_j=\Delta_j=(-1)^j\frac{\sin((j+1)\pi/r)}{\sin(\pi/r)},\qquad\theta_j=(-1)^jA^{j(j+2)}.
$$

Their dimensions are nonzero. The recurrence decomposes $f_j\otimes1$ into the two orthogonal channels $f_{j+1}$ and $f_{j-1}$: the first is the new projector, while its complementary cap-cup [idempotent](../../../commutative-algebra.md#idempotent) is the latter, with inclusion/projection normalized by the nonzero partial-closure scalar. At the upper endpoint the $r-1$ channel vanishes. Iterating gives a complete decomposition of every tensor power into these colors. A matching between projected colors of different sizes has a turnback on the larger side and vanishes; on the same size only the identity matching survives. Thus their endomorphism spaces are one-dimensional and all [matrix](../../../vector-space.md#matrix) blocks split. Applying the recurrence to the decompositions proves the [fusion of Jones-Wenzl colors](../../../knot-theory.md#fusion-of-jones-wenzl-colors) rule

$$
a\otimes b=\bigoplus_cN_{ab}^c c,\qquad N_{ab}^c=\begin{cases}1,&a+b+c\text{ even},\ |a-b|\leq c\leq\min(a+b,2r-4-a-b),\\0,&\text{otherwise}.\end{cases}
$$

One can verify the induction by multiplying by color 1: both sides satisfy the same adjacent-color recurrence and the same zero boundary at $r-1$. Taking closures proves $d_ad_b=\sum_cN_{ab}^cd_c$. Cups and caps make every color self-dual, so these fusion coefficients are symmetric in all three labels.

We next prove the [Kirby color handle-slide identity](../../../knot-theory.md#kirby-color-handle-slide-identity), rather than assume it. In the annular skein space let $\widehat f_b$ be the closure of color b and define the [Kirby color](../../../knot-theory.md#kirby-color) $\Omega=\sum_bd_b\widehat f_b$. For a fixed color a, choose inclusion/projection maps $i_c:c\to b\otimes a$, $p_c:b\otimes a\to c$ for the fusion channels, with $p_ci_c=1_c$ and $\sum_ci_cp_c=1_{b\otimes a}$. Bend the a strand with a cup and cap, obtaining

$$
U_c^b=(p_c\otimes1_a)(1_b\otimes\operatorname{coev}_a):b\longrightarrow c\otimes a,\qquad V_c^b=(1_b\otimes\operatorname{ev}_a)(i_c\otimes1_a):c\otimes a\longrightarrow b.
$$

Closing the resulting diagrams and straightening the bent strand gives $\operatorname{tr}(V_c^bU_c^b)=\operatorname{tr}(p_ci_c)=d_c$. Since b is simple, $V_c^bU_c^b=(d_c/d_b)1_b$. The symmetric fusion rule supplies all channels of $c\otimes a$, so their normalized projections are complete. Therefore

$$
\sum_b\frac{d_b}{d_c}U_c^bV_c^b=1_{c\otimes a},\qquad\boxed{\sum_bd_bU_c^bV_c^b=d_c1_{c\otimes a}.}
$$

To slide an a-colored strand over an $\Omega$-colored component, cut at the slide band and insert the resolution $\sum_ci_cp_c$. Carrying the band across that loop bends its two maps into U and V. In each outgoing channel c, the boxed identity replaces the sum over the old loop color b by exactly the new loop weight $d_c$; the rest of the diagrams are isotopic as framed ribbons. This proves invariance for fixed a. Summing a with its own weight proves invariance when both surgery components are colored by $\Omega$. The band framing is carried in this argument, as required for a framed [handle slide](../../../topology.md#handle-slide).

We must also show that the stabilization normalization is nonzero. Let $H_{ij}$ be the full bracket of the zero-framed [Hopf link](../../../knot-theory.md#hopf-link) with colors i,j. On a fusion channel k, its double braiding has eigenvalue $\theta_k/(\theta_i\theta_j)$: the full twist of the combined ribbon equals double braiding followed by the two separate twists. Taking the trace gives the balancing identity

$$
H_{ij}=\frac1{\theta_i\theta_j}\sum_kN_{ij}^kd_k\theta_k.
$$

For $j=1$ there are only the $i-1,i+1$ channels; substitution of their dimensions and twists gives $H_{i1}/d_i=-(A^{2i+2}+A^{-2i-2})$, with a vanished endpoint channel simply omitted. A color-1 meridian therefore acts on the simple color i by that scalar. The annular closures obey $\widehat f_j=X\widehat f_{j-1}-\widehat f_{j-2}$, where X is a color-1 core, by the two-channel fusion decomposition. Applying this recurrence to meridians gives the [Hopf pairing of Jones-Wenzl colors](../../../knot-theory.md#hopf-pairing-of-jones-wenzl-colors)

$$
H_{ij}=(-1)^{i+j}[(i+1)(j+1)].
$$

Indeed the recurrence is the sine identity $\sin((j+1)x)=2\cos x\sin(jx)-\sin((j-1)x)$ with $x=(i+1)\pi/r$, and its initial values are $H_{i0}=d_i$ and the computed $H_{i1}$. Finite sine orthogonality now gives

$$
H^2=\mathcal D^2I,\qquad\mathcal D^2=\sum_jd_j^2=\frac{r}{2\sin^2(\pi/r)},\qquad\mathcal D>0.
$$

For example, orthogonality follows by writing products of sines as differences of cosines and summing the finite geometric series of rth roots of unity; the result is $\sum_{k=1}^{r-1}\sin(ik\pi/r)\sin(jk\pi/r)=\frac r2\delta_{ij}$. Thus no degeneracy remains in this pairing.

The [Gauss sums of Jones-Wenzl colors](../../../knot-theory.md#gauss-sums-of-jones-wenzl-colors) are $p_\pm=\sum_jd_j^2\theta_j^{\pm1}$, the evaluations of the plus- and minus-one-framed $\Omega$-colored unknots. Balancing and dimension fusion prove

$$
\sum_id_i\theta_iH_{ij}=\theta_j^{-1}\sum_{i,k}d_iN_{ij}^kd_k\theta_k=p_+\theta_j^{-1}d_j.
$$

In the last step $\sum_id_iN_{ij}^k=d_jd_k$, by symmetry of the fusion coefficients. In vector notation this is $HTd=p_+T^{-1}d$, with $T=\operatorname{diag}(\theta_j)$. The [matrix](../../../vector-space.md#matrix) $H$ and [vector](../../../vector-space.md#vector) $d$ are real, and each twist has modulus one, so conjugation gives $HT^{-1}d=p_-Td$. Apply H again and use its orthogonality to obtain $\boxed{p_+p_-=\mathcal D^2}$. Hence neither factor vanishes.

We may use the surgery existence theorem and [Kirby calculus](../../../knot-theory.md#kirby-calculus): every closed oriented three-manifold has an integral framed-link surgery description, and two descriptions are related by [handle slides](../../../topology.md#handle-slide) and insertion/removal of disjoint plus- or minus-one-framed unknots. For an m-component surgery [link](../../../knot-theory.md#link) L let $\sigma(L)$ be the [signature](../../../linear-algebra.md#signature-of-a-quadratic-form) of its symmetric [surgery linking matrix](../../../knot-theory.md#surgery-linking-matrix), put $\kappa=p_+/\mathcal D$, and define the [Jones polynomial surgery invariant](../../../knot-theory.md#jones-polynomial-surgery-invariant)

$$
\boxed{\tau_r(M_L)=\mathcal D^{-m}\kappa^{-\sigma(L)}\langle L(\Omega,\ldots,\Omega)\rangle.}
$$

A [handle slide](../../../topology.md#handle-slide) preserves the colored bracket by the proved identity and changes the linking [matrix](../../../vector-space.md#matrix) by congruence, preserving its [signature](../../../linear-algebra.md#signature-of-a-quadratic-form). Adding a disjoint plus-one-framed [unknot](../../../knot-theory.md#unknot) multiplies the bracket by $p_+$ and changes $(m,\sigma)$ to $(m+1,\sigma+1)$, so the net factor is $p_+/(\mathcal D\kappa)=1$. For a minus-one-framed [unknot](../../../knot-theory.md#unknot) it is $\kappa p_-/\mathcal D=p_+p_-/\mathcal D^2=1$. [Kirby calculus](../../../knot-theory.md#kirby-calculus) therefore proves that the displayed value is a well-defined oriented three-manifold invariant. Our normalization has $\tau_r(S^3)=1$; reversing [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) conjugates the value. Its construction uses precisely the bracket and colored projectors underlying the [Jones polynomial](../../../knot-theory.md#jones-polynomial).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
