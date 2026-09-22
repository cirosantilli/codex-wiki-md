# Interior (topology)

↑ **Parent:** [Topology](topology-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interior_(topology))

The [interior](interior-topology.md) of a [subset](subset.md) $A$ of a [topological space](topological-space.md) $X$ is the [union](set-union.md) of all [open sets](open-set.md) contained in $A$, equivalently the largest [open subset](open-set.md) of $A$. A point lies in $A^\circ=\operatorname{int}_X A$ exactly when it has an [open](open-set.md) [neighbourhood](neighbourhood-mathematics.md) contained in $A$. In a [metric space](metric-space.md), this says that some [open ball](open-ball.md) $B(x,r)$, with $r>0$, is contained in $A$. The [interior](interior-topology.md) therefore identifies the points with room to move locally while staying in $A$. [Jiří Lebl, Basic Analysis, Definition 7.2.23](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/mit18_100af20_basic_analysis.pdf)

For the half-open [interval](interval-mathematics.md) $A=[0,1)$ in the [real line](real-line.md), $A^\circ=(0,1)$. Every point strictly between the endpoints has a sufficiently small [open ball](open-ball.md) inside $A$, but every [open ball](open-ball.md) about zero also contains negative points. Although $0\in A$, it is not in the [interior](interior-topology.md); it is a [boundary](boundary-of-a-set.md) point instead. Together, the [interior](interior-topology.md) and [closure](closure-topology.md) bracket the original [subset](subset.md): $A^\circ\subseteq A\subseteq\overline A$.

The ambient [topological space](topological-space.md) matters: for $X=[0,1]$ with its [subspace topology](subspace-topology.md), $\operatorname{int}_X X=X$, whereas $\operatorname{int}_{\mathbb R}X=(0,1)$. The diagram accompanying [boundary of a set](boundary-of-a-set.md) illustrates the relative [open ball](open-ball.md) at zero. A [subset](subset.md) is [open](open-set.md) exactly when $A=A^\circ$, and taking the [interior](interior-topology.md) twice has the same effect as taking it once. The [complement](complement-of-a-set.md) identity $\operatorname{int}_X A=X\setminus\operatorname{cl}_X(X\setminus A)$ links [interior](interior-topology.md) directly to [closure](closure-topology.md).

## ↑ Ancestors (5)

1. [Topology](topology-split.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
