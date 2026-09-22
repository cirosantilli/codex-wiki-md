<h1 id="1/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An [affine linear classifier](../../../../../../affine-linear-classifier.md) in $\mathbb R^k$ has [VC dimension](../../../../../../vc-dimension.md) $k+1$. The upper bound follows from the [intersecting convex hull partition theorem](../../../../../../radon-s-theorem.md): for any $k+2$ points, label the two parts oppositely. The two [convex hulls](../../../../../../convex-hull.md) cannot be strictly separated by an [affine hyperplane](../../../../../../affine-hyperplane.md), since they intersect. A weak boundary convention gives the same contradiction: an affine score is nonnegative on the positive [convex hull](../../../../../../convex-hull.md) and strictly negative on the negative [convex hull](../../../../../../convex-hull.md). The lower bound comes from the $k+1$ [affinely independent](../../../../../../affine-independence.md) vertices of a [simplex](../../../../../../simplex.md), because an affine score can interpolate arbitrary signs there.

Consequently, parts (i) and (ii) immediately give

$$
\boxed{d+1\leq\operatorname{VC}(\mathcal B_d)\leq d+2.}
$$

The one-sided orientation of the lifted separators permits the sharper, exact conclusion

$$
\boxed{\operatorname{VC}(\mathcal B_d)=d+1\qquad(d\geq1).}
$$

To prove the remaining upper bound, take any $d+2$ distinct points and a nonzero [affine dependence](../../../../../../affine-dependence.md) $\lambda_i$ as in part (c). Write $Q=\sum_i\lambda_i\|x_i\|^2$. Reverse every coefficient if necessary so that $Q\geq0$. Prescribe positive labels when $\lambda_i>0$ and negative labels when $\lambda_i<0$; zero coefficients may be labelled arbitrarily. If a [Euclidean ball](../../../../../../euclidean-ball.md) realized these labels, its score $g(x)=r^2-\|x-c\|^2$ would satisfy

$$
\sum_i\lambda_i g(x_i)>0.
$$

Indeed, every positive-coefficient term is nonnegative and every negative-coefficient term is strictly positive, with at least one of the latter. On the other hand, expanding the score and using the two [affine dependence](../../../../../../affine-dependence.md) identities gives

$$
\sum_i\lambda_i g(x_i)
=(r^2-\|c\|^2)\sum_i\lambda_i+2c\cdot\sum_i\lambda_i x_i-\sum_i\lambda_i\|x_i\|^2
=-Q\leq0,
$$

a contradiction. No $d+2$ points are shattered, completing the exact determination of the [VC dimension of Euclidean balls](../../../../../../vc-dimension-of-euclidean-balls.md). In the exceptional zero-dimensional [Euclidean space](../../../../../../euclidean-norm.md), every positive-radius [Euclidean ball](../../../../../../euclidean-ball.md) is the whole singleton space, so the [VC dimension](../../../../../../vc-dimension.md) is zero.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Computational learning theory](../../../../computational-learning-theory-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
