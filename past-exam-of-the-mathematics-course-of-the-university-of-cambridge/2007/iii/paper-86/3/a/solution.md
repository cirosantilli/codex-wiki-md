<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $k=re^{i\theta}$, with $r>0$, and rotate the plane into the line coordinates

$$
\tau=x_1\cos\theta+x_2\sin\theta,\qquad\rho=-x_1\sin\theta+x_2\cos\theta.
$$

Thus $x_1=\tau\cos\theta-\rho\sin\theta$ and $x_2=\tau\sin\theta+\rho\cos\theta$, agreeing with the directed-line geometry in the PDF. Direct substitution, rather than a formal complex rotation, gives the directional differential operator

$$
D_k=\frac{k+k^{-1}}2\partial_{x_1}+\frac{k-k^{-1}}{2i}\partial_{x_2}=A(r)\partial_\tau+iB(r)\partial_\rho,
$$

where $A=(r+r^{-1})/2$ and $B=(r^{-1}-r)/2$. If $r\ne1$, choose the invertible real-linear complex coordinate

$$
\boxed{z=\tau+i\frac{A(r)}{B(r)}\rho,\qquad\nu(r)=2A(r)=r+r^{-1}.}
$$

The [Wirtinger derivative](../../../../../../wirtinger-derivatives.md) in this coordinate is $\partial_{\bar z}=\tfrac12[\partial_\tau+i(B/A)\partial_\rho]$, so $D_k=\nu(r)\partial_{\bar z}$. Substitution gives the required transformed equation with the same multiplication and source terms. This $z$ is a new spectral-dependent spatial coordinate, not the physical $x_1+ix_2$ used in Question 2.

**The complex change of variables is valid for $0<|k|\ne1$.** At $|k|=1$, $B=0$ and the operator becomes the real line derivative $\partial_\tau$; there can be no invertible elliptic complex-coordinate change there. The two limits to this characteristic circle are precisely the boundary values needed in part (b). The expression at $k=0$ is undefined in the printed equation and is treated through its spectral limit, not by substitution.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
