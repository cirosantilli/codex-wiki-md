<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the [unit-width box kernel](../../../../../unit-width-box-kernel.md), the order-zero [local polynomial estimator](../../../../../local-polynomial-regression.md) minimizes, over constants $a$,

$$
Q_x(a)=\sum_{i=1}^nK\left(\frac{x_i-x}{h}\right)(Y_i-a)^2.
$$

A common factor such as $h^{-1}$ in these weights does not change the minimizer. Put $I_x=\{i:|i/n-x|\le h/2\}$ and $N_x=|I_x|$. If $N_x>0$, differentiating the quadratic gives its unique minimizer:

$$
\boxed{\widehat m_{n,h}^P(x)=\frac1{N_x}\sum_{i\in I_x}Y_i=\frac{\sum_iK((x_i-x)/h)Y_i}{\sum_iK((x_i-x)/h)}=\widehat m_{n,h}^K(x).}
$$

The last expression is the [Nadaraya–Watson estimator](../../../../../nadaraya-watson-estimator.md). Every $x\in[0,1]$ is within $1/n$ of some design point $i/n$. Since $nh\ge2$ gives $h/2\ge1/n$, that point is in the closed kernel window. Thus $N_x\ge1$ and the equality holds throughout the domain, including $x=0$ and $x=1$.

For the error bound, first take the usual bandwidth range $0<h\le1$. The clipped window $[x-h/2,x+h/2]\cap[0,1]$ has length at least $h/2$. Any closed interval of length $L$ in $[0,1]$ contains at least $\lfloor nL\rfloor$ points of the design $\{1/n,\ldots,1\}$. Consequently

$$
N_x\ge\lfloor nh/2\rfloor\ge nh/4,
$$

where the last inequality uses $nh/2\ge1$. This is a [window occupancy for an equally spaced regression design](../../../../../window-occupancy-for-an-equally-spaced-regression-design.md) bound that remains valid at the boundary.

Let $L_m=\|m'\|_\infty$, the [Lipschitz constant](../../../../../lipschitz-constant.md) supplied by the bounded-derivative assumption. The [bias](../../../../../bias-of-an-estimator.md) is bounded by

$$
|\mathbb E\widehat m_{n,h}^P(x)-m(x)|\le\frac1{N_x}\sum_{i\in I_x}|m(x_i)-m(x)|\le L_mh/2.
$$

Independence and the variance bound give

$$
\operatorname{Var}(\widehat m_{n,h}^P(x))=\frac1{N_x^2}\sum_{i\in I_x}V(x_i)\le\frac{\sigma^2}{N_x}.
$$

By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and the triangle inequality,

$$
\boxed{\mathbb E|\widehat m_{n,h}^P(x)-m(x)|\le\frac{2\sigma}{\sqrt{nh}}+\frac12\|m'\|_\infty h\le2\left(\frac{\sigma}{\sqrt{nh}}+\|m'\|_\infty h\right).}
$$

Thus **$\kappa=2$ works uniformly in $x$ and the design size in this bandwidth range**. The same clipped-length proof in fact works for $0<h\le2$.

There is a genuine omission in the unrestricted formulation: an upper restriction on bandwidth is necessary for the displayed $1/\sqrt{nh}$ variance scale. Take $n=1$, $m\equiv0$, $Y_1\sim N(0,\sigma^2)$ and $h\ge2$. The window contains the sole observation for every $x\in[0,1]$, and $nh\ge2$ holds. Its mean absolute error is $\sigma\sqrt{2/\pi}$, whereas the proposed variance term is $\kappa\sigma/\sqrt h$. No fixed $\kappa$ can satisfy this for unbounded $h$.

A valid statement for every $h>0$ satisfying $nh\ge2$ uses $q=\min(h,1)$. The clipped window has length at least $q/2$, so $N_x\ge nq/2-1$, while the preceding coverage argument gives $N_x\ge1$. If $nq\ge4$, the first bound gives $N_x\ge nq/4$; if $nq<4$, the second does. Therefore the same bias and variance calculation proves the unrestricted correction

$$
\boxed{\mathbb E|\widehat m_{n,h}^P(x)-m(x)|\le\frac{2\sigma}{\sqrt{n\min(h,1)}}+\frac12\|m'\|_\infty h.}
$$

This [mean absolute error of local constant regression](../../../../../mean-absolute-error-of-local-constant-regression.md) bound reduces to the requested rate for ordinary small bandwidths and saturates its stochastic term when the window covers the whole design.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
