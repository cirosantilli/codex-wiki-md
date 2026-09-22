<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [homotopy](../../../../homotopy-split.md) from $g$ to $h$ is a continuous $H:X\times[0,1]\to Y$ with $H(x,0)=g(x)$ and $H(x,1)=h(x)$. Precomposing gives $(w,t)\mapsto H(f(w),t)$, a [homotopy](../../../../homotopy-split.md) from $gf$ to $hf$; postcomposing gives $(x,t)\mapsto k(H(x,t))$, a [homotopy](../../../../homotopy-split.md) from $kg$ to $kh$.

A [homotopy equivalence](../../../../homotopy-equivalence.md) consists of maps $u:X\to Y$ and $v:Y\to X$ with $vu\simeq\operatorname{id}_X$ and $uv\simeq\operatorname{id}_Y$. Identity maps prove reflexivity, and exchanging $u,v$ proves symmetry. For equivalences $X\leftrightarrows Y$ and $Y\leftrightarrows Z$, compose their forward maps and compose their inverse maps in reverse order. The two compositions with these candidate inverses are homotopic to the respective identities by the pre- and postcomposition result. Concatenating the homotopies proves transitivity.

For the first listed space, radial projection onto the unit sphere gives a strong [deformation retraction](../../../../deformation-retraction.md):

$$
H_t(x)=\left(1-t+\frac t{\|x\|}\right)x.
$$

The scalar is positive, so a point outside the two coordinate axes never enters either removed axis. Their intersection with the sphere is the four points $\pm e_1,\pm e_2$. The allowed homeomorphism statement therefore identifies this retract with the four-punctured sphere in the list.

[Stereographic projection](../../../../stereographic-projection.md) from one puncture identifies that sphere with the plane minus three points. Remove small disjoint open disks around the punctures and choose a larger enclosing disk. Radial motions in the three punctured disks push their remaining points to the small boundary circles, while the exterior pushes to the large boundary circle. This reduces the space to a [compact](../../../../compact-space.md) disk with three holes. It has a spine consisting of three loops [connected](../../../../connected-space.md) by a tree of arcs; cutting along those arcs gives a disk and collapsing its collar gives the retraction onto the spine. Collapsing a maximal tree in the spine is a [homotopy equivalence](../../../../homotopy-equivalence.md) onto a wedge of three circles.

Finally the three parallel removed lines give the product

$$
\bigl(\mathbb R^2\setminus\{(1,0),(2,0),(3,0)\}\bigr)\times\mathbb R.
$$

The [homotopy](../../../../homotopy-split.md) $(x,y,z)\mapsto(x,y,(1-t)z)$ retracts this onto the [punctured plane](../../../../punctured-complex-plane.md), hence onto the same rank-three [graph](../../../../graph-split.md). Composing these maps and [homotopy](../../../../homotopy-split.md) inverses proves **all four listed spaces have the same [homotopy](../../../../homotopy-split.md) type**. The two intersecting axes produce four spherical punctures, which is why three loops appear rather than two.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../split.md)
5. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
