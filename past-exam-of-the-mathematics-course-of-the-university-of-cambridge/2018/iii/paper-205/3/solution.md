<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a diagonal entry, put $Z_j=\sum_{i=1}^d(A_{ij}^2-1)$. Independence and the given [moment-generating function](../../../../../moment-generating-function.md) inequality for the [chi-squared distribution](../../../../../chi-squared-distribution.md) give

$$
\mathbb E e^{aZ_j}\leq e^{2da^2}\qquad(|a|<1/4).
$$

The [Chernoff bound](../../../../../chernoff-bound.md) with $a=t/4$ yields

$$
\mathbb P(Z_j\geq dt)\leq e^{-adt+2da^2}=e^{-dt^2/8}.
$$

Apply the same argument to $-Z_j$ and sum the two tails:

$$
\boxed{\mathbb P\left(\left|\frac{(A^TA)_{jj}}d-1\right|\geq t\right)\leq2e^{-dt^2/8}\qquad(0<t<1).}
$$

To obtain the off-diagonal bound, set $U=(V+W)/\sqrt2$ and $D=(V-W)/\sqrt2$. They are jointly normal with unit variances and covariance zero, so [independence of uncorrelated jointly normal variables](../../../../../independence-of-uncorrelated-jointly-normal-variables.md) makes them independent standard normals. Since $VW=(U^2-D^2)/2$, the [moment-generating function](../../../../../moment-generating-function.md) of the [product of two independent standard normal random variables](../../../../../product-of-two-independent-standard-normal-random-variables.md) is

$$
\boxed{\mathbb E e^{aVW}=(1-a)^{-1/2}(1+a)^{-1/2}=(1-a^2)^{-1/2}\qquad(|a|<1).}
$$

For $j\ne k$, $(A^TA)_{jk}$ is a sum of $d$ independent such products. The given inequality implies $\mathbb E e^{a(A^TA)_{jk}}\leq e^{da^2}$ for $|a|\leq1/2$. Taking $a=t/2$, and repeating for the negative tail, gives

$$
\boxed{\mathbb P\left(\frac{|(A^TA)_{jk}|}d\geq t\right)\leq2e^{-dt^2/4}\qquad(0<t<1).}
$$

Now take $t=c\sqrt{\log p/d}\in(0,1)$ and $E=A^TA/d-I_p$. There are $p$ diagonal entries but only $p(p-1)/2$ distinct off-diagonal entries, since $E$ is symmetric. By the [union bound](../../../../../boole-s-inequality.md), the event $\|E\|_{\max}\leq t$ has probability at least

$$
\begin{aligned}
1-2p e^{-dt^2/8}-p(p-1)e^{-dt^2/4}
&\geq1-2p^{1-c^2/8}-p^{2-c^2/4}.
\end{aligned}
$$

This is the required [entrywise concentration of a Gaussian Gram matrix](../../../../../entrywise-concentration-of-a-gaussian-gram-matrix.md).

On that single event, any vector $z$ supported on at most $s$ coordinates satisfies

$$
|z^TEz|\leq t\sum_{j,k}|z_jz_k|=t\|z\|_1^2\leq st\|z\|_2^2,
$$

where the last step is the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) on the support. If $u,v$ each have at most $s/2$ nonzero coordinates, $z=u-v$ has at most $s$. The same entrywise event applies simultaneously to all of them, so no union over vectors is needed. The [sparse norm preservation from entrywise Gram control](../../../../../sparse-norm-preservation-from-entrywise-gram-control.md) gives

$$
\boxed{\left|\frac{\|A(u-v)\|_2^2}{d\|u-v\|_2^2}-1\right|\leq sc\sqrt{\frac{\log p}{d}}\qquad(u\ne v).}
$$

The printed ratio is undefined at $u=v$. Its equivalent quadratic statement, $|\|A(u-v)\|_2^2/d-\|u-v\|_2^2|\leq st\|u-v\|_2^2$, includes that case trivially. The nontrivial concentration argument assumes $p\geq2,c>0$; at $p=1$ the stated probability lower bound is nonpositive and hence vacuous.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
