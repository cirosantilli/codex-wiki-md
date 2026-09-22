<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the recurrence exactly as printed. Set $B=A^*A$ and $R=I-B/\alpha$. It gives

$$
x_{n+1}=Rx_n+\frac1\alpha A^*y,\qquad
x_0=(B+\alpha I)^{-1}A^*y.
$$

Repeated substitution yields a function of $A^*y$ alone:

$$
\boxed{x_n=R^n(B+\alpha I)^{-1}A^*y+
\frac1\alpha\sum_{j=0}^{n-1}R^jA^*y.}
$$

The empty sum is zero for $n=0$. This is [Landweber iteration with a Tikhonov initial value](../../../../../../landweber-iteration-with-a-tikhonov-initial-value.md). In the [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md), $Rv_i=r_i v_i$, where $r_i=1-\sigma_i^2/\alpha$. Thus

$$
x_n=\sum_i\left[
r_i^n\frac{\sigma_i}{\sigma_i^2+\alpha}
+\frac{\sigma_i}{\alpha}\sum_{j=0}^{n-1}r_i^j\right](y,u_i)v_i.
$$

For every positive [singular value](../../../../../../singular-value.md), the finite geometric sum gives

$$
\frac{\sigma_i}{\alpha}\sum_{j=0}^{n-1}r_i^j
=\frac{1-r_i^n}{\sigma_i}.
$$

Therefore **the [closed form of a Tikhonov-initialized Landweber iterate](../../../../../../closed-form-of-a-tikhonov-initialized-landweber-iterate.md) is**

$$
\boxed{x_n=\sum_i g_{\alpha,n}(\sigma_i)(y,u_i)v_i,\qquad
g_{\alpha,n}(\sigma)=\frac1{\sigma}\left[
1-\frac{\alpha}{\alpha+\sigma^2}\left(1-\frac{\sigma^2}{\alpha}\right)^n
\right].}
$$

In the printed notation, $g_\alpha(y,u_i)$ means the coefficient $g_{\alpha,n}(\sigma_i)(y,u_i)$; its dependence on $n$ and $\sigma_i$ is implicit. At $n=0$, the formula reduces to $\sigma/(\sigma^2+\alpha)$, exactly the [Tikhonov regularization](../../../../../../tikhonov-regularization.md) initial value. At fixed $n$, its apparent singularity at $\sigma=0$ is removable:

$$
g_{\alpha,n}(\sigma)=\frac{(n+1)\sigma}{\alpha}+O(\sigma^3).
$$

Thus each fixed iterate is a bounded reconstruction operator and the series converges in norm.

The terminology in the question requires care. The printed recurrence is explicit [Landweber iteration](../../../../../../landweber-iteration.md) with step $1/\alpha$. Convergence of its nonzero modes requires $|1-\sigma_i^2/\alpha|<1$; a sufficient uniform step condition is

$$
\boxed{\alpha>\frac{\|A\|^2}{2}.}
$$

With exact compatible data and this condition, $x_n\to x^\dagger$. At equality the largest singular-value mode can alternate, and smaller $\alpha$ can produce growing modes. With noisy data, [early stopping of Landweber iteration](../../../../../../early-stopping-of-landweber-iteration.md) is needed to prevent recovery of arbitrarily unstable small-singular-value components.

Conventional [Iterated Tikhonov regularization](../../../../../../iterated-tikhonov-regularization.md) instead uses the implicit update

$$
(B+\alpha I)x_{n+1}=\alpha x_n+A^*y.
$$

With the same [Tikhonov regularization](../../../../../../tikhonov-regularization.md) initial value its filter would be $[1-(\alpha/(\alpha+\sigma^2))^{n+1}]/\sigma$, not the filter derived above. The solution here retains the authoritative printed update rather than silently changing it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
