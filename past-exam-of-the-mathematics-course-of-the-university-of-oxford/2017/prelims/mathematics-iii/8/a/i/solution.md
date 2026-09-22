<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat the explanatory variables as fixed and put $S_{xx}=\sum_i x_i^2$, $S_{zz}=\sum_i z_i^2$. To identify both slopes, assume $S_{xx}>0$ and $S_{zz}>0$. The given centring and [orthogonality](../../../../../../../orthogonal-vectors.md) conditions make the three columns $1,x,z$ pairwise [orthogonal](../../../../../../../orthogonal-vectors.md).

The [log-likelihood function](../../../../../../../log-likelihood.md) in the [normal linear model](../../../../../../../normal-linear-model-split.md), up to a constant independent of the coefficients, is

$$
\ell(\beta_0,\beta_1,\beta_2)=-\frac1{2\sigma^2}\sum_i(Y_i-\beta_0-\beta_1x_i-\beta_2z_i)^2.
$$

Thus [maximum likelihood estimation](../../../../../../../maximum-likelihood-estimation-split.md) minimizes the [residual sum of squares](../../../../../../../residual-sum-of-squares.md). Setting its [partial derivatives](../../../../../../../partial-derivative.md) to zero gives

$$
\sum_i(Y_i-\beta_0-\beta_1x_i-\beta_2z_i)=0,\quad
\sum_i x_i(Y_i-\beta_0-\beta_1x_i-\beta_2z_i)=0,\quad
\sum_i z_i(Y_i-\beta_0-\beta_1x_i-\beta_2z_i)=0.
$$

Using $\sum x_i=\sum z_i=\sum x_iz_i=0$ decouples these equations:

$$
\boxed{\widehat\beta_0=\overline Y,\qquad
\widehat\beta_1=\frac{\sum_i x_iY_i}{S_{xx}},\qquad
\widehat\beta_2=\frac{\sum_i z_iY_i}{S_{zz}}.}
$$

The [Hessian matrix](../../../../../../../hessian-matrix.md) of the [residual sum of squares](../../../../../../../residual-sum-of-squares.md) is $2\operatorname{diag}(n,S_{xx},S_{zz})$, which is positive definite. These are therefore the unique minimizers. If either squared sum is zero, the associated explanatory variable vanishes identically and its coefficient cannot be identified.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
