<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Vinogradov mean value](../../../../../../vinogradov-mean-value.md) is

$$
J_{k,r}(Z)=\int_{[0,1]^r}\left|\sum_{1\le z\le Z}e(\theta_1z+\cdots+\theta_rz^r)\right|^{2k}\,d\boldsymbol\theta.
$$

By [orthogonality of integer Fourier modes](../../../../../../orthogonality-of-integer-fourier-modes.md), it counts the ordered integer solutions of $\sum_{i=1}^kx_i^j=\sum_{i=1}^ky_i^j$ for $1\le j\le r$, with every coordinate between one and $\lfloor Z\rfloor$. The diagonal solutions $y_i=x_i$ give $J_{k,r}(Z)\ge\lfloor Z\rfloor^k$.

Put $D=r(r+1)/2$. The moment vector $(\sum_i x_i^j)_{j=1}^r$ has at most $\prod_{j=1}^r(k\lfloor Z\rfloor^j+1)\ll_{k,r}Z^D$ possible values. If $R(v)$ counts the tuples with vector $v$, then $\sum_vR(v)=\lfloor Z\rfloor^k$ and $J_{k,r}(Z)=\sum_vR(v)^2$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $J_{k,r}(Z)\gg_{k,r}Z^{2k-D}$. Combining the two lower bounds, with one common positive constant for large $Z$, yields

$$
\boxed{J_{k,r}(Z)\ge c(k,r)\max\{Z^k,Z^{2k-r(r+1)/2}\}.}
$$

Here is an explicit way that upper bounds enter the [Vinogradov mean-value method for a bilinear exponential sum](../../../../../../vinogradov-mean-value-method-for-a-bilinear-exponential-sum.md). Write $U=\sum_{x,y\le Z}e(\sum_j\alpha_jx^jy^j)$ and $L_j=k\lfloor Z\rfloor^j$. Two applications of the [Holder inequality](../../../../../../holder-inequality.md), followed by grouping equal differences of moment vectors, give

$$
|U|^{4k^2}\ll_{k,r}Z^{8k^2-4k}J_{k,r}(Z)^2\prod_{j=1}^r\sum_{|v|\le L_j}\min\left(2L_j+1,\frac1{2\|\alpha_jv\|}\right).
$$

At integer $\alpha_jv$ the minimum is defined as $2L_j+1$; $\|u\|$ means distance to the nearest integer. To explain the mean-value factor, let $r(v)$ count pairs of $k$-tuples with prescribed moment difference. It is an autocorrelation of $R$, so $r(v)\le\sum_wR(w)^2=J_{k,r}(Z)$ by [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). The first [Holder inequality](../../../../../../holder-inequality.md) groups the $y$ tuples, and the second groups the $x$ tuples, providing the two factors $J$. The remaining sums over moment differences are bounded by the displayed finite [geometric series](../../../../../../geometric-series.md) estimates. Good [Vinogradov mean value](../../../../../../vinogradov-mean-value.md) upper bounds, together with rational approximation or spacing bounds for $\alpha_j$, therefore give cancellation in $U$. The mean-value estimate alone does not force cancellation for arbitrary coefficients: when all $\alpha_j$ are integers, $U=\lfloor Z\rfloor^2$. For the paper take $Z=N^{2/5}$ and the specified $\alpha_j$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
