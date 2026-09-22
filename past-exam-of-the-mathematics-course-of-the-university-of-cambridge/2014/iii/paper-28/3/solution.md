<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The purpose of the [RSW lemma](../../../../../russo-seymour-welsh-theorem.md) is to turn local crossing information into control at every fixed shape and scale. Work with independent [bond percolation](../../../../../bond-percolation-split.md) on the [square lattice](../../../../../square-lattice.md). Let $H(a,b)$ be the event of an open left-to-right [graph path](../../../../../path-in-a-graph.md) in $[0,a]\times[0,b]\cap\mathbb Z^2$, and write $h_p(a,b)=\mathbb P_p(H(a,b))$.

A useful precise uniform version of the [RSW lemma](../../../../../russo-seymour-welsh-theorem.md) is the following [uniform RSW crossing estimate](../../../../../uniform-rsw-crossing-estimate.md). If for a fixed parameter $p$ and some $\delta>0$,

$$
\inf_{n\geq1}h_p(n,n)\geq\delta,
$$

then for every fixed aspect ratio $\rho>1$ there is $c(\delta,\rho)>0$, independent of $n$, such that

$$
\boxed{\inf_{n\geq1}h_p(\lceil\rho n\rceil,n)\geq c(\delta,\rho).}
$$

In particular this bounds length $2n$ in terms of the uniform square bound at length $n$. The constants need not be sharp. The hypotheses used in the proof are planarity, translation and reflection symmetries, the [Harris-FKG inequality](../../../../../harris-fkg-inequality.md) and [independence](../../../../../independent-random-variables.md) of unexplored [edges](../../../../../edge-of-a-graph.md). At a self-dual parameter the same argument for dual crossings gives an upper bound strictly below one as well. Neither an exact value of $p_c$ nor the existence of an infinite cluster is an assumption of this estimate.

Here is the gluing picture behind the [RSW lemma](../../../../../russo-seymour-welsh-theorem.md). For increasing crossing or attachment events, the [Harris-FKG inequality](../../../../../harris-fkg-inequality.md) provides a lower bound on their joint [probability](../../../../../probability.md). If an event of [probability](../../../../../probability.md) at least $\delta$ is a union of two reflection-related increasing alternatives $A_1,A_2$, the [square-root trick for positively associated events](../../../../../square-root-trick-for-positively-associated-events.md) gives

$$
\mathbb P_p(A_i)\geq1-\sqrt{1-\delta}.
$$

Indeed their decreasing complements are positively associated too, so $\mathbb P_p(A_1^c\cap A_2^c)\geq\mathbb P_p(A_1^c)^2$. This prevents a square crossing from concentrating all its useful attachment locations on just one side.

The nontrivial first gluing step enlarges a square to aspect ratio $3/2$. Explore an extremal square crossing, revealing the [edges](../../../../../edge-of-a-graph.md) on the explored side but leaving its other side unexamined. In that unexplored region the conditional law is still independent [bond percolation](../../../../../bond-percolation-split.md). Compare possible attachments to the crossing with their reflected alternatives. Reflection symmetry and the preceding square-root estimate give a positive bound, depending only on $\delta$, for the required attachment after averaging over the explored crossing. Carry out the reflected construction at the other end and use the [Harris-FKG inequality](../../../../../harris-fkg-inequality.md) to combine the increasing attachment events with the original crossing. Planarity ensures that the relevant transverse paths actually meet. This [RSW reflection extension lemma](../../../../../rsw-reflection-extension-lemma.md) yields a lower bound $u(\delta)>0$ for the $3n/2$-by-$n$ crossing. The exploration is important: a reflection compares the laws of fresh configurations; reflecting the picture of an open path does not make the reflected [edges](../../../../../edge-of-a-graph.md) open.

From that first extension, longer rectangles are obtained by a genuinely transverse gluing. Two $3n/2$-by-$n$ rectangles shifted by $n/2$ overlap in an $n$-by-$n$ square. Require a horizontal crossing in each long rectangle and a vertical crossing of the overlap square. Each horizontal crossing crosses that overlap from left to right, and therefore meets its vertical crossing. Their union crosses the $2n$-by-$n$ rectangle. The [Harris-FKG inequality](../../../../../harris-fkg-inequality.md) gives a lower bound $u(\delta)^2\delta$. Repeat a bounded number of times for any fixed $\rho$. Integer rounding uses neighboring lattice rectangles and bounded additional gluing steps; finitely many smallest scales can be absorbed into the constant. The constants deteriorate with $\rho$ but not with $n$. Merely requiring horizontal crossings in adjacent squares would not suffice, since their endpoints need not coincide; the overlap crossing solves that problem.

I apply the [RSW lemma](../../../../../russo-seymour-welsh-theorem.md) to the exact threshold for [bond percolation](../../../../../bond-percolation-split.md) on the [square lattice](../../../../../square-lattice.md). The [planar duality for rectangle crossings](../../../../../planar-duality-for-rectangle-crossings.md) says that an open horizontal crossing and a closed dual vertical crossing are complementary. At $p=1/2$, the dual [edge](../../../../../edge-of-a-graph.md) states have the same law as the primal ones. For the balanced lattice rectangle with side lengths $n+1,n$, the rotated dual crossing rectangle has those same side lengths: its transverse lengths before rotation are $n,n+1$. Thus the [exact self-dual rectangle crossing probability](../../../../../exact-self-dual-rectangle-crossing-probability.md) is $1/2$. Restricting a crossing of this rectangle to its first visit to the shorter vertical side gives

