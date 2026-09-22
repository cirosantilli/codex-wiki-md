<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathbf x(\mathbf X,t)$ be the particle [flow map](../../../../../flow-map.md) from the fixed reference volume $V_0$ to the [material volume](../../../../../material-volume.md), and let $J=\det(\partial\mathbf x/\partial\mathbf X)$. Change variables and differentiate on the fixed domain:

$$
\frac d{dt}\int_{V(t)}f\,dV
=\int_{V_0}\left(\frac{Df}{Dt}J+f\frac{DJ}{Dt}\right)dV_0.
$$

Use the two permitted identities, $DJ/Dt=J\nabla\cdot\mathbf u$ and $Df/Dt=f_t+\mathbf u\cdot\nabla f$. Changing back gives

$$
\boxed{\frac d{dt}\int_{V(t)}f\,dV
=\int_{V(t)}\left(f_t+\mathbf u\cdot\nabla f+f\nabla\cdot\mathbf u\right)dV
=\int_{V(t)}\left(f_t+\nabla\cdot(f\mathbf u)\right)dV.}
$$

This is the [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md): both the value carried by each particle and the changing volume element contribute.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
