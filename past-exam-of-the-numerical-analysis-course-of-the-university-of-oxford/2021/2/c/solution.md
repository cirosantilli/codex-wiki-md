<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We use the [spectral theorem](../../../../spectral-theorem.md) to construct a sufficiently accurate approximate [eigenpair](../../../../eigenpair.md). Complete $x$ to an [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md) $x,x_2,\ldots,x_n$ of the [symmetric matrix](../../../../symmetric-matrix.md) $B$, with corresponding [eigenvalues](../../../../eigenvalue.md) $\lambda,\lambda_2,\ldots,\lambda_n$. Simplicity of $\lambda$ means that every $\lambda_j-\lambda$ below is nonzero. Put

$$
a=x^TEx,\qquad
v=-\sum_{j=2}^n\frac{x_j^TEx}{\lambda_j-\lambda}x_j.
$$

The [orthogonal decomposition](../../../../orthogonal-decomposition-by-a-closed-subspace.md) of $Ex$ shows that $x^Tv=0$ and

$$
(B-\lambda I)v=-(E-aI)x.
$$

With $u_\varepsilon=x+\varepsilon v$ and $\mu_\varepsilon=\lambda+\varepsilon a$, direct expansion cancels every first-order term:

$$
\begin{aligned}
(B+\varepsilon E)u_\varepsilon-\mu_\varepsilon u_\varepsilon
&=\varepsilon\big((B-\lambda I)v+(E-aI)x\big)
+\varepsilon^2(E-aI)v\\
&=\varepsilon^2(E-aI)v.
\end{aligned}
$$

Also $\|u_\varepsilon\|_2^2=1+\varepsilon^2\|v\|_2^2\geq1$. Thus its [eigenpair residual](../../../../eigenpair-residual.md) has [Euclidean norm](../../../../euclidean-norm.md) $O(\varepsilon^2)$ in [Big O notation](../../../../big-o-notation.md).

For completeness, a real [symmetric matrix](../../../../symmetric-matrix.md) $M$ always has an [eigenvalue](../../../../eigenvalue.md) within $\|(M-\mu I)u\|_2/\|u\|_2$ of any real $\mu$ and nonzero $u$. Indeed, writing $u=\sum_jc_jq_j$ in an [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md) with [eigenvalues](../../../../eigenvalue.md) $\theta_j$ gives

$$
\|(M-\mu I)u\|_2^2
=\sum_j(\theta_j-\mu)^2c_j^2
\geq\left(\min_j|\theta_j-\mu|\right)^2\|u\|_2^2.
$$

Apply this [symmetric eigenvalue residual bound](../../../../symmetric-eigenvalue-residual-bound.md) to $M=B+\varepsilon E$. There is an [eigenvalue](../../../../eigenvalue.md) $\lambda_\varepsilon$ such that

$$
|\lambda_\varepsilon-(\lambda+\varepsilon a)|
\leq\varepsilon^2\|(E-aI)v\|_2,
$$

which proves

$$
\boxed{\lambda_\varepsilon=\lambda+\varepsilon(x^TEx)+O(\varepsilon^2).}
$$

This establishes the [first-order perturbation of a simple symmetric eigenvalue](../../../../first-order-perturbation-of-a-simple-symmetric-eigenvalue.md) without presupposing differentiability of the perturbed [eigenvector](../../../../eigenvector.md). If $n=1$, the sum defining $v$ is empty and the displayed [eigenvalue](../../../../eigenvalue.md) formula is exact.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
