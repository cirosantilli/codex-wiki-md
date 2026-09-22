<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix the coefficient-column convention: write the [local frame](../../../../../../frame-of-a-vector-bundle.md) as a row $e=(e_1,\ldots,e_r)$ and a section as $s=eu$ for a column $u$ of functions. Define the [connection matrix](../../../../../../connection-one-form.md) $\theta=(\theta_{ij})$ by

$$
\nabla e_j=\sum_i e_i\theta_{ij},\qquad \nabla(eu)=e(du+\theta u).
$$

Each entry is a smooth one-form. Define the [curvature form of a connection](../../../../../../curvature-form.md) by

$$
R^E(X,Y)s=\nabla_X\nabla_Ys-\nabla_Y\nabla_Xs-\nabla_{[X,Y]}s.
$$

The same Leibniz cancellations as for tangent-bundle curvature show that this is linear over [smooth functions](../../../../../../smooth-function.md) in $X,Y,s$. Thus it is a two-form with values in the [endomorphisms](../../../../../../endomorphism.md) of $E$. Its [curvature matrix](../../../../../../curvature-form.md) $\Theta=(\Theta_{ij})$ is specified by $R^E(X,Y)e_j=\sum_i e_i\Theta_{ij}(X,Y)$.

The [covariant exterior derivative](../../../../../../exterior-covariant-derivative.md) on coefficient forms is $d+\theta\wedge$. Squaring it on $u$ gives

$$
(d+\theta\wedge)^2u=d\theta\,u-\theta\wedge du+\theta\wedge du+\theta\wedge\theta\,u.
$$

Therefore the [Cartan curvature matrix equation](../../../../../../cartan-curvature-matrix-equation.md) is

$$
\boxed{\Theta=d\theta+\theta\wedge\theta,\qquad\Theta_{ij}=d\theta_{ij}+\sum_k\theta_{ik}\wedge\theta_{kj}.}
$$

Matrix-valued wedge products here combine [matrix](../../../../../../matrix.md) multiplication with the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md), in the stated order.

Using $d^2=0$ and the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md),

$$
d\Theta=d\theta\wedge\theta-\theta\wedge d\theta.
$$

On the other hand, associativity of the [endomorphism-valued exterior product](../../../../../../endomorphism-valued-exterior-product.md) gives

$$
\begin{aligned}
\Theta\wedge\theta-\theta\wedge\Theta
&=d\theta\wedge\theta+\theta\wedge\theta\wedge\theta
-\theta\wedge d\theta-\theta\wedge\theta\wedge\theta\\
&=d\theta\wedge\theta-\theta\wedge d\theta.
\end{aligned}
$$

The cubic terms cancel, proving the requested [Bianchi identity](../../../../../../bianchi-identity.md)

$$
\boxed{d\Theta=\Theta\wedge\theta-\theta\wedge\Theta.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
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
