<h1 id="14c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [First Lyapunov theorem](../../../../../../first-lyapunov-theorem.md) states that for a locally Lipschitz autonomous system $\dot x=f(x)$ with equilibrium zero, if a $C^1$ function $V$ is positive definite near zero and $\dot V=\nabla V\cdot f\le0$, then the equilibrium is [Lyapunov stable](../../../../../../lyapunov-stability.md). To prove it, choose a small sphere $|x|=\varepsilon$ inside that neighborhood. Compactness and positivity give $m=\min_{|x|=\varepsilon}V(x)>0$. Continuity at zero gives a smaller ball $|x|<\delta$ where $V<m$. Since $V$ cannot increase along a trajectory, a trajectory starting there cannot first cross the sphere where $V\ge m$. It stays within the sphere for all future time, with continuation justified by confinement in a compact subset of the vector field's domain. This proves stability for every sufficiently small $\varepsilon$.

The [LaSalle invariance principle](../../../../../../lasalle-s-invariance-principle.md) states that on a compact positively invariant set on which $\dot V\le0$, every trajectory approaches the largest invariant subset of $\{\dot V=0\}$. If that subset is just the equilibrium, the trapping and stability argument proves [asymptotic stability](../../../../../../asymptotic-stability.md).

For example take $\dot x=y$, $\dot y=-x-y$ and $V=(x^2+y^2)/2$. Then $\dot V=-y^2$, which is not strictly negative on the punctured plane. Nevertheless its sublevel discs are compact and invariant, and a trajectory confined to $y=0$ must have $\dot y=-x=0$, hence $x=0$. LaSalle gives [asymptotic stability](../../../../../../asymptotic-stability.md) despite the non-strict orbital derivative of this particular energy function.

**The printed phrase about nonexistence of a strict [Lyapunov function](../../../../../../lyapunov-function.md) must be understood as a limitation of the chosen candidate.** In this example a strict function actually exists:

$$
W=\tfrac34x^2+\tfrac12xy+\tfrac12y^2,\qquad \dot W=-\tfrac12(x^2+y^2).
$$

More generally the converse Lyapunov theorem supplies local strict functions for asymptotically stable sufficiently smooth systems. LaSalle avoids having to find such a function; it does not show that none exists.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [14C](../../14c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
