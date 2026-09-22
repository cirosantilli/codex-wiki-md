<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Under the permitted [singular value](../../../../../singular-value.md) bounds, $m=4n$ gives

$$
\sqrt n\leq\sigma_{\min}(G)\leq\sigma_{\max}(G)\leq3\sqrt n.
$$

For the [symmetric positive-definite matrix](../../../../../symmetric-positive-definite-matrix.md) $H=G^TG$ in part (iii), its [eigenvalues](../../../../../eigenvalue.md) are the squared [singular values](../../../../../singular-value.md) of $G$, so

$$
n\leq\lambda_{\min}(H)\leq\lambda_{\max}(H)\leq9n,
\qquad \boxed{\kappa_2(H)\leq9}.
$$

Apply the supplied [conjugate gradient convergence bound](../../../../../conjugate-gradient-convergence-bound.md) to $H$. For $e_k=x_k-x_*$ and nonzero $e_0$, the function $(\sqrt\kappa-1)/(\sqrt\kappa+1)$ increases with $\kappa\geq1$, giving

$$
\boxed{\frac{\|e_k\|_H}{\|e_0\|_H}\leq2\left(\frac{3-1}{3+1}\right)^k
=2^{1-k}}.
$$

Thus the error in this [weighted norm](../../../../../weighted-norm.md) contracts at a guaranteed exponential factor of at most $1/2$ per iteration, up to the prefactor $2$. Here $\|e\|_H=\|Ge\|_2$. The [Pythagorean identity](../../../../../pythagorean-theorem-in-an-inner-product-space.md) in part (iii) also identifies $\|e_k\|_H^2$ with the excess squared [linear least-squares problem](../../../../../linear-least-squares-problem.md) objective, which consequently decreases by a bound proportional to $4^{-k}$. For the [Euclidean norm](../../../../../euclidean-norm.md), the same [eigenvalue](../../../../../eigenvalue.md) bounds give $\|e_k\|_2/\|e_0\|_2\leq6\,2^{-k}$.

For relative accuracy $0<\epsilon<1$ in the $H$-[weighted norm](../../../../../weighted-norm.md), it is sufficient to take

$$
k\geq\left\lceil\log_2\frac2\epsilon\right\rceil.
$$

Compute $c=G^Tb$ once in $O(mn)$ operations. Each iteration applies $p\mapsto G^T(Gp)$ with two dense [matrix multiplications](../../../../../matrix-multiplication.md) and uses $O(n)$ further arithmetic operations; when $m=4n$ this costs $O(n^2)$. Hence the total cost is

$$
\boxed{O\!\left(n^2\log\frac2\epsilon\right)}.
$$

Using [finite termination of the conjugate gradient method](../../../../../finite-termination-of-the-conjugate-gradient-method.md) in exact arithmetic refines this to $O(n^2\min\{n,\lceil\log_2(2/\epsilon)\rceil\})$. Explicitly constructing $G^TG$ first would add $O(mn^2)=O(n^3)$ setup work and is unnecessary. These accuracy estimates concern relative error; an absolute tolerance replaces $2/\epsilon$ by $2\|e_0\|_H/\epsilon$ when $\|e_0\|_H>\epsilon$. If $e_0=0$, the initial guess already solves the problem.

As in part 2(b)(v), the Gaussian assumption alone does not make the printed [singular value](../../../../../singular-value.md) interval a certainty. For example, the event that every entry of $G$ has absolute value below a sufficiently small positive number has positive [probability](../../../../../probability.md) and forces $\|G\|_F<\sqrt n$, contradicting the asserted lower endpoint. The displayed rate is therefore **conditional on the singular-value bounds authorized by the paper**. The cost and convergence derivation are exact under that condition; an unconditional probabilistic statement would need an additional failure-probability estimate.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
