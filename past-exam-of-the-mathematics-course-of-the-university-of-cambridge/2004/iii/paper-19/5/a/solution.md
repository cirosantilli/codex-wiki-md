<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a finite symmetric generating set $S$ for $\Gamma$, let $B_S(m)$ be its [word metric](../../../../../../word-metric.md) ball, and fix $p\in M$. Set $D=\max_{s\in S}d(p,sp)$. The [triangle inequality](../../../../../../triangle-inequality.md) and invariance of distance imply

$$
d(p,\gamma p)\leq Dm\qquad(\gamma\in B_S(m)).
$$

The [properly discontinuous group action](../../../../../../properly-discontinuous-group-action.md) has a finite [point stabilizer](../../../../../../stabilizer-subgroup.md) $H=\Gamma_p$. It also gives uniform separation of distinct orbit points. To see this, only finitely many [group](../../../../../../group-split.md) elements can send $p$ into a fixed [compact](../../../../../../compact-space.md) ball about $p$, by proper discontinuity and the [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md). The positive distances among this finite list, together with the radius of the ball for all other elements, have a positive lower bound $\delta$. Thus $d(\gamma p,\gamma'p)\geq\delta$ whenever the centers differ.

Take $0<\varepsilon<\delta/2$ and write $v=\operatorname{Vol}B(p,\varepsilon)>0$. Balls of radius $\varepsilon$ about distinct orbit points are disjoint and all have volume $v$, because the action is by [isometries](../../../../../../isometry.md). Those corresponding to words of length at most $m$ lie in $B(p,Dm+\varepsilon)$. Each orbit point arises from at most $|H|$ [group](../../../../../../group-split.md) elements in $B_S(m)$, so

$$
\frac{|B_S(m)|}{|H|}\,v\leq\operatorname{Vol}B(p,Dm+\varepsilon)
\leq\omega_n(Dm+\varepsilon)^n.
$$

The final inequality is the allowed [Bishop-Gromov inequality](../../../../../../bishop-gromov-inequality.md) for nonnegative [Ricci curvature](../../../../../../ricci-curvature.md). If the entire [group](../../../../../../group-split.md) fixes $p$, proper discontinuity already makes it finite and the conclusion is immediate. Otherwise the preceding separation argument applies. Therefore

$$
\boxed{|B_S(m)|\leq\frac{|H|\omega_n}{v}(Dm+\varepsilon)^n\leq C(1+m)^n.}
$$

This is [polynomial growth of a group](../../../../../../polynomial-growth-of-a-group.md) of degree at most $n$, proved by [polynomial group growth from orbit packing](../../../../../../polynomial-group-growth-from-orbit-packing.md). Neither freeness of the action nor [compactness](../../../../../../compact-space.md) of the quotient was assumed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
