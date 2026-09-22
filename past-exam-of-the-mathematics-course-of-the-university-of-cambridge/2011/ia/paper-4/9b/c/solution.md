<h1 id="9b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $\psi=0$, the [angular momentum](../../../../../../angular-momentum.md) becomes $\mathbf L=m\mathbf r\times\dot{\mathbf r}$ and is constant. The identity $\mathbf L\cdot\mathbf r=0$ confines the trajectory to the plane through the origin perpendicular to $\mathbf L$ when $\mathbf L\ne0$. If $\mathbf L=0$, the [velocity](../../../../../../velocity.md) is radial and a [central force](../../../../../../central-force.md) preserves the radial line; this degenerate motion is also planar.

For the proposed [Laplace-Runge-Lenz vector](../../../../../../laplace-runge-lenz-vector.md) convention, differentiate $\mathbf K=\mathbf L\times\dot{\mathbf r}-\phi(r)\mathbf r$. Since $\ddot{\mathbf r}=-\phi'(r)\widehat{\mathbf r}/m$ and $\mathbf L$ is constant, the [vector triple product](../../../../../../vector-triple-product.md) gives

$$
\mathbf L\times\ddot{\mathbf r}
=-\phi'(r)(r\dot{\mathbf r}-\dot r\,\mathbf r).
$$

Therefore

$$
\dot{\mathbf K}
=-\phi'(r)(r\dot{\mathbf r}-\dot r\,\mathbf r)
-\phi'(r)\dot r\,\mathbf r-\phi(r)\dot{\mathbf r}
=-[r\phi'(r)+\phi(r)]\dot{\mathbf r}.
$$

It vanishes for general motion precisely when $(r\phi)'=0$, giving

$$
\boxed{\phi(r)=\frac Cr\quad\text{for a constant }C,\qquad\dot{\mathbf K}=0.}
$$

This is an [inverse-square potential](../../../../../../inverse-square-potential.md), attractive when $C<0$ and repulsive when $C>0$; $C=0$ is the free-particle case. An additive constant in $\phi$ leaves the force unchanged but would change this particular $\mathbf K$ by a constant multiple of $\mathbf r$, so its definition requires the displayed choice of energy zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9B](../../9b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
