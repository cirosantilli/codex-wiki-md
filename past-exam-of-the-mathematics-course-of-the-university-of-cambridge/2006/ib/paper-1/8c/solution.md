<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

For maximization of $f(x)$ subject to $g_j(x)\le0$ and $h_k(x)=0$, the [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) says: if a feasible $x^*$ globally maximizes $L(x)=f(x)-\sum_j\lambda_jg_j(x)+\sum_k\nu_kh_k(x)$, where $\lambda_j\ge0$, and $\lambda_jg_j(x^*)=0$, then $x^*$ globally maximizes $f$ over the feasible set. Indeed, at every feasible $x$,

$$
f(x)\le L(x)\le L(x^*)=f(x^*).
$$

This requires a global maximum of the [optimization Lagrangian](../../../../../optimization-lagrangian.md); a stationary point alone is not sufficient without additional concavity or another justification.

Put $q=p/(p-1)$ and $C=(\sum_i|a_i|^q)^{1/q}$. If every $a_i=0$, **the maximum is zero and every feasible vector is optimal**. Otherwise set

$$
x_i^*=\frac{\operatorname{sgn}(a_i)|a_i|^{q-1}}{C^{q-1}},\qquad \lambda=\frac Cp.
$$

Since $p(q-1)=q$, $\sum_i|x_i^*|^p=1$. For $g(x)=\sum_i|x_i|^p-1$, the [optimization Lagrangian](../../../../../optimization-lagrangian.md) is $L(x)=\sum_i a_ix_i-\lambda g(x)$. Its [gradient](../../../../../gradient.md) vanishes at $x^*$ because

$$
\lambda p\operatorname{sgn}(x_i^*)|x_i^*|^{p-1}=a_i.
$$

The function $\sum_i|x_i|^p$ is a [strictly convex function](../../../../../strictly-convex-function.md) for $p>1$, so $L$ is a [strictly concave function](../../../../../strictly-concave-function.md). Its supporting-hyperplane inequality proves that this stationary point is its global maximum. [Complementary slackness](../../../../../complementary-slackness.md) and feasibility hold, so the sufficiency theorem applies. Substitution gives

$$
\boxed{\max_{\sum_i|x_i|^p\le1}\sum_i a_ix_i=C=\left(\sum_i|a_i|^{p/(p-1)}\right)^{(p-1)/p}.}
$$

The maximizing vector is unique when $a\ne0$. It is the [norming vector for Holder inequality](../../../../../norming-vector-for-holder-inequality.md), and the value is the corresponding [dual norm](../../../../../dual-norm.md).

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
