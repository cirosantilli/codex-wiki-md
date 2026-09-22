<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

For a continuously differentiable [vector field](../../../../../vector-field.md) on all of $\mathbb R^3$, the necessary and sufficient condition for a [conservative vector field](../../../../../conservative-vector-field.md) is **$\nabla\times\mathbf F=0$**. Necessity follows from equality of [mixed partial derivatives](../../../../../mixed-partial-derivative.md) of a potential; sufficiency uses the $\mathbb R^3$ being a [simply connected space](../../../../../simply-connected-space.md). On a general domain the [topology](../../../../../topology-split.md) cannot be omitted.

Here the relevant [mixed partial derivatives](../../../../../mixed-partial-derivative.md) are

$$
\partial_yF_z=\partial_zF_y=2ye^z,\quad
\partial_zF_x=\partial_xF_z=-6z^2,\quad
\partial_xF_y=\partial_yF_x=-2x\sin y.
$$

Thus the [curl](../../../../../curl.md) vanishes. Integrating the first component in $x$ gives $\Phi=x^2\cos y-2xz^3+A(y,z)$. Matching the second component gives $A_y=3+2ye^z$, hence $A=3y+y^2e^z+B(z)$. Matching the last component forces $B'=0$. A [potential of a conservative vector field](../../../../../potential-of-a-conservative-vector-field.md) with the convention $\mathbf F=\nabla\Phi$ is consequently

$$
\boxed{\Phi=x^2\cos y-2xz^3+3y+y^2e^z+C.}
$$

If a physical potential is defined instead through $\mathbf F=-\nabla V$, it is $V=-\Phi$.

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
