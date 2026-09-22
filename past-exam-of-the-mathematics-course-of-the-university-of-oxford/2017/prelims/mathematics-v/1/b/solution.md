<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [triangle](../../../../../../triangle.md) is $0\leq y\leq x\leq1$. In [polar coordinates](../../../../../../polar-coordinates.md) this becomes

$$
0\leq\theta\leq\frac\pi4,\qquad 0\leq r\leq\sec\theta,
$$

because the outer side is $x=r\cos\theta=1$. The [vector field](../../../../../../vector-field.md) and the [Jacobian determinant](../../../../../../jacobian-determinant.md) give

$$
\mathbf f=r\cos^2\theta\,\mathbf e_1+r\cos\theta\sin\theta\,\mathbf e_2,\qquad dx\,dy=r\,dr\,d\theta.
$$

Evaluate the [double integral](../../../../../../double-integral.md) component by component:

$$
\begin{aligned}
\iint_R\mathbf f\,dx\,dy
&=\frac13\int_0^{\pi/4}\bigl(\sec\theta\,\mathbf e_1+\sec\theta\tan\theta\,\mathbf e_2\bigr)d\theta\\
&=\frac13\left[\log(\sec\theta+\tan\theta)\,\mathbf e_1+\sec\theta\,\mathbf e_2\right]_0^{\pi/4}.
\end{aligned}
$$

Consequently,

$$
\boxed{\iint_R\mathbf f\,dx\,dy=\frac{\log(1+\sqrt2)}3\,\mathbf e_1+\frac{\sqrt2-1}3\,\mathbf e_2.}
$$

The origin causes no ambiguity in this [double integral](../../../../../../double-integral.md): the [continuous extension](../../../../../../continuous-extension.md) from part (a) is bounded there, and changing a value at a single point does not change the [integral](../../../../../../integral-split.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
