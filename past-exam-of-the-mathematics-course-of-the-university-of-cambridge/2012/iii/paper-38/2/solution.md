<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [autocovariance of an MA(1) process](../../../../../autocovariance-of-an-ma-1-process.md) comes directly from shared noise terms:

$$
\boxed{\gamma_0=\sigma^2(1+\theta^2),\qquad
\gamma_1=\gamma_{-1}=\sigma^2\theta,\qquad
\gamma_k=0\quad(|k|\ge2).}
$$

Work with the zero-mean [white noise](../../../../../white-noise.md) convention and $\sigma^2>0$. Put $\mathcal H_{t-1}=\operatorname{span}(X_1,\ldots,X_{t-1})$. Suppose the preceding [finite-past innovations](../../../../../finite-past-innovation.md) $U_1,\ldots,U_{t-1}$ are mutually orthogonal. Their triangular relation to the observations means that they span the same finite past. For $s\le t-2$, $U_s$ is a [linear combination](../../../../../linear-combination.md) of $X_1,\ldots,X_s$, so $\operatorname{Cov}(X_t,U_s)=0$. Moreover,

$$
\operatorname{Cov}(X_t,U_{t-1})
=\operatorname{Cov}(X_t,X_{t-1}-\lambda_{t-1}U_{t-2})
=\gamma_1.
$$

Projection onto this [orthogonal basis](../../../../../orthogonal-basis.md) therefore has only its last coefficient nonzero:

$$
\boxed{\lambda_t=\frac{\gamma_1}{\varphi_{t-1}},\qquad
\widehat X_t=\lambda_tU_{t-1},\qquad
U_t=X_t-\widehat X_t.}
$$

The residual is orthogonal to the entire preceding span, proving the induction. Expanding its [variance](../../../../../variance-split.md) gives

$$
\boxed{\varphi_t=\gamma_0-2\lambda_t\gamma_1+\lambda_t^2\varphi_{t-1}
=\gamma_0-\gamma_1\lambda_t.}
$$

The initialization is $U_1=X_1$, $\varphi_1=\gamma_0$, $\lambda_1=0$ and $U_0=0$. Each finite [covariance matrix](../../../../../covariance-matrix.md) is a [positive-definite matrix](../../../../../positive-definite-matrix.md): the last observation in any nonzero finite [linear combination](../../../../../linear-combination.md) contains a noise term absent from earlier observations. Thus all the projection denominators are positive. These are the [finite-sample innovations of an MA(1) process](../../../../../finite-sample-innovations-of-an-ma-1-process.md), requiring no Gaussian assumption.

Substituting the [covariances](../../../../../covariance.md) into the recursion gives

$$
\lambda_t=\frac{\theta}{1+\theta^2-\theta\lambda_{t-1}}.
$$

The denominator has a positive limit when $\lambda_{t-1}\to\lambda\in[-1,1]$. Taking limits gives $(\lambda-\theta)(\theta\lambda-1)=0$. The permitted interval selects

$$
\boxed{\lambda=\begin{cases}
\theta,&|\theta|\le1,\\
1/\theta,&|\theta|>1.
\end{cases}}
$$

For $\theta=0$, every coefficient is zero; at $\theta=\pm1$, the roots coincide. This is the [limiting MA(1) innovations coefficient](../../../../../limiting-ma-1-innovations-coefficient.md). The limiting innovation [variance](../../../../../variance-split.md) is correspondingly $\sigma^2\max(1,\theta^2)$.

For the observed numerical case, $\gamma_0=2$ and $\gamma_1=-1$. The exact innovation calculations are

$$
\lambda_2=-\tfrac12,\quad
U_1=-\tfrac{13}{10},\quad
U_2=\tfrac45-\left(-\tfrac12\right)\left(-\tfrac{13}{10}\right)=\tfrac3{20},
\quad \varphi_2=\tfrac32,\quad \lambda_3=-\tfrac23.
$$

Therefore the predictor of $X_3$ based on the two observations and its error [variance](../../../../../variance-split.md) are

$$
\boxed{\widehat X_{3\mid2}=-\tfrac1{10},\qquad
\operatorname{Var}(X_3-\widehat X_{3\mid2})=\tfrac43.}
$$

For $X_4$, the available information is still only $\mathcal H_2$. Since its [covariances](../../../../../covariance.md) with both $X_1$ and $X_2$ are zero, its [orthogonal projection](../../../../../orthogonal-projection.md) onto that span is zero:

$$
\boxed{\widehat X_{4\mid2}=0,\qquad
\operatorname{Var}(X_4-\widehat X_{4\mid2})=2.}
$$

This is [two-step prediction for an MA(1) process](../../../../../two-step-prediction-for-an-ma-1-process.md). Applying the next one-step recursion would instead use an observed $X_3$, which is not available here.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
