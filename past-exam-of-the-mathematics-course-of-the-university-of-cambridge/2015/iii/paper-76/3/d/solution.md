<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For nonzero $A$, a sufficient step-size condition for [strong convergence of relaxed Landweber iteration](../../../../../../strong-convergence-of-relaxed-landweber-iteration.md) is

$$
\boxed{0<\tau<\frac2{\|A\|^2}.}
$$

For the unrelaxed iteration, this reads $\|A\|^2<2$. The data must also admit a [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md) $x^\dagger$; for the exact problem, $y\in\operatorname{Ran}A$ is sufficient. More generally, the projected-data condition in part (a), or the [Picard criterion](../../../../../../picard-criterion.md) $\sum_i|\langle y,u_i\rangle|^2/\sigma_i^2<\infty$, ensures the required solution.

Every positive [singular value](../../../../../../singular-value.md) satisfies $|1-\tau\sigma_i^2|<1$, so for fixed $\sigma_i>0$,

$$
\boxed{\lim_{\alpha\to0}g_\alpha(\sigma_i)=\frac1{\sigma_i}.}
$$

This is the correct inverse coefficient. For exact data with a [least-squares solution](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md), the [norm](../../../../../../norm.md) error is

$$
 \|x_n-x^\dagger\|^2=\sum_i
 |1-\tau\sigma_i^2|^{2n}\frac{|\langle y,u_i\rangle|^2}{\sigma_i^2}\longrightarrow0.
$$

The summable majorant is precisely the [Picard criterion](../../../../../../picard-criterion.md), so the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) proves strong convergence, despite the absence of a uniform contraction constant when the [singular values](../../../../../../singular-value.md) approach zero. Initialization at zero selects the solution orthogonal to $\ker A$. At $\tau=2/\|A\|^2$, a top singular mode of a nonzero [compact operator](../../../../../../compact-operator-split.md) has multiplier $-1$ and can oscillate indefinitely; the strict step bound avoids this failure.

Pointwise convergence of filters alone is not a full noisy-data [inverse-problem regularization](../../../../../../regularization-of-an-inverse-problem.md) proof. For each finite $n$, put $t=\tau\sigma^2$; the step restriction gives $|1-t|\leq1$, and

$$
 |1-(1-t)^n|\leq\min(nt,2),\qquad
 |g_{1/n}(\sigma)|\leq\min(n\tau\sigma,2/\sigma)\leq\sqrt{2n\tau}.
$$

This proves the [uniform noise bound for relaxed Landweber iteration](../../../../../../uniform-noise-bound-for-relaxed-landweber-iteration.md)

$$
 \|x_n^{(\delta)}-x_n\|\leq\delta\sqrt{2n\tau}.
$$

Together with the exact-data convergence,

$$
\boxed{\|x_n^{(\delta)}-x^\dagger\|
 \leq\delta\sqrt{2n\tau}+\|x_n-x^\dagger\|\longrightarrow0}
$$

whenever $n=n(\delta)\to\infty$ and $\delta\sqrt{n(\delta)}\to0$. Equivalently, the [a priori regularization parameter choice](../../../../../../a-priori-regularization-parameter-choice.md) satisfies $\alpha(\delta)\to0$ and $\delta/\sqrt{\alpha(\delta)}\to0$. For example, $n(\delta)=\lfloor\delta^{-1}\rfloor$ works as $\delta\to0$. The sharper familiar bound $\delta\sqrt{n\tau}$ is available when $\tau\|A\|^2\leq1$.

Thus **finite iteration followed by an appropriate stopping rule is a [convergent regularization of an inverse problem](../../../../../../convergent-regularization-of-an-inverse-problem.md)**. Taking $n\to\infty$ for fixed noisy data is not the same operation and can amplify the small-singular-value noise without bound. If $A=0$, the zero starting iterate stays zero and is the [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md) for every datum; the step restriction is needed only for nonzero $A$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
