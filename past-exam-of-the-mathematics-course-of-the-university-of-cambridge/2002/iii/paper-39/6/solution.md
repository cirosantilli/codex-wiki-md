<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $f(x)=(f_1(x),\ldots,f_p(x))^T$ and let an [approximate experimental design](../../../../../approximate-experimental-design.md) $\xi$ specify the proportions of observations allocated to points of the design region. Its normalized [information matrix of an experimental design](../../../../../information-matrix-of-an-experimental-design.md) is

$$
M(\xi)=\int f(x)f(x)^T\,d\xi(x).
$$

For $N$ independent equal-variance observations realizing those proportions, $X^TX=NM(\xi)$, and the [least-squares estimator](../../../../../ordinary-least-squares-estimators.md) has [covariance matrix](../../../../../covariance-matrix.md) $\sigma^2M(\xi)^{-1}/N$. A [D-optimal design](../../../../../d-optimal-design.md) maximizes $\det M(\xi)$, equivalently minimizing the [determinant](../../../../../determinant.md) of this [covariance](../../../../../covariance.md) at fixed $N$. A [G-optimal design](../../../../../g-optimal-design.md) minimizes the largest [variance of a fitted regression mean](../../../../../variance-of-a-fitted-regression-mean.md) over the design region, equivalently

$$
\sup_x d(x,\xi),\qquad d(x,\xi)=f(x)^TM(\xi)^{-1}f(x),
$$

where $d$ is the [design sensitivity function](../../../../../design-sensitivity-function.md). This is the [variance](../../../../../variance-split.md) of the estimated mean multiplied by $N/\sigma^2$, not the [variance](../../../../../variance-split.md) of a new noisy observation.

For continuous regressors spanning a $p$-dimensional parameter space on a compact design region, the [general equivalence theorem for optimal design](../../../../../general-equivalence-theorem-for-optimal-design.md) states that, among approximate designs with nonsingular information [matrices](../../../../../matrix.md), the following are equivalent: being a [D-optimal design](../../../../../d-optimal-design.md), being a [G-optimal design](../../../../../g-optimal-design.md), and

$$
\boxed{\sup_x d(x,\xi)=p.}
$$

At every support point of an optimal design, $d=p$. To see the criterion, the sensitivity average is $\int d\,d\xi=\operatorname{tr}(M^{-1}M)=p$, so the supremum is at least $p$. Adding an infinitesimal allocation at $x$ has directional derivative $d(x,\xi)-p$ for $\log\det M$. At a D-optimum each derivative is nonpositive. Conversely, if all sensitivities are at most $p$, the tangent bound for the concave function $\log\det M$ shows that no competing design increases it. A nonsingular D-optimum exists by the spanning assumption and compactness of the information-matrix set, so the smallest possible G-value is also $p$. Equality at support points follows from the average. The theorem refers to the full approximate-design class; constrained integer allocations or mandated augmentations require separate comparison.

For the linear mean $\beta_0+\beta_1x_1+\beta_2x_2$, take $f(x)=(1,x_1,x_2)^T$. Equal replication at the four corners gives

$$
X^TX=4mI_3.
$$

All odd corner sums and the sum of $x_1x_2$ vanish, while each squared regressor sum is $4m$. If $\bar Y_{ab}$ is the mean of the $m$ observations at $(a,b)$, $a,b\in\{-1,1\}$, the [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) give

$$
\boxed{\widehat\beta=\frac14\sum_{a,b\in\{-1,1\}}\bar Y_{ab}
\begin{pmatrix}1\\a\\b\end{pmatrix},\qquad
\operatorname{Cov}(\widehat\beta)=\frac{\sigma^2}{4m}I_3.}
$$

In particular the [intercept](../../../../../regression-intercept.md) is the average of the four cell means, and each slope is the average of its sign-weighted cell means. Independence and equal error [variance](../../../../../variance-split.md) suffice for this [covariance](../../../../../covariance.md) formula; [normal](../../../../../normal-distribution.md) errors are not needed for it.

The normalized corner design has $M=I_3$, so its sensitivity is

$$
d(x,\xi)=1+x_1^2+x_2^2\le3\qquad\text{on }[-1,1]^2,
$$

with equality at all four corners. Since $p=3$, the [general equivalence theorem for optimal design](../../../../../general-equivalence-theorem-for-optimal-design.md) proves that **the equally weighted corner design is D-optimal and G-optimal**.

For the augmentation, all $m$ added observations share the regressor $f=(1,x_1,x_2)^T$. The enlarged [design matrix](../../../../../design-matrix.md) satisfies

$$
\widetilde X^T\widetilde X=m(4I_3+ff^T).
$$

By the [matrix determinant lemma](../../../../../matrix-determinant-lemma.md),

$$
\begin{aligned}
\det(\widetilde X^T\widetilde X)
&=m^3\det(4I_3)\left(1+f^T(4I_3)^{-1}f\right)\\
&=64m^3\left(1+\frac{1+x_1^2+x_2^2}{4}\right)
=16m^3(5+x_1^2+x_2^2).
\end{aligned}
$$

For the permitted nine points, the [determinant](../../../../../determinant.md) is $80m^3$ at the center, $96m^3$ at an edge midpoint and $112m^3$ at a corner. Therefore

$$
\boxed{(x_1,x_2)\in\{(-1,-1),(-1,1),(1,-1),(1,1)\},
\qquad\det(\widetilde X^T\widetilde X)=112m^3.}
$$

All four corners tie for the best mandated single-point augmentation. This is optimality among the specified augmented designs, not unrestricted D-optimality with $5m$ observations: the resulting normalized [determinant](../../../../../determinant.md) is $112/125<1$, whereas equal corner proportions have [determinant](../../../../../determinant.md) one. The restriction that the extra $m$ runs all occur at one point is what prevents recovering equal proportions.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
