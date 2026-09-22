<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

The [fixed points](../../../../../fixed-point.md) are $(0,0)$ and $(\pm|\mu|,\mu^2)$. The [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J(x,y)=\begin{pmatrix}\mu^2-y&-x\\2x&-1\end{pmatrix}.
$$

At the origin its [eigenvalues](../../../../../eigenvalue.md) are $\mu^2$ and $-1$, so it is a [saddle equilibrium](../../../../../saddle-equilibrium.md) for every allowed $\mu$. At either nonzero fixed point the [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\lambda^2+\lambda+2\mu^2$, giving

$$
\boxed{\lambda_\pm=\frac{-1\pm\sqrt{1-8\mu^2}}2.}
$$

Thus both are [stable nodes](../../../../../stable-node.md) for $0<|\mu|<1/(2\sqrt2)$ and [stable focuses](../../../../../stable-spiral.md) for $|\mu|>1/(2\sqrt2)$. At equality the repeated [eigenvalue](../../../../../eigenvalue.md) is $-1/2$ and the [matrix](../../../../../matrix.md) is not scalar, so there is only one independent [eigenvector](../../../../../eigenvector.md): the fixed point is a stable improper node.

The [stable manifold](../../../../../stable-manifold.md) of the origin is **$x=0$**, exactly: there $\dot y=-y$. Conversely, a trajectory converging to the origin with $x\ne0$ would eventually have $\dot x/x=\mu^2-y>\mu^2/2$, which precludes convergence of $x$ to zero.

For the local [unstable manifold](../../../../../unstable-manifold.md), write $y=h(x)=ax^2+bx^4+O(x^6)$. Reflection symmetry makes $h$ even, and the [invariance equation for a graph](../../../../../invariance-equation-for-a-graph.md) requires

$$
h'(x)x(\mu^2-h(x))=-h(x)+x^2.
$$

Comparing quadratic and quartic terms gives $2a\mu^2=1-a$ and $4b\mu^2-2a^2=-b$. Therefore

$$
\boxed{y=\frac{x^2}{1+2\mu^2}+\frac{2x^4}{(1+4\mu^2)(1+2\mu^2)^2}+O(x^6).}
$$

## ↑ Ancestors (11)

1. [7C](../7c.md)
2. [Section I](../section-i.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
