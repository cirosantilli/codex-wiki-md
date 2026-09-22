<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $\delta=-A^2-A^{-2}$. The reduced [Kauffman bracket](../../../../../kauffman-bracket.md) is the [Laurent polynomial](../../../../../laurent-polynomial.md) determined by $\langle\bigcirc\rangle=1$, $\langle D\sqcup\bigcirc\rangle=\delta\langle D\rangle$, and the crossing expansion $\langle D\rangle=A\langle D_A\rangle+A^{-1}\langle D_B\rangle$. Fix the A smoothing so that a positive curl has multiplier $-A^3$; rotating the local crossing interchanges the smoothing descriptions. Equivalently, its [bracket smoothing states](../../../../../bracket-smoothing-state.md) give

$$
\boxed{\langle D\rangle=\sum_sA^{a(s)-b(s)}\delta^{|s|-1},}
$$

where $a(s)$ and $b(s)$ count its A and B smoothings and $|s|$ is the number of state [circles](../../../../../circle.md). Resolving all crossings proves that the recursive rules define the same [polynomial](../../../../../polynomial-split.md) independently of the order of expansion.

Under a positive [Reidemeister move](../../../../../reidemeister-move.md) of type I, the two resolutions give $A\delta+A^{-1}=-A^3$ times the straight strand; the negative curl gives $A^{-1}\delta+A=-A^{-3}$. Thus the bracket itself is not an unframed [link invariant](../../../../../link-invariant.md). For type II, use the adjacent cap-cup generator $e$ of the [Temperley-Lieb algebra](../../../../../temperley-lieb-diagram-algebra.md), with $e^2=\delta e$. The crossing and its inverse are $R=A1+A^{-1}e$ and $R^{-1}=A^{-1}1+Ae$, and

$$
RR^{-1}=1+(A^2+A^{-2}+\delta)e=1.
$$

For type III, $e_ie_{i+1}e_i=e_i$ and the analogous reversed relation give

$$
R_iR_{i+1}R_i-R_{i+1}R_iR_{i+1}=A^{-1}(A^2+\delta+A^{-2})(e_i-e_{i+1})=0.
$$

Hence the bracket is invariant under types II and III.

For an oriented diagram, let $w(D)$ be its [writhe](../../../../../writhe.md), the sum of its signed crossings. Types II and III preserve writhe, while a positive or negative curl changes it by one or minus one. The [Jones polynomial](../../../../../jones-polynomial.md) is therefore

$$
\boxed{V_L(t)=(-A^3)^{-w(D)}\langle D\rangle,\qquad t=A^{-4},\qquad V_{\bigcirc}=1.}
$$

The normalization cancels type I, so all [Reidemeister moves](../../../../../reidemeister-move.md) preserve it. It is a [Laurent polynomial](../../../../../laurent-polynomial.md) in $t^{1/2}$; its breadth means the largest occurring t exponent minus the smallest, including half-integral exponents for [links](../../../../../link.md).

Write $s_A,s_B$ for the all-A and all-B [circle](../../../../../circle.md) counts of a diagram with $n$ crossings. A state obtained from the all-A state by $k$ smoothing changes has at most $s_A+k$ [circles](../../../../../circle.md), because each change either joins two [circles](../../../../../circle.md) or splits one. Its largest A exponent is consequently at most $n-2k+2(s_A+k-1)=n+2s_A-2$. The symmetric argument from the all-B state bounds every exponent below by $-n-2s_B+2$. Thus the [Kauffman bracket breadth bound](../../../../../kauffman-bracket-breadth-bound.md) is

$$
\operatorname{br}_A\langle D\rangle\leq2n+2s_A+2s_B-4.
$$

For a connected diagram, construct the [Turaev surface](../../../../../turaev-surface.md) by placing A-state [circles](../../../../../circle.md) above the projection [sphere](../../../../../sphere.md), B-state [circles](../../../../../circle.md) below it, inserting one saddle at each crossing, and capping the state [circles](../../../../../circle.md). This is a connected embedded closed orientable [surface](../../../../../topological-surface.md); its disks and saddles give $\chi=s_A+s_B-n$. Since $\chi=2-2g_T\leq2$, $s_A+s_B\leq n+2$. Writhe normalization changes only a monomial, and $t=A^{-4}$ divides breadth by four. Therefore

