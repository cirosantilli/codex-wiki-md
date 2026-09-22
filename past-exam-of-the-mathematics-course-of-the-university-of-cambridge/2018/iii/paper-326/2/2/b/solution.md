<h1 id="2/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\eta=f^\delta-f$, so $\|\eta\|\leq\delta$. By linearity, $u_\delta^{(k)}-u^{(k)}=R_{1/k}\eta$. The preceding [operator norm](../../../../../../../operator-norm.md) estimate gives

$$
\boxed{\|u_\delta^{(k)}-u^{(k)}\|\leq\sqrt{k\tau}\,\delta.}
$$

Moreover, $KR_{1/k}$ has factors $1-(1+\tau\sigma_j^2)^{-k}$ on the data [singular vectors](../../../../../../../singular-vector.md), and is zero on $\mathcal R(K)^\perp$. Every factor is in $[0,1]$, hence

$$
\boxed{\|Ku_\delta^{(k)}-Ku^{(k)}\|\leq\delta.}
$$

Thus, for any fixed $k$, one can take $C=\sqrt{k\tau}$ and $\gamma=1$.

**The first constant cannot generally be chosen independently of the iteration count.** On the [l2 sequence space](../../../../../../../l2-sequence-space.md), take $(Ku)_n=u_n/n$, $\tau=1$, and noise $\eta=\delta e_n$. At $k=n^2$ the solution perturbation has [norm](../../../../../../../norm.md)

$$
\delta n\left[1-\left(1+\frac1{n^2}\right)^{-n^2}\right]
\sim(1-e^{-1})\delta n.
$$

This disproves a uniform-in-$k$ interpretation of the stated first estimate. For a closed [operator range](../../../../../../../range-of-a-bounded-linear-operator.md), boundedness of the [Moore–Penrose inverse of an operator](../../../../../../../moore-penrose-inverse-of-an-operator.md) instead supplies the uniform constant $\|K^\dagger\|$.

## ↑ Ancestors (12)

1. [B](../b.md)
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
