<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For common [positive-definite](../../../../../../positive-definite-bilinear-form.md) covariance, subtracting the two Gaussian log densities cancels the quadratic term. Equal priors leave the [linear discriminant analysis](../../../../../../linear-discriminant-analysis.md) score

$$
\delta(x)=(\mu_1-\mu_2)^T\Sigma^{-1}\left(x-\frac{\mu_1+\mu_2}{2}\right).
$$

Here

$$
\Sigma^{-1}=\begin{pmatrix}1/2&-1\\-1&3\end{pmatrix},\qquad
\Delta=\mu_1-\mu_2=\begin{pmatrix}3\\-1\end{pmatrix},\qquad
\Sigma^{-1}\Delta=\begin{pmatrix}5/2\\-6\end{pmatrix}.
$$

Thus

$$
\boxed{\delta(x)=\tfrac52x_1-6x_2+\tfrac{31}4;\quad
\text{assign class one if }10x_1-24x_2+31>0.}
$$

Assign class two if the expression is negative; a tie has zero probability under either continuous Gaussian law.

To compute the error rather than just specify the boundary, put $D^2=\Delta^T\Sigma^{-1}\Delta=27/2$. Within class one the score has mean $D^2/2=27/4$, and within class two mean $-27/4$. In both classes its [variance](../../../../../../variance-split.md) is $\Delta^T\Sigma^{-1}\Sigma\Sigma^{-1}\Delta=D^2$. Hence both conditional error probabilities are $\Phi(-D/2)$, where $\Phi$ is the [standard normal distribution](../../../../../../standard-normal-distribution.md) function. Equal priors give the [equal-covariance Gaussian classification error](../../../../../../equal-covariance-gaussian-classification-error.md)

$$
\boxed{P_{\mathrm{error}}=\Phi\left(-\sqrt{27/8}\right)\approx0.0331.}
$$

For the specified observation, the score is $\delta(2,1)=27/4>0$, so **assign it to class one**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
