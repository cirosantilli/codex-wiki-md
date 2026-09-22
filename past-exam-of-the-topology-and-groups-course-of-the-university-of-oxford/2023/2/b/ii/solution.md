<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $n=(0,0,1)$ and use the [open cover](../../../../../open-cover.md)

$$
U=Y\setminus\{n\},\qquad V=\{(x,y,z)\in S^2:z>1/2\}.
$$

The cap $V$ is open in $Y$: it equals $Y\cap\{z>1/2\}$ because the attached chord has $z=0$. The cap is [homeomorphic](../../../../../homeomorphism.md) to an [open disk](../../../../../open-disk.md), and $U\cap V=V\setminus\{n\}$ is a punctured [open disk](../../../../../open-disk.md), hence [homotopy equivalent](../../../../../homotopy-inverse.md) to a [circle](../../../../../circle.md). Both sets and their [intersection](../../../../../set-intersection.md) are [path-connected](../../../../../path-connected-space.md). Choose the [base point](../../../../../base-point.md) $b$ in that [intersection](../../../../../set-intersection.md).

We first calculate $\pi_1(U,b)$. A [stereographic projection](../../../../../stereographic-projection.md) identifies $S^2\setminus\{n\}$ with $\mathbb R^2$ and sends the two chord endpoints to $(-1,0),(1,0)$. Thus $U$ becomes the [Euclidean plane](../../../../../euclidean-plane.md) with an extra [closed interval](../../../../../closed-real-interval.md) attached at those two points. This description is a [homeomorphism](../../../../../homeomorphism.md): gluing the two closed pieces along their endpoints gives exactly the original [subspace topology](../../../../../subspace-topology.md).

The [Euclidean plane](../../../../../euclidean-plane.md) has a [deformation retraction](../../../../../deformation-retraction.md) onto $L=[-1,1]\times\{0\}$ while fixing its endpoints. An explicit [homotopy](../../../../../homotopy-split.md) is

$$
D((u,v),t)=\big((1-t)u+t\,c(u),(1-t)v\big),\qquad
c(u)=\max(-1,\min(1,u)).
$$

Extend it by the [identity map](../../../../../identity-function.md) on the extra chord. The [pasting lemma for closed subspaces](../../../../../pasting-lemma-for-closed-subspaces.md) gives a [deformation retraction](../../../../../deformation-retraction.md) of $U$ onto two distinct [closed intervals](../../../../../closed-real-interval.md) sharing just their endpoints, a [circle](../../../../../circle.md). Consequently $\pi_1(U,b)\cong\mathbb Z$, with the routine [base point](../../../../../base-point.md) transport if the [retraction](../../../../../retraction.md) moves $b$.

The inclusion-induced [group homomorphism](../../../../../group-homomorphism.md) $\pi_1(U\cap V,b)\to\pi_1(U,b)$ is trivial: it factors through $S^2\setminus\{n\}\cong\mathbb R^2$, which is [contractible](../../../../../contractible-space.md). Also $\pi_1(V,b)=1$. All hypotheses of the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) are now checked, and it gives the [fundamental group of a sphere with an attached chord](../../../../../fundamental-group-of-a-sphere-with-an-attached-chord.md):

$$
\boxed{\pi_1(Y,b)\cong\mathbb Z*_{\mathbb Z}1\cong\mathbb Z,}
$$

where both maps from the amalgamating [infinite cyclic group](../../../../../infinite-cyclic-group.md) are trivial. A [group generator](../../../../../generator-of-a-group.md) follows the chord from one endpoint to the other and returns along any [path](../../../../../continuous-path.md) on the [sphere](../../../../../sphere.md), with a connecting [path](../../../../../continuous-path.md) from the chosen [base point](../../../../../base-point.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
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
