<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take $v=|\mathbf x|^2$ in [Green's second identity](../../../../../../../green-second-identity.md). Since $\nabla^2u=0$, $\nabla^2v=6$, $v=1$ on the unit [sphere](../../../../../../../sphere.md), and $\partial_nv=2$ there,

$$
6\iiint_Bu\,dV=2\iint_{\partial B}u\,dS-\iint_{\partial B}\partial_nu\,dS.
$$

The final term vanishes by the [divergence theorem](../../../../../../../divergence-theorem.md), because it equals $\iiint_B\nabla^2u\,dV=0$. Therefore

$$
\boxed{\iiint_Bu\,dV=\frac13\iint_{\partial B}u\,dS.}
$$

We assume sufficient boundary regularity for the stated boundary values and [integrals](../../../../../../../integral-split.md), or use the corresponding trace/[limit](../../../../../../../limit-of-a-function.md) formulation. This is the equality of [volume](../../../../../../../volume.md) and surface averages for a [harmonic function](../../../../../../../harmonic-function.md), since the [unit ball](../../../../../../../unit-ball.md) and [sphere](../../../../../../../sphere.md) have [volume](../../../../../../../volume.md) $4\pi/3$ and [area](../../../../../../../surface-area.md) $4\pi$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
