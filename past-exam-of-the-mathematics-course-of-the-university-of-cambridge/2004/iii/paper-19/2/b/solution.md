<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [local isometry](../../../../../../local-isometry.md) preserves the [Levi-Civita connection](../../../../../../levi-civita-connection.md) and hence [geodesics](../../../../../../geodesic.md), as well as the lengths of lifted curves. We first show that a complete source permits finite-length paths to lift all the way to their endpoints. Begin lifting a piecewise smooth path $c:[0,1]\to N$ from any chosen point above $c(0)$, using local inverse maps. If its lift is defined only up to a maximal $b\leq1$, then

$$
d_M(\widetilde c(s),\widetilde c(t))\leq\operatorname{length}(c|_{[s,t]})\longrightarrow0
\quad\text{as }s,t\uparrow b.
$$

Completeness gives a limit point in $M$. A local inverse at that point continues the lift, including its endpoint. Thus such a finite obstruction is impossible. Connectedness of $N$ and piecewise smooth paths from $f(p)$ to any target point prove that $f$ is onto; no prior completeness of $N$ is used in this step.

Now lift the initial position and velocity of any [geodesic](../../../../../../geodesic.md) in $N$. The resulting [geodesic](../../../../../../geodesic.md) in $M$ exists for all real time by [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md). Its image extends the original target [geodesic](../../../../../../geodesic.md) by uniqueness of the [geodesic](../../../../../../geodesic.md) initial-value problem. Hence $N$ is geodesically complete, and therefore complete.

**The converse is false for a general local [isometry](../../../../../../isometry.md)**, even an onto one. Give the interval $(0,4\pi)$ its ordinary metric and map it to the unit circle by $t\mapsto e^{it}$. This is an onto [local isometry](../../../../../../local-isometry.md) to a complete circle, but the sequence $t_j=1/j$ is Cauchy in the interval and has no limit there. It is not a [covering map](../../../../../../covering-space.md): the identity point of the circle has only one preimage, whereas nearby points have two.

**The converse holds for a Riemannian covering.** If $f$ is also a [covering map](../../../../../../covering-space.md) and $N$ is complete, every target [geodesic](../../../../../../geodesic.md) defined on $\mathbb R$ lifts globally with any specified initial point. A [local isometry](../../../../../../local-isometry.md) makes that lift a [geodesic](../../../../../../geodesic.md). Its initial velocity can be any prescribed source velocity because $df$ is an isomorphism. Thus all source [geodesics](../../../../../../geodesic.md) extend for all time, and $M$ is complete by the [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
