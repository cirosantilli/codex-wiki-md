<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Serre fibration](../../../../../serre-fibration.md) has the [homotopy lifting property](../../../../../homotopy-lifting-property.md) for disks: for every $k\geq0$, a map $D^k\to E$ and a [homotopy](../../../../../homotopy.md) $D^k\times I\to B$ starting at its composite with $p:E\to B$ admit a compatible lift $D^k\times I\to E$. Equivalently, it has that lifting property for [CW complexes](../../../../../cw-complex.md). Relative lifting for CW pairs follows by attaching cells.

Let $i:F\hookrightarrow E$ be the inclusion of the chosen fiber. **The [long exact sequence of homotopy groups of a fibration](../../../../../long-exact-sequence-of-homotopy-groups-of-a-fibration.md) is**

$$
\boxed{\cdots\longrightarrow\pi_{q+1}(B,b_0)
\xrightarrow{\partial}\pi_q(F,e_0)
\xrightarrow{i_*}\pi_q(E,e_0)
\xrightarrow{p_*}\pi_q(B,b_0)
\xrightarrow{\partial}\pi_{q-1}(F,e_0)
\longrightarrow\cdots.}
$$

Its low-dimensional end is

$$
\pi_1(F)\xrightarrow{i_*}\pi_1(E)\xrightarrow{p_*}\pi_1(B)
\xrightarrow{\partial}\pi_0(F)\xrightarrow{i_*}\pi_0(E)
\longrightarrow\pi_0(B)=\{*\}.
$$

The maps $i_*$ and $p_*$ are induced by inclusion and projection on based maps; at degree zero they send a [path component](../../../../../path-component.md) to its containing or image component. The last part is an exact sequence of [pointed sets](../../../../../pointed-set.md), not in general a sequence of groups.

For $\partial:\pi_q(B)\to\pi_{q-1}(F)$, represent a class by a based cube $a:I^{q-1}\times I\to B$, constant at $b_0$ on its boundary. Lift it from the constant map $e_0$ on the bottom and side faces, using relative disk lifting. Its top face lands in $F$ and is constant on that face's boundary; its class is $\partial[a]$. The choice of lifts does not change the resulting class. For $q=1$, lift a based loop starting at $e_0$ and take the [path component](../../../../../path-component.md) of its endpoint in $F$. This fixes the boundary-map convention and defines every map in the displayed sequence.

For the splitting assertion, first take $n\geq1$. We use the [cohomological Serre spectral sequence](../../../../../cohomological-serre-spectral-sequence.md) with coefficient group $G$:

$$
E_2^{s,t}=H^s(B;H^t(F;G))
\Longrightarrow H^{s+t}(E;G),\qquad
d_r:E_r^{s,t}\to E_r^{s+r,t-r+1}.
$$

Since $B$ is [simply connected](../../../../../simply-connected-space.md), these coefficient systems are constant. The [Eilenberg–MacLane space](../../../../../eilenberg-maclane-space.md) $F=K(G,n)$ has $H^t(F;G)=0$ for $0<t<n$, and

$$
H^n(F;G)\cong\operatorname{Hom}(G,G).
$$

For $n=1$ this uses $H_1(F)=G$, with $G$ abelian; for $n>1$ it follows from the [Hurewicz theorem](../../../../../hurewicz-theorem.md) and the [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md). Let $u$ correspond to $\operatorname{id}_G$, the [universal cohomology class of an Eilenberg–MacLane space](../../../../../universal-cohomology-class-of-an-eilenberg-maclane-space.md).

In bidegree $(0,n)$ there are no incoming differentials. For $2\leq r\leq n$, an outgoing differential lands in a vanishing fiber-cohomology row. The only remaining possible differential is

$$
d_{n+1}u\in H^{n+1}(B;G)=0.
$$

Thus $u$ survives. The edge map, which is restriction to $F$, supplies a class

$$
c\in H^n(E;G),\qquad i^*c=u.
$$

By [representability of cohomology by Eilenberg–MacLane spaces](../../../../../representability-of-cohomology-by-eilenberg-maclane-spaces.md), choose a based map $q:E\to K(G,n)$ representing $c$. On $F$, $q$ induces the identity on $\pi_n=G$ and is an isomorphism on every [homotopy group](../../../../../homotopy-group.md), since the other positive groups vanish.

Consider $h=(p,q):E\to B\times K(G,n)$. This is a map of fibrations over $B$, whose map on the fiber is the weak equivalence just obtained. The map on the base is the identity. Comparing the two instances of the [long exact sequence of homotopy groups of a fibration](../../../../../long-exact-sequence-of-homotopy-groups-of-a-fibration.md) and applying exactness, or the [Five lemma](../../../../../five-lemma.md) in the group-valued range, shows that $h$ induces all [homotopy](../../../../../homotopy.md) isomorphisms. The spaces are path-connected because the base and fiber are. Hence **the [splitting of a simply connected Eilenberg–MacLane fibration](../../../../../splitting-of-a-simply-connected-eilenberg-maclane-fibration.md) gives**

$$
\boxed{E\xrightarrow{\ \simeq_{\mathrm w}\ }B\times K(G,n).}
$$

The crucial use of $H^{n+1}(B;G)=0$ is to lift the fiber's identity class; existence of a section alone was not assumed to prove a product splitting.

If $K(G,0)$ is allowed, its components have trivial positive [homotopy groups](../../../../../homotopy-group.md). The [simply connected](../../../../../simply-connected-space.md) base has no monodromy on this discrete set. Obstruction theory on the CW base gives a section in each fiber component, since all positive-dimensional fiber obstructions vanish and the component system is constant. Together these sections give $B\times G\to E$, a weak equivalence on each component. Thus the same conclusion also covers that interpretation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