$$
h_{1/2}(n,n)\geq\frac12.
$$

The one-unit balance avoids assuming an exact one-half [probability](../../../../../probability.md) for every finite vertex-square convention. The [RSW lemma](../../../../../russo-seymour-welsh-theorem.md) now gives scale-independent positive bounds for all fixed-aspect-ratio primal and closed dual rectangle crossings.

Arrange four appropriately overlapping long rectangles around a square ring. Closed dual crossings along the four sides, with transverse overlap crossings if needed, join to a closed dual [graph cycle](../../../../../cycle-in-a-graph.md) surrounding the inner square. The [Harris-FKG inequality](../../../../../harris-fkg-inequality.md), applied to the closed dual states, and the [RSW lemma](../../../../../russo-seymour-welsh-theorem.md) give a constant $b>0$ for this circuit event, uniformly over ring size. Choose disjoint rings with radii increasing, for example, by a factor of four. Their circuit events depend on disjoint [edge](../../../../../edge-of-a-graph.md) sets, so they are independent. An open [graph path](../../../../../path-in-a-graph.md) from the origin to infinity would have to avoid every one of these dual barriers. Its [probability](../../../../../probability.md) is at most $(1-b)^j$ after $j$ rings and therefore zero. Hence

$$
\theta_2(1/2)=0,\qquad p_c(2)\geq\frac12.
$$

This is the [independent annular barriers for percolation](../../../../../independent-annular-barriers-for-percolation.md) argument. It is worth separating it from the other inequality: the absence of an infinite cluster at one parameter alone does not prove that every larger parameter percolates.

For the reverse inequality use [sharpness of the percolation transition](../../../../../sharpness-of-the-percolation-transition.md): below $p_c$, independent [bond percolation](../../../../../bond-percolation-split.md) on the [cubic lattice](../../../../../cubic-lattice.md) has exponentially decaying connection [probabilities](../../../../../probability.md). One can see why this is the relevant general ingredient through the [finite-set criterion for percolation sharpness](../../../../../finite-set-criterion-for-percolation-sharpness.md). For a finite set $S$ containing the origin put

$$
\varphi_p(S)=p\sum_{\substack{x\in S,\ y\notin S\\x\sim y}}
\mathbb P_p(0\leftrightarrow x\text{ using only edges in }S),
\qquad
\widetilde p_c=\sup\{p:\varphi_p(S)<1\text{ for some finite }S\ni0\}.
$$

If $\varphi_p(S)<1$, split a long open [self-avoiding walk](../../../../../self-avoiding-walk.md) at its first exit from $S$. Its internal connection, exit [edge](../../../../../edge-of-a-graph.md) and subsequent connection have disjoint witnesses. The [BK inequality](../../../../../van-den-berg-kesten-inequality.md) gives a contraction by $\varphi_p(S)$ each time distance decreases by the diameter of $S$ plus a fixed step. Iteration proves [exponential decay of subcritical percolation](../../../../../exponential-decay-of-subcritical-percolation.md) at such $p$.

To identify this finite-set threshold with $p_c$, the [Margulis–Russo formula](../../../../../margulis-russo-formula.md) expresses the derivative of $g_n(p)$ as the sum of pivotal-edge [probabilities](../../../../../probability.md). Explore the cluster attached to the box boundary, and let $S$ be its complement. On failure of the origin-to-boundary event, $0\in S$; all [edges](../../../../../edge-of-a-graph.md) from $S$ to the boundary cluster are closed, while the internal [edges](../../../../../edge-of-a-graph.md) of $S$ remain fresh. A boundary [edge](../../../../../edge-of-a-graph.md) is pivotal precisely when its endpoint in $S$ is connected to the origin inside $S$. Removing the factor $1-p$ for a closed pivotal [edge](../../../../../edge-of-a-graph.md) yields the general differential inequality

$$
\frac{d}{dp}g_n(p)\geq
\frac{1-g_n(p)}{p(1-p)}
\inf_{\substack{0\in S\subseteq\Lambda_n\setminus\partial\Lambda_n}}
\varphi_p(S).
$$

For $p>\widetilde p_c$ every finite-set quantity on the right is at least one. Integrating from any $p_0\in(\widetilde p_c,p)$ gives a positive lower bound for $g_n(p)$ independent of $n$, and taking $n\to\infty$ gives $\theta(p)>0$. Combined with the contraction below $\widetilde p_c$, this proves $p_c=\widetilde p_c$ and the stated sharpness conclusion. This outline supplies the extra threshold argument rather than assuming the desired critical value.

If $p_c(2)>1/2$, sharpness would give $g_n(1/2)\leq C e^{-cn}$. But a square crossing starting somewhere on the left side entails an open connection from that starting [graph vertex](../../../../../vertex-graph-theory.md) to distance $n$. A [union bound](../../../../../boole-s-inequality.md) over the $n+1$ possible starting [graph vertices](../../../../../vertex-graph-theory.md) gives

$$
\frac12\leq h_{1/2}(n,n)\leq(n+1)g_n(1/2),
$$

contradicting exponential decay. Therefore $p_c(2)\leq1/2$, and the two directions establish

$$
\boxed{p_c(\mathbb Z^2)=\frac12,\qquad\theta_2(1/2)=0.}
$$

This is the [Harris-Kesten theorem](../../../../../harris-kesten-theorem.md). The overall mechanism is that self-duality supplies a square crossing, the [RSW lemma](../../../../../russo-seymour-welsh-theorem.md) transports it between shapes and creates barriers at every scale, and sharpness converts the finite-scale crossing information into the exact threshold.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
