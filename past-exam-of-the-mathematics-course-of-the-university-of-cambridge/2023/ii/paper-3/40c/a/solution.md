<h1 id="40c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For

$$
F(x)=\frac12x^TAx-b^Tx,
$$

the gradient is $\nabla F(x)=Ax-b=-r$. The [steepest descent method](../../../../../../gradient-descent.md) with [exact line search for a positive-definite quadratic](../../../../../../exact-line-search-for-a-positive-definite-quadratic.md) therefore uses

$$
x^{(k+1)}=x^{(k)}+\alpha_kr^{(k)},
\qquad
\boxed{\alpha_k=\frac{(r^{(k)})^Tr^{(k)}}{(r^{(k)})^TAr^{(k)}}.}
$$

For $A=\operatorname{diag}(1,\gamma)$ and $b=0$, the minimizer is $x^*=0$. Put

$$
q=\frac{\gamma-1}{\gamma+1}.
$$

Starting from $x^{(0)}=(\gamma,1)^T$, direct substitution gives $\alpha_k=2/(\gamma+1)$ and, inductively,

$$
\boxed{x^{(k)}=q^k(\gamma,(-1)^k)^T.}
$$

The Euclidean norm is unchanged by the alternating sign, so

$$
\frac{\|x^{(k)}-x^*\|_2}{\|x^{(0)}-x^*\|_2}=q^k.
$$

For a [positive-definite matrix](../../../../../../positive-definite-matrix.md), the [spectral condition number of a positive-definite matrix](../../../../../../spectral-condition-number-of-a-positive-definite-matrix.md) is

$$
\kappa_2(A)=\frac{\lambda_{\max}(A)}{\lambda_{\min}(A)}.
$$

Here $\kappa_2(A)=\gamma$, and hence

$$
\boxed{
\frac{\|x^{(k)}-x^*\|_2}{\|x^{(0)}-x^*\|_2}
=\left(\frac{\kappa-1}{\kappa+1}\right)^k.}
$$

The [Conjugate gradient method](../../../../../../conjugate-gradient-method.md) starts with $p_0=r_0$ and updates

$$
\alpha_k=\frac{r_k^Tr_k}{p_k^TAp_k},\quad
x_{k+1}=x_k+\alpha_kp_k,\quad
r_{k+1}=r_k-\alpha_kAp_k,
$$



$$
p_{k+1}=r_{k+1}
+\frac{r_{k+1}^Tr_{k+1}}{r_k^Tr_k}p_k.
$$

By [finite termination of the conjugate gradient method](../../../../../../finite-termination-of-the-conjugate-gradient-method.md), it reaches the exact solution in at most the number of distinct eigenvalues. This matrix has two, so at most

$$
\boxed{2\text{ iterations}}
$$

are required in exact arithmetic.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40C](../../40c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
