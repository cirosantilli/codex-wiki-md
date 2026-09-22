<h1 id="14f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $z_j=c+Re^{i\theta_j}$ with $\theta_1<\theta_2<\theta_3<\theta_4<\theta_1+2\pi$. In the identity

$$
z_j-z_\ell=2iR e^{i(\theta_j+\theta_\ell)/2}
\sin\frac{\theta_j-\theta_\ell}{2},
$$

the phase factors cancel in the [cross-ratio](../../../../../../cross-ratio.md). In our convention the two numerator sine factors are negative, while the denominator factors have opposite signs. Thus **$r<0$**, and the exchanged cross-ratio $1-r$ is **greater than one**. Consequently $|r|+1=1-r=|1-r|$.

Taking absolute values of the two formulas in part (a) gives

$$
|r|=\frac{|z_1-z_4||z_2-z_3|}{|z_1-z_2||z_3-z_4|},\qquad
|1-r|=\frac{|z_1-z_3||z_2-z_4|}{|z_1-z_2||z_3-z_4|}.
$$

Multiplying $|r|+1=|1-r|$ by the common positive denominator proves [Ptolemy theorem](../../../../../../ptolemy-s-theorem.md):

$$
\boxed{|z_1-z_3||z_2-z_4|
=|z_1-z_2||z_3-z_4|+|z_1-z_4||z_2-z_3|.}
$$

The product of the diagonals equals the sum of the products of opposite sides.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14F](../../14f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
