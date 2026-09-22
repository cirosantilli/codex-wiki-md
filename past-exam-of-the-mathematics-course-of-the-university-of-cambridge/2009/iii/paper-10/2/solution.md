<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [completely regular Hausdorff space](../../../../../completely-regular-hausdorff-space.md) is a [Hausdorff space](../../../../../hausdorff-space.md) in which each point $x$ outside a [closed set](../../../../../closed-set.md) $F$ is separated from $F$ by a [continuous function](../../../../../continuous-function.md) $u:X\to[0,1]$ with $u(x)=1$ and $u|_F=0$. Put $E=C_b(X)$ and define the [evaluation character](../../../../../evaluation-character.md) by $\delta_x(g)=g(x)$. The [weak-star topology](../../../../../weak-star-topology.md) on $E'$ is the topology of pointwise convergence on $E$: its coordinate maps $p\mapsto p(g)$ are continuous, and generate the topology. It is [Hausdorff](../../../../../hausdorff-space.md), and the dual unit ball is compact in it by the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md).

For nonempty $X$, $\|\delta_x\|=1$ by the [supremum norm](../../../../../supremum-norm.md) bound and the constant function $1$. All the coordinates of $x\mapsto\delta_x$ are continuous, so $\delta$ is continuous. Complete regularity separates distinct points, proving injectivity. To prove [continuity](../../../../../continuous-function.md) of the inverse onto its image, let $x\in O$ with $O$ open in $X$. Separating $x$ from $X\setminus O$ gives a bounded continuous $u$ with

$$
\delta_x\in\{p:p(u)>1/2\},\qquad\delta^{-1}\{p:p(u)>1/2\}\subseteq O.
$$

Such neighborhoods prove that **$\delta$ is a [homeomorphism](../../../../../homeomorphism.md) onto $\delta(X)$**. This qualification is essential: it is not onto the whole dual, since the zero functional is not an evaluation on a nonempty space.

Define the [Stone-Čech compactification](../../../../../stone-cech-compactification.md) to be

$$
\boxed{\beta X=\overline{\delta(X)}^{\,w^*}\subseteq B_{E'}.}
$$

The [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) makes this a [compact Hausdorff space](../../../../../compact-hausdorff-space.md), with $X$ identified with its dense evaluation copy. For $g\in C_b(X)$, the coordinate function $\widetilde g(p)=p(g)$ is a continuous extension. Density gives $\|\widetilde g\|_\infty=\|g\|_\infty$. Conversely any $h\in C(\beta X)$ restricts to an element $g$ of $C_b(X)$, and $h=\widetilde g$ because they agree on the [dense subset](../../../../../dense-set.md) $X$. Restriction and coordinate extension are inverse linear isometries, hence

$$
\boxed{C(\beta X)\cong C_b(X)\quad\text{isometrically}.}
$$

They also preserve products: the corresponding [continuous functions](../../../../../continuous-function.md) agree on $X$ and hence everywhere.

For the universal extension property, let $f:X\to K$ be continuous and $K$ a [compact Hausdorff space](../../../../../compact-hausdorff-space.md). Pullback defines a bounded [linear operator](../../../../../linear-operator.md) $T:C(K)\to C_b(X)$ by $Tg=g\circ f$. Its dual map $T':E'\to C(K)'$ is weak-star continuous, since $(T'p)(g)=p(Tg)$. Evaluation $\delta_K:K\to C(K)'$ is a [homeomorphism](../../../../../homeomorphism.md) onto a compact, thus closed, subset: a [compact Hausdorff space](../../../../../compact-hausdorff-space.md) is completely regular, by the [Urysohn lemma](../../../../../urysohn-s-lemma.md). Now $T'\delta_x=\delta_K(f(x))$, so

$$
T'(\beta X)\subseteq\overline{\delta_K(f(X))}\subseteq\delta_K(K).
$$

Therefore $\overline f=\delta_K^{-1}\circ T'|_{\beta X}$ is the required continuous extension. Two continuous maps into the [Hausdorff space](../../../../../hausdorff-space.md) $K$ agreeing on the [dense subset](../../../../../dense-set.md) $X$ agree everywhere, proving uniqueness.

If $X$ is open in $\beta X$, then it is a [locally compact space](../../../../../locally-compact-space.md): around any $x$, regularity of the [compact Hausdorff space](../../../../../compact-hausdorff-space.md) $\beta X$ gives an open neighborhood whose closure is compact and lies in $X$. Conversely, suppose $X$ is locally compact. Choose an open neighborhood $U$ of $x$ in $X$ with compact closure $C\subseteq X$. There is an open $O\subseteq\beta X$ with $O\cap X=U$. Density of $X$ implies $O\subseteq\overline U^{\beta X}$, while compactness of $C$ makes it closed in $\beta X$, so $\overline U^{\beta X}\subseteq C$. Thus $x\in O\subseteq X$. This proves

$$
\boxed{X\text{ is open in }\beta X\iff X\text{ is locally compact}.}
$$

The empty-space cases are immediate.

The final printed assertion, for an arbitrary subset of $\beta X$, is false. Take the infinite [discrete space](../../../../../discrete-space.md) $X=\mathbb N$. It is not compact, so its [compactification](../../../../../compactification-physics.md) has a point $p\in\beta\mathbb N\setminus\mathbb N$. The singleton $\{p\}$ is closed, hence equals its own closure. It is not open, since every nonempty open subset of $\beta\mathbb N$ meets the dense copy of $\mathbb N$. This is a counterexample.

The valid result holds for subsets $D\subseteq X$, and more generally for open subsets of $\beta X$. For $D\subseteq X$, its indicator is bounded continuous because $X$ is discrete. Its extension $\widetilde{\mathbf1_D}$ is still idempotent by density, so it takes only the values zero and one. The set $H=\{\widetilde{\mathbf1_D}=1\}$ is clopen and has $H\cap X=D$. Density then gives $H=\overline D^{\beta X}$. If $O$ is open in $\beta X$, the set $O\cap X$ is dense in $O$, so $\overline O=\overline{O\cap X}$ is clopen by the result just proved. Consequently **$\beta X$ is extremally disconnected**, which means the closure of every [open set](../../../../../open-set.md) is open. This is the [discrete Stone-Čech compactifications are extremally disconnected](../../../../../discrete-stone-cech-compactifications-are-extremally-disconnected.md) theorem, with the essential open-set qualification.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
