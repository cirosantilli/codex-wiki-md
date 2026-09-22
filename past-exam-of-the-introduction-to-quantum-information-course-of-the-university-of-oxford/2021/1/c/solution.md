<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Conjugation by the [Hadamard gate](../../../../hadamard-gate.md) sends $(X,Y,Z)$ to $(Z,-Y,X)$. Therefore its [Bloch vector](../../../../bloch-vector.md) action is

$$
\boxed{H:\ (s_x,s_y,s_z)\longmapsto(s_z,-s_y,s_x).}
$$

It is a rotation through $\pi$ about $(\mathbf e_x+\mathbf e_z)/\sqrt2$: $H=(X+Z)/\sqrt2$ differs by a [global phase](../../../../global-phase.md) from the corresponding spin rotation.

The [S gate](../../../../s-gate.md) and [T gate](../../../../t-gate.md) differ by global phases from $z$-axis rotations:

$$
\boxed{S:\ R_z(\pi/2),\qquad T:\ R_z(\pi/4).}
$$

Indeed $\operatorname{diag}(1,e^{i\theta})=e^{i\theta/2}e^{-i\theta Z/2}$, which sends $(s_x,s_y,s_z)$ to $(s_x\cos\theta-s_y\sin\theta,s_x\sin\theta+s_y\cos\theta,s_z)$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
