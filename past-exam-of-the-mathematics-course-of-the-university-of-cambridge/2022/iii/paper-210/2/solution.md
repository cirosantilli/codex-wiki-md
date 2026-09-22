<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [kernel for density estimation](../../../../../kernel-for-density-estimation.md) is an integrable function $K:\mathbb R\to\mathbb R$ with $\int K=1$. For bandwidth $h>0$, the [kernel density estimator](../../../../../kernel-density-estimation.md) is

$$
\widehat f_{n,h,K}(x)
=\frac1{nh}\sum_{i=1}^n
K\!\left(\frac{x-X_i}{h}\right).
$$

A [kernel of order ell](../../../../../kernel-of-order-ell.md) has

$$
\int u^jK(u)\,du=0
\quad(1\leq j<\ell),
\qquad
\int|u|^\ell|K(u)|\,du<\infty.
$$

Let $\mathcal H_{n,\delta}$ and $\Gamma$ be as in the question, put $h_{\max}=\max\mathcal H_{n,\delta}$, and define the positive pilot bound

$$
\widehat f_\infty
=\max\{\widehat f_{n,h_{\max},K}(x),0\}+1.
$$

For every $h\in\mathcal H_{n,\delta}$, form

$$
\widehat I_{n,h,\delta}
=\left[
\widehat f_{n,h,K}(x)-\widehat\sigma_{n,h,\delta},
\widehat f_{n,h,K}(x)+\widehat\sigma_{n,h,\delta}
\right].
$$

The [Lepski bandwidth selection method](../../../../../lepski-bandwidth-selection-method.md) takes

$$
\widehat h_\delta
=\max\left\{
h\in\mathcal H_{n,\delta}:
\bigcap_{\substack{\widetilde h\in\mathcal H_{n,\delta}\\
\widetilde h\leq h}}
\widehat I_{n,\widetilde h,\delta}\ne\varnothing
\right\}.
$$

Small bandwidths have little bias but wide intervals; the rule increases the bandwidth until the estimates cease to be mutually compatible.

The grid is geometric with ratio two. Its lower endpoint has order $\log(\log n/\delta)/n$, while its upper endpoint is of order

$$
n^{-1/(2\ell+1)}\log(\log n/\delta).
$$

For fixed $\beta\leq\ell$, the oracle bandwidth

$$
h_{\rm opt}
=\left\{
D_{\beta,L,K}^2\frac{\log(2|\mathcal H_{n,\delta}|/\delta)}n
\right\}^{1/(2\beta+1)}
$$

eventually lies between these endpoints. Its largest grid predecessor $\widetilde h_{\rm opt}$ therefore exists, and the dyadic spacing gives

$$
\widetilde h_{\rm opt}\geq\frac12h_{\rm opt}.
$$

On $\Omega_0$, the true value $f(x)$ belongs to every interval with $h\leq\widetilde h_{\rm opt}$. Their intersection is therefore nonempty, so

$$
\widehat h_\delta\geq\widetilde h_{\rm opt}.
$$

The intervals at $\widehat h_\delta$ and $\widetilde h_{\rm opt}$ have a common point. Since $\widehat\sigma_{n,h,\delta}$ decreases with $h$,

$$
\begin{aligned}
|\widehat f_{n,\widehat h_\delta,K}(x)-f(x)|
&\leq
|\widehat f_{n,\widehat h_\delta,K}(x)
-\widehat f_{n,\widetilde h_{\rm opt},K}(x)|
+\widehat\sigma_{n,\widetilde h_{\rm opt},\delta}\\
&\leq
\widehat\sigma_{n,\widehat h_\delta,\delta}
+2\widehat\sigma_{n,\widetilde h_{\rm opt},\delta}\\
&\leq3\widehat\sigma_{n,\widetilde h_{\rm opt},\delta}.
\end{aligned}
$$

Using $\widehat f_\infty\leq A$ and $\widetilde h_{\rm opt}\geq h_{\rm opt}/2$ gives

$$
|\widehat f_{n,\widehat h_\delta,K}(x)-f(x)|
\leq
24\sqrt{A R(K)}\,D_{\beta,L,K}^{-1/(2\beta+1)}
\left\{\frac{\log(2|\mathcal H_{n,\delta}|/\delta)}n\right\}^{\beta/(2\beta+1)}.
$$

Because $|\mathcal H_{n,\delta}|=O(\log n)$, enlarging the constant gives the required

$$
C(\beta,L,K)
\left\{\frac{\log(\log(4n)/\delta)}n\right\}^{\beta/(2\beta+1)}.
$$

For the final claim take $\delta_n=n^{-3}$ for sufficiently large $n$ and use $\widehat h=\widehat h_{\delta_n}$. The squared error on $\Omega_0$ is at most a constant times

$$
\left\{\frac{\log(en)}n\right\}^{2\beta/(2\beta+1)}.
$$

Off $\Omega_0$, boundedness of $K$ and the lower endpoint of the bandwidth grid give a deterministic polynomial bound on $|\widehat f_{n,\widehat h,K}(x)|$; multiplying its square by $\mathbb P(\Omega_0^c)\leq n^{-3}$ is $O(n^{-1})$. Since $f(x)\leq A$ and $N$ is independent of $\delta_n$, this term is no larger than the target rate after changing the constant. Enlarging it once more covers the finitely many $n<N$, proving the claimed adaptive [mean squared error](../../../../../mean-squared-error.md) bound.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
