<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A real [positive-definite kernel](../../../../../positive-semidefinite-kernel.md) is a symmetric [function](../../../../../function-split.md) $k:\mathcal X\times\mathcal X\to\mathbb R$ such that, for every finite collection $x_1,\ldots,x_n$ and every $a\in\mathbb R^n$,

$$
\sum_{i,l=1}^na_i a_l k(x_i,x_l)\ge0.
$$

Thus every [kernel matrix](../../../../../kernel-matrix.md) is a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md); “positive definite” here does not require strict positivity. A [Reproducing kernel Hilbert space](../../../../../reproducing-kernel-hilbert-space.md) is a [Hilbert space](../../../../../hilbert-space-split.md) $\mathcal H$ of [functions](../../../../../function-split.md) on $\mathcal X$ in which every [point evaluation](../../../../../point-evaluation-functional.md) is a [continuous linear functional](../../../../../continuous-linear-functional.md). Its [reproducing property](../../../../../reproducing-property.md) is $f(x)=\langle f,k_x\rangle_{\mathcal H}$ with $k_x=k(\cdot,x)\in\mathcal H$, and $k(x,y)=\langle k_y,k_x\rangle_{\mathcal H}$. For a sum of [positive-definite kernels](../../../../../positive-semidefinite-kernel.md), the [quadratic form](../../../../../quadratic-form.md) of its [kernel matrix](../../../../../kernel-matrix.md) is a sum of nonnegative [quadratic forms](../../../../../quadratic-form.md). Symmetry also survives summation. Consequently $\boxed{k=\sum_jk_j\text{ is a positive-definite kernel}.}$

For the [representer theorem](../../../../../representer-theorem.md), put $V=\operatorname{span}\{k_{x_1},\ldots,k_{x_n}\}$. This is a closed [finite-dimensional vector space](../../../../../finite-dimensional-vector-space.md). The [orthogonal decomposition by a closed subspace](../../../../../orthogonal-decomposition-by-a-closed-subspace.md) gives $f=f_V+f_\perp$, where $f_V\in V$ and $f_\perp\perp V$. The [reproducing property](../../../../../reproducing-property.md) implies $f_\perp(x_i)=0$ for every observed input, and therefore

$$
Q_1(f)=Q_1(f_V)+\lambda\|f_\perp\|_{\mathcal H}^2.
$$

Since $\lambda>0$, any [minimizer](../../../../../global-minimizer.md) must lie in $V$. For $f_\alpha=\sum_i\alpha_i k_{x_i}$, the [reproducing property](../../../../../reproducing-property.md) gives the evaluation [vector](../../../../../vector.md) $K\alpha$ and $\|f_\alpha\|_{\mathcal H}^2=\alpha^TK\alpha$. Hence $Q_1(f_\alpha)=M(\alpha)$. If $\widehat f$ minimizes $Q_1$, its representation yields a minimizing $\widehat\alpha$. Conversely, if $\widehat\alpha$ minimizes $M$, then, for any $f\in\mathcal H$, representing $f_V=f_\alpha$ gives $Q_1(f)\ge M(\alpha)\ge M(\widehat\alpha)$. Thus

$$
\boxed{\widehat f=\sum_i\widehat\alpha_i k(\cdot,x_i),\qquad \widehat\alpha\in\operatorname*{argmin}_{\alpha\in\mathbb R^n}M(\alpha).}
$$

This is an equivalence of [minimizers](../../../../../global-minimizer.md), not an existence or uniqueness assertion: the [loss function](../../../../../loss-function.md) is arbitrary. A singular [kernel matrix](../../../../../kernel-matrix.md) also allows nonunique coefficients, since differences in $\ker K$ represent the zero [function](../../../../../function-split.md). Strict [convexity](../../../../../convex-function.md) of the loss was not used.

Now use the stated minimum-norm description of a [sum of reproducing-kernel Hilbert spaces](../../../../../sum-of-reproducing-kernel-hilbert-spaces.md). Let $\widehat f=\sum_j\widehat f_j$. If the minimizing tuple did not attain the minimum total squared [norm](../../../../../norm.md) among decompositions of $\widehat f$, replacing it by that unique minimum-norm tuple would preserve the [loss function](../../../../../loss-function.md) and strictly lower the penalty. This contradicts optimality. Therefore

$$
Q_2(\widehat f_1,\ldots,\widehat f_p)=Q_1(\widehat f).
$$

For an arbitrary $f\in\mathcal H$, take its minimum-norm decomposition $(f_1,\ldots,f_p)$. Then $Q_1(\widehat f)=Q_2(\widehat f_1,\ldots,\widehat f_p)\le Q_2(f_1,\ldots,f_p)=Q_1(f)$, proving that $\widehat f$ minimizes $Q_1$.

Choose $\widehat\alpha$ from the [representer theorem](../../../../../representer-theorem.md) for this minimizing sum, and define $g_j=\sum_i\widehat\alpha_i k_j(\cdot,x_i)$. Write $K_j$ for the component [kernel matrices](../../../../../kernel-matrix.md). Then

$$
\sum_jg_j=\widehat f,\qquad
\sum_j\|g_j\|_{\mathcal H_j}^2=\sum_j\widehat\alpha^TK_j\widehat\alpha=\widehat\alpha^TK\widehat\alpha=\|\widehat f\|_{\mathcal H}^2.
$$

By uniqueness of the minimum-norm decomposition, $g_j=\widehat f_j$ for every $j$. This proves the [common representer coefficients for a sum of kernels](../../../../../common-representer-coefficients-for-a-sum-of-kernels.md) conclusion:

$$
\boxed{\widehat f_j(\cdot)=\sum_{i=1}^n\widehat\alpha_i k_j(\cdot,x_i)\quad\text{for every }j,\quad\widehat\alpha\in\operatorname*{argmin}M.}
$$

The same coefficient [vector](../../../../../vector.md) works simultaneously. Even when $K$ is singular, changing that [vector](../../../../../vector.md) by $a\in\ker K$ leaves every component unchanged: $0=a^TKa=\sum_ja^TK_ja$ forces each nonnegative squared component [norm](../../../../../norm.md) to vanish.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
