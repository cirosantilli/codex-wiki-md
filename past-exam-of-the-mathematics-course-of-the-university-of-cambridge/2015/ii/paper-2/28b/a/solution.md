<h1 id="28b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The linearized perturbation obeys $\dot\eta=D\mathbf f(\mathbf X(t))\eta$, so its [fundamental matrix](../../../../../../fundamental-matrix-of-a-linear-differential-equation.md) satisfies

$$
\boxed{\dot\Phi=D\mathbf f(\mathbf X(t))\Phi,\qquad\Phi(0)=I.}
$$

The [Floquet multipliers](../../../../../../floquet-multiplier.md) are the [eigenvalues](../../../../../../eigenvalue.md) of the [monodromy matrix](../../../../../../monodromy-matrix.md) $\Phi(T)$. Differentiating the orbit equation shows that $\dot{\mathbf X}(t)=\mathbf f(\mathbf X(t))$ is a solution of the variational equation. For a nonconstant [periodic orbit](../../../../../../periodic-orbit.md) this tangent solution is nonzero and periodic, giving one multiplier equal to $1$.

The [Liouville formula for a fundamental matrix](../../../../../../liouville-formula-for-a-fundamental-matrix.md) gives $(\det\Phi)'=(\operatorname{tr}D\mathbf f)\det\Phi$. Since $\det\Phi(0)=1$, the product of the two multipliers is $\exp(\int_0^T\nabla\cdot\mathbf f(\mathbf X(t))\,dt)$. The other multiplier is therefore **exactly this exponential**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28B](../../28b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