$$
\boxed{\operatorname{br}_tV_L\leq n.}
$$

For a connected [reduced alternating diagram](../../../../../reduced-alternating-link-diagram.md), checkerboard color its complementary regions. Alternation makes all-A [circles](../../../../../circle.md) the boundaries of one color and all-B [circles](../../../../../circle.md) the boundaries of the other. Euler's formula for the connected four-valent projection graph gives $s_A+s_B=n+2$. Its [Tait graph](../../../../../tait-graph.md) and planar dual have no loops: a loop in either, equivalently a loop or bridge in one, gives a nugatory crossing cut off by a simple closed curve. Reducedness excludes precisely such crossings. Changing one smoothing in the all-A or all-B state therefore joins distinct [circles](../../../../../circle.md), so the diagram is an [adequate link diagram](../../../../../adequate-link-diagram.md).

This also proves that the extreme coefficients cannot cancel. If $k\geq1$ smoothings are changed from the all-A state, the first change lowers its [circle](../../../../../circle.md) count by one and the remaining $k-1$ changes increase it by at most $k-1$. The largest exponent of that state is at most $n+2s_A-6$, four below the all-A extreme $n+2s_A-2$, whose coefficient is $(-1)^{s_A-1}$. The all-B extreme is uniquely attained for the same reason. Consequently

$$
\boxed{\operatorname{br}_AV_L(A^{-4})=4n,\qquad\operatorname{br}_tV_L=n\quad\text{for a connected reduced alternating diagram}.}
$$

For each alternating [knot](../../../../../knot.md) $K_i$, remove nugatory crossings from an alternating diagram. The equality just proved, together with the general breadth bound for any [knot](../../../../../knot.md) diagram, shows that its reduced crossing count is minimal: $c(K_i)=\operatorname{br}V_{K_i}$. Joining two [knot](../../../../../knot.md) diagrams by an orientation-compatible [connected sum of knots](../../../../../connected-sum-of-knots.md) gives $V_{K_1\#K_2}=V_{K_1}V_{K_2}$. Indeed the state [circles](../../../../../circle.md) joined along the sum arc become one, so the bracket state sums multiply, and writhe adds. Nonzero Laurent [polynomials](../../../../../polynomial-split.md) have additive breadth, because their extreme coefficients multiply. Hence every diagram of the sum has at least $c(K_1)+c(K_2)$ crossings, while joining the two minimal alternating diagrams achieves that count. Thus

$$
\boxed{c(K_1\#K_2)=c(K_1)+c(K_2).}
$$

Finally suppose that the two-component [link](../../../../../link.md) is split. Its [Jones polynomial](../../../../../jones-polynomial.md) satisfies $V_L=-(t^{1/2}+t^{-1/2})V_{K_1}V_{K_2}$, by the disjoint-union bracket rule, so $V_L(-1)=0$. If the given alternating diagram were connected, its [Tait graph](../../../../../tait-graph.md) $G$ would be connected. Evaluate the bracket at $A=e^{\pi i/4}$, where $\delta=0$ and $t=-1$. Only one-circle states survive. These are exactly the [spanning trees](../../../../../spanning-tree.md) of $G$: a regular neighborhood of a chosen spanning subgraph has one boundary [circle](../../../../../circle.md) exactly when it is connected and has no cycle. All [spanning trees](../../../../../spanning-tree.md) use the same number of black-joining smoothings, $|V(G)|-1$. Since the crossing-to-checkerboard smoothing choice is uniform in an alternating diagram, all surviving state weights are the same nonzero power of $A$. Therefore $\langle D\rangle$ is that power times the positive number of [spanning trees](../../../../../spanning-tree.md), and $V_L(-1)\ne0$, a contradiction.

The diagram is thus disconnected. Each of the two [link](../../../../../link.md) components projects to a connected subset, so the two projection components can be separated by a boundary curve of a small regular neighborhood in the projection [sphere](../../../../../sphere.md). Hence **a split two-component [link](../../../../../link.md) represented by a reduced alternating diagram has a split diagram**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
