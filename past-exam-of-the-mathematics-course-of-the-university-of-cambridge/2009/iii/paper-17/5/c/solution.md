<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let another [local frame](../../../../../../frame-of-a-vector-bundle.md) be $e'=eA$ with $A:U\to GL_r(\mathbb R)$ smooth. Since the coefficient columns satisfy $u=Au'$, the Leibniz rule gives the [change of frame of a vector-bundle connection](../../../../../../change-of-frame-of-a-vector-bundle-connection.md):

$$
\theta'=A^{-1}\theta A+A^{-1}dA.
$$

The [curvature form of a connection](../../../../../../curvature-form.md) is linear over [smooth functions](../../../../../../smooth-function.md) in its section argument, so its [matrix](../../../../../../matrix.md) transforms homogeneously:

$$
\Theta'=A^{-1}\Theta A.
$$

Consequently

$$
\operatorname{tr}\Theta'=\operatorname{tr}(A^{-1}\Theta A)=\operatorname{tr}\Theta.
$$

The entries of $A$ are functions, of degree zero, so ordinary cyclic invariance of [trace](../../../../../../matrix-trace.md) applies without a graded sign. The local forms therefore glue to a globally defined two-form $\alpha=\operatorname{tr}\Theta$, the [trace of vector-bundle curvature](../../../../../../trace-of-vector-bundle-curvature.md).

Apply the [Bianchi identity](../../../../../../bianchi-identity.md) proved in part (b):

$$
d\alpha=\operatorname{tr}(\Theta\wedge\theta)-\operatorname{tr}(\theta\wedge\Theta).
$$

For the first term,

$$
\operatorname{tr}(\Theta\wedge\theta)=\sum_{i,j}\Theta_{ij}\wedge\theta_{ji}
=\sum_{i,j}\theta_{ji}\wedge\Theta_{ij}
=\sum_{i,j}\theta_{ij}\wedge\Theta_{ji}
=\operatorname{tr}(\theta\wedge\Theta).
$$

The middle interchange has sign $(-1)^{2\cdot1}=1$, and the next equality simply renames $i,j$. Thus

$$
\boxed{\alpha=\operatorname{tr}\Theta\text{ is frame-independent and }d\alpha=0.}
$$

One can also check closedness locally: the off-diagonal terms in $\operatorname{tr}(\theta\wedge\theta)=\sum_{i,j}\theta_{ij}\wedge\theta_{ji}$ cancel in pairs, while the diagonal terms vanish. Hence $\alpha=d(\operatorname{tr}\theta)$ in each frame, and $d^2=0$ gives the same conclusion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
