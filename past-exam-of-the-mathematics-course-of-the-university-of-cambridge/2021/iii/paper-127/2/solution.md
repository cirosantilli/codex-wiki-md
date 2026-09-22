<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A map $p:E\to B$ is a [Serre fibration](../../../../../serre-fibration.md) when it has the [homotopy lifting property](../../../../../homotopy-lifting-property.md) for every disc: given $g:D^k\to E$ and $H:D^k\times I\to B$ with $pg=H(-,0)$, there is a lift $\widetilde H:D^k\times I\to E$ satisfying $\widetilde H(-,0)=g$ and $p\widetilde H=H$.

Fix $b_0\in B$, $e_0\in F=p^{-1}(b_0)$, and write $i:F\hookrightarrow E$. The [long exact sequence of homotopy groups of a fibration](../../../../../long-exact-sequence-of-homotopy-groups-of-a-fibration.md) is

$$
\cdots\to\pi_k(F,e_0)\xrightarrow{i_*}\pi_k(E,e_0)
\xrightarrow{p_*}\pi_k(B,b_0)
\xrightarrow{\partial}\pi_{k-1}(F,e_0)\to\cdots.
$$

The first two maps are induced by inclusion and projection. To define $\partial$, represent a class of $\pi_k(B)$ by a map of pairs $(D^k,S^{k-1})\to(B,b_0)$, lift it beginning at $e_0$ along radial paths, and restrict the lift to $S^{k-1}$; that restriction lies in $F$. At the bottom, exactness continues through the pointed sets $\pi_1(B)\to\pi_0(F)\to\pi_0(E)\to\pi_0(B)$.

Every [fiber bundle](../../../../../fiber-bundle-split.md) is a Serre fibration. Pull a bundle back along $H:D^k\times I\to B$; a lift of $H$ is the same as a section of this pullback extending the section over $D^k\times\{0\}$ supplied by $g$. Since $D^k\times I$ is compact, finitely many bundle charts cover it. A Lebesgue-number subdivision of $I$, followed by a finite subdivision of $D^k$, makes each resulting prism lie in one chart. In a trivialization $U\times F\to U$, extend the section across a prism by keeping its $F$-coordinate constant along the interval direction. Proceed prism by prism and time-slab by time-slab; on an already treated face use its prescribed coordinate, and the transition functions ensure agreement on overlaps. The resulting sections glue to the required lift $\widetilde H$.

Now consider $i:\mathbb{RP}^n\hookrightarrow\mathbb{CP}^n$. The target is simply connected, so $i_*$ is zero on $\pi_1$. For $k\geq2$, every based map $S^k\to\mathbb{RP}^n$ lifts through the double cover to $S^n$. The composite

$$
S^n\longrightarrow\mathbb{RP}^n\xrightarrow{i}\mathbb{CP}^n,
\qquad x\longmapsto[\mathbb Cx],
$$

lifts through the [Hopf fibration](../../../../../hopf-fibration.md) $S^{2n+1}\to\mathbb{CP}^n$ to the real-coordinate inclusion $S^n\hookrightarrow S^{2n+1}$. This inclusion is null-homotopic because $\pi_n(S^{2n+1})=0$. Hence $i_*$ is zero on every $\pi_k$, including the cases $n=1$ and $k\geq2$ where the source groups already vanish.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 127](../../paper-127-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
