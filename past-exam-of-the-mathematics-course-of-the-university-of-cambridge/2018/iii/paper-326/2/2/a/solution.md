<h1 id="2/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [Iterated Tikhonov regularization](../../../../../../../iterated-tikhonov-regularization.md), set $A=K^*K$ and $B=(I+\tau A)^{-1}$. In a [singular system of a compact operator](../../../../../../../singular-system-of-a-compact-operator.md), each coefficient obeys

$$
c_j^{(k+1)}=\frac{c_j^{(k)}+\tau\sigma_j\langle f^\delta,w_j\rangle}
{1+\tau\sigma_j^2},\qquad c_j^{(0)}=0.
$$

Summing this geometric recurrence gives

$$
\boxed{R_{1/k}f^\delta=u_\delta^{(k)}
=\sum_j\frac{1-(1+\tau\sigma_j^2)^{-k}}{\sigma_j}
\langle f^\delta,w_j\rangle v_j.}
$$

Equivalently, its [iterated Tikhonov spectral filter](../../../../../../../iterated-tikhonov-spectral-filter.md) is $g_k(\lambda)=[1-(1+\tau\lambda)^{-k}]/\lambda$. For $x\geq0$, the finite geometric sum gives

$$
0\leq1-(1+x)^{-k}\leq\min(kx,1).
$$

Consequently the inverse coefficient is at most $\min(k\tau\sigma,1/\sigma)\leq\sqrt{k\tau}$. Thus every $R_{1/k}$ is a [bounded linear operator](../../../../../../../continuous-linear-operator.md) with

$$
\boxed{\|R_{1/k}\|\leq\sqrt{k\tau}.}
$$

For exact admissible data, write $f_j=\langle f,w_j\rangle$. The [Picard criterion](../../../../../../../picard-criterion.md) gives $\sum_j|f_j|^2/\sigma_j^2<\infty$, and

$$
\|R_{1/k}f-K^\dagger f\|^2
=\sum_j(1+\tau\sigma_j^2)^{-2k}\frac{|f_j|^2}{\sigma_j^2}\longrightarrow0
$$

by [dominated convergence theorem](../../../../../../../dominated-convergence-theorem.md). Therefore this is a linear [regularization of an inverse problem](../../../../../../../regularization-of-an-inverse-problem.md) with discrete parameter $\alpha=1/k$; a family for all positive $\alpha$ can be obtained by setting $k=\max(1,\lceil1/\alpha\rceil)$. No upper restriction on the positive [step size](../../../../../../../step-size.md) $\tau$ is needed for this implicit iteration.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
