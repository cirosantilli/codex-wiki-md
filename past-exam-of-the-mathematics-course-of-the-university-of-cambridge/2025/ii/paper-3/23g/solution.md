<h1 id="23g/solution">Solution</h1>

↑ **Parent:** [23G](../23g.md)

Choose an evenly covered neighbourhood $U\subset R$ and a component $V$ of $\pi^{-1}(U)$. If $z:U\to\mathbb C$ is a complex chart, use

$$
z\circ\pi|_V:V\longrightarrow\mathbb C
$$

as a chart on $S$. On overlaps, the transition maps are exactly transition maps between charts of $R$, hence are holomorphic. These charts give the unique [complex structure lifted through a covering map](../../../../../complex-structure-lifted-through-a-covering-map.md) for which $\pi$ is a local biholomorphism, and therefore analytic. The Hausdorff assumption is already given; connectedness and the second-countability of a Riemann surface ensure the resulting covering surface has the required manifold properties.

A surface is simply connected when it is path-connected and every loop is null-homotopic, equivalently when its fundamental group is trivial. The [uniformization theorem](../../../../../uniformization-theorem.md) says that every simply connected Riemann surface is biholomorphic to exactly one of

$$
\mathbb C_\infty,\qquad \mathbb C,\qquad \mathbb D.
$$

Their analytic automorphism groups are

$$
\begin{aligned}
\operatorname{Aut}(\mathbb C_\infty)
&=\left\{z\mapsto\frac{az+b}{cz+d}:ad-bc\ne0\right\}/\mathbb C^*,\\
\operatorname{Aut}(\mathbb C)
&=\{z\mapsto az+b:a\ne0\},\\
\operatorname{Aut}(\mathbb D)
&=\left\{z\mapsto e^{i\theta}
\frac{z-a}{1-\bar a z}:|a|<1\right\}.
\end{aligned}
$$

A [covering space action](../../../../../covering-space-action.md) of $G$ on $X$ is an action by homeomorphisms such that every $x\in X$ has a neighbourhood $U$ satisfying

$$
gU\cap U=\varnothing\qquad(g\ne1).
$$

In particular the action is free. Every nonidentity Möbius transformation of $\mathbb C_\infty$ has a fixed point: solving $z=(az+b)/(cz+d)$ gives a root on the sphere. Consequently a subgroup $H\leq\operatorname{Aut}(\mathbb C_\infty)$ acting as a covering space action must be trivial. Its quotient is the sphere itself and is Hausdorff.

The Hausdorff conclusion fails on other Riemann surfaces. On  
$R=\mathbb C^*\cong\mathbb R^2\setminus\{0\}$, let $G=\langle T\rangle$ with

$$
T(x,y)=(2x,y/2).
$$

Every orbit is discrete in $R$ and has trivial stabilizer; small enough neighbourhoods have disjoint nontrivial translates, so this is a covering space action. Yet the two orbits through

$$
p=(1,0),\qquad q=(0,1)
$$

cannot be separated in the quotient. Indeed, for

$$
z_n=(2^{-n},1),\qquad
T^nz_n=(1,2^{-n}),
$$

we have $z_n\to q$ and $T^nz_n\to p$. Thus every pair of quotient neighbourhoods of the two distinct orbits intersects, proving that $R/G$ is not Hausdorff.

Simple connectedness does not repair this. Lift $T$ to the universal cover $\widetilde R\cong\mathbb C$ of $\mathbb C^*$. Choose the lift preserving the angular interval from $0$ to $\pi/2$. The lifted points of $z_n$ still converge to a lift of $q$, while their $n$th translates converge to a lift of $p$; those two lifts belong to different orbits. The lifted action is again a covering space action, and its quotient is non-Hausdorff although $\widetilde R$ is simply connected.

## ↑ Ancestors (10)

1. [23G](../23g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
