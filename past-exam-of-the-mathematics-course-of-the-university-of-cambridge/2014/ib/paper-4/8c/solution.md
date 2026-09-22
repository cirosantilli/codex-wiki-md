<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

For any distinct nodes, the [polynomial](../../../../../polynomial-split.md) $q(x)=\prod_{j=1}^\nu(x-c_j)^2$ has degree $2\nu$, is nonnegative, and vanishes at every node. The [quadrature rule](../../../../../quadrature-rule.md) sum for $q$ is zero, but $\int_0^\pi wq\,dx>0$ because the weight is positive and $q$ is positive except at finitely many points. Therefore **no such rule is exact for all polynomials of degree at most $2\nu$**, irrespective of the chosen weights.

For the sine weight, its first four [moments](../../../../../moment.md) are $2,\pi,\pi^2-4,\pi^3-6\pi$. A monic degree-two [orthogonal polynomial](../../../../../orthogonal-polynomial.md) is

$$
 p_2(x)=x^2-\pi x+2,
$$

since direct use of these [moments](../../../../../moment.md) gives $\int p_2\sin x\,dx=\int xp_2\sin x\,dx=0$. Its roots lie in $(0,\pi)$ and are

$$
 \boxed{c_{1,2}=\frac\pi2\mp\sqrt{\frac{\pi^2}{4}-2},\qquad b_1=b_2=1.}
$$

The weights follow by requiring exactness for $1$ and $x$: $b_1+b_2=2$ and $b_1c_1+b_2c_2=\pi$, and the symmetric nodes imply both weights are one. To prove cubic exactness, divide any cubic as $f=ap_2+r$, with $a,r$ of degree at most one. The [integral](../../../../../integral.md) of $ap_2$ is zero by [orthogonality](../../../../../orthogonal-vectors.md), and its nodal values vanish; the remaining linear [polynomial](../../../../../polynomial-split.md) is integrated exactly. This is the [two-node Gaussian quadrature with sine weight](../../../../../two-node-gaussian-quadrature-with-sine-weight.md); the argument proves its [Gaussian quadrature](../../../../../gaussian-quadrature.md) property without assuming a general quadrature theorem.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
