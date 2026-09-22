<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**With [local path connectedness](../../../../../locally-path-connected-space.md), the intended conclusion holds.** Choose a [base point](../../../../../base-point.md) $x_0$ and the standard [covering map](../../../../../covering-space.md)

$$
p:\mathbb R\longrightarrow S^1,\qquad p(t)=e^{2\pi it}.
$$

The [fundamental group](../../../../../fundamental-group.md) of the [circle](../../../../../circle.md) is $\mathbb Z$. Since the image of a [finite group](../../../../../finite-group.md) under a [group homomorphism](../../../../../group-homomorphism.md) is finite and $\mathbb Z$ has no nontrivial finite [subgroups](../../../../../subgroup.md),

$$
f_*:\pi_1(X,x_0)\longrightarrow\pi_1(S^1,f(x_0))\cong\mathbb Z
$$

is trivial. If $X$ is also [locally path-connected](../../../../../locally-path-connected-space.md), the [lifting criterion for a covering space](../../../../../lifting-criterion-for-a-covering-space.md) supplies a [continuous map](../../../../../continuous-map.md) $\widetilde f:X\to\mathbb R$ with $p\widetilde f=f$, because $p_*\pi_1(\mathbb R)=0$. The [homotopy](../../../../../homotopy-split.md)

$$
\boxed{H(x,s)=p\big((1-s)\widetilde f(x)+s\widetilde f(x_0)\big)}
$$

runs from $f$ to the [constant function](../../../../../constant-function.md) $f(x_0)$. This proves the claimed [null-homotopy](../../../../../null-homotopy.md) under that additional hypothesis, in particular for [CW complexes](../../../../../cw-complex.md) and the [topological graphs](../../../../../graph-topology.md) considered later in the paper.

**For arbitrary [path-connected spaces](../../../../../path-connected-space.md), the printed assertion is false.** Here is an explicit [Warsaw circle](../../../../../warsaw-circle.md) counterexample, including the obstruction that the usual lifting argument misses. In the [Euclidean plane](../../../../../euclidean-plane.md) take

$$
G=\{(x,\sin(\pi/x)):0<x\leq1\},\qquad
L=\{0\}\times[-1,1].
$$

Join $P=(1,0)$ to $Q=(0,-1)$ by the polygonal [arc](../../../../../arc-topology.md) $A$ passing successively through $(2,0),(2,-2),(0,-2)$, and put $W=G\cup L\cup A$ with its [subspace topology](../../../../../subspace-topology.md). The [arc](../../../../../arc-topology.md) meets $G\cup L$ only at $P,Q$. The [topologist's sine curve](../../../../../topologist-s-sine-curve.md) $G\cup L$ has two [path components](../../../../../path-component.md), but the added [arc](../../../../../arc-topology.md) joins them, making $W$ [path-connected](../../../../../path-connected-space.md).

Every [loop](../../../../../loop-topology.md) in $W$ is contained in

$$
T_\delta=L\cup A\cup\{(x,\sin(\pi/x)):\delta\leq x\leq1\}
$$

for some $\delta>0$. To justify the assertion, a [path](../../../../../continuous-path.md) cannot reach $L$ along the oscillating tail: the [intermediate value theorem](../../../../../intermediate-value-theorem.md) for its $x$-coordinate would force its $y$-coordinate to attain both $1$ and $-1$ arbitrarily close to the supposed arrival time, contradicting [continuity](../../../../../continuous-function.md). The only alternative route from the tail to $L$ uses $P$ and the joining [arc](../../../../../arc-topology.md). If a [loop](../../../../../loop-topology.md) visited tail points with $x\to0$, a convergent subsequence of their parameter values would approach a time at which the [loop](../../../../../loop-topology.md) lies in $L$. On a sufficiently small parameter [interval](../../../../../interval-mathematics.md) around that time its image avoids $P$. That would give a forbidden [path](../../../../../continuous-path.md) from $L$ into the tail without passing through $P$. Thus those tail coordinates have a positive lower bound. The space $T_\delta$ is a finite [tree](../../../../../tree-graph-theory-split.md), in fact a single [arc](../../../../../arc-topology.md), so every such [loop](../../../../../loop-topology.md) contracts. Consequently

$$
\pi_1(W)=1.
$$

Now define a [continuous map](../../../../../continuous-map.md) $h:W\to S^1$ to be $1$ on $G\cup L$, and to make one full turn on $A$: for a parametrization $a:[0,1]\to A$ from $P$ to $Q$, set $h(a(t))=e^{2\pi it}$. The pieces $G\cup L$ and $A$ are closed in $W$, and the formulas agree at $P,Q$, so the [pasting lemma for closed subspaces](../../../../../pasting-lemma-for-closed-subspaces.md) proves [continuity](../../../../../continuous-function.md).

There is no [continuous lift](../../../../../continuous-lift.md) $\widetilde h:W\to\mathbb R$. Any such lift is [integer](../../../../../integer-split.md)-valued on $G\cup L$, so it is constant on each of the [connected spaces](../../../../../connected-space.md) $G,L$. Since $G$ accumulates on $L$, [continuity](../../../../../continuous-function.md) forces those two constants to be the same. But along $A$ a lift of $e^{2\pi it}$ has the form $t+k$, giving values at $Q$ and $P$ differing by $1$, a contradiction. Finally, if $h$ had a [null-homotopy](../../../../../null-homotopy.md), the [homotopy lifting theorem for a covering map](../../../../../homotopy-lifting-theorem-for-a-covering-map.md), starting with a lift of the final [constant function](../../../../../constant-function.md) and reversing time, would produce a [continuous lift](../../../../../continuous-lift.md) of $h$. This theorem needs no [local path connectedness](../../../../../locally-path-connected-space.md) of the parameter space. Hence $h$ is not [null-homotopic](../../../../../null-homotopic-map.md), although $W$ has finite, indeed trivial, [fundamental group](../../../../../fundamental-group.md).

The native PDF explicitly assumes only [path connectedness](../../../../../path-connected-space.md) here. The missing [local path connectedness](../../../../../locally-path-connected-space.md) cannot be inferred from the finiteness of the [fundamental group](../../../../../fundamental-group.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology and groups course of the University of Oxford](../../../../split.md)
6. [Topology and groups course of the University of Oxford](../../../../../topology-and-groups-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
