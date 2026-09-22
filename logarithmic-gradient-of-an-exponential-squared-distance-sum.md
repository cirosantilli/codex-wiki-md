# Logarithmic gradient of an exponential squared-distance sum

↑ **Parent:** [Log-sum-exp function](log-sum-exp-function.md)

For fixed [vectors](vector.md) $a_1,\ldots,a_m$ in a finite-dimensional [Euclidean space](euclidean-norm.md), define

$$
F(x)=\sum_{i=1}^m e^{\|x-a_i\|^2},\quad
w_i(x)=\frac{e^{\|x-a_i\|^2}}{F(x)},\quad
\bar a(x)=\sum_iw_i(x)a_i.
$$

The [gradient](gradient.md) and [Hessian matrix](hessian-matrix.md) of $\Phi=\log F$ are

$$
\nabla\Phi(x)=2(x-\bar a),\qquad
\nabla^2\Phi(x)=2I+4\sum_iw_i(a_i-\bar a)(a_i-\bar a)^T.
$$

To derive the first identity, differentiate each [exponential function](exponential-function.md) and divide the sum of its [gradients](gradient.md) by $F$. For the second, differentiating a normalized weight gives $\nabla w_i=2w_i(\bar a-a_i)$. Thus $J_{\bar a}=-2\operatorname{Cov}_w(a_i)$, where the weighted [covariance matrix](covariance-matrix.md) is the sum in the displayed [Hessian matrix](hessian-matrix.md). Differentiating $2(x-\bar a)$ completes the calculation.

The weighted [covariance matrix](covariance-matrix.md) is positive semidefinite, so $\nabla^2\Phi\succeq2I$. Also $\Phi(x)\geq\|x-a_1\|^2\to\infty$ as $\|x\|\to\infty$. Therefore $F$ and $\Phi$ share a unique global minimizer, characterized by $x=\bar a(x)$. The weights place that minimizer in the [convex hull](convex-hull.md) of the centres.

For stable numerical evaluation, subtract the largest exponent before computing the normalized weights. This is the [log-sum-exp](log-sum-exp-function.md) principle and avoids [floating-point overflow](floating-point-overflow.md) without changing the [gradient](gradient.md). A naive iteration $x_{n+1}=\bar a(x_n)$ need not converge: in one dimension, centres $-1,1$ give $\bar a(x)=-\tanh(2x)$ with [derivative](derivative.md) $-2$ at its unique fixed point. A [Newton root-finding iteration](newton-root-finding-iteration.md) or a suitable [quasi-Newton method](quasi-newton-method.md) instead uses the positive curvature of $\Phi$.

## ↑ Ancestors (6)

1. [Log-sum-exp function](log-sum-exp-function.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/6/b/i/solution.md)
