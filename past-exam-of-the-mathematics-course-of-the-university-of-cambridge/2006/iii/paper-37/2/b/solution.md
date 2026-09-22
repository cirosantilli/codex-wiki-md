<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use the [Van den Berg-Kesten inequality](../../../../../../van-den-berg-kesten-inequality.md): for increasing events $A,B$ under independent [bond percolation](../../../../../../bond-percolation-split.md), their disjoint occurrence $A\mathbin\square B$, meaning that they have disjoint sets of open [edges](../../../../../../edge-of-a-graph.md) witnessing the two events, satisfies $\mathbb P_p(A\mathbin\square B)\le\mathbb P_p(A)\mathbb P_p(B)$. The finite-edge statement applies here; connection to a finite-box boundary can always be witnessed before the first exit from that box.

On the event $0\leftrightarrow\partial\Lambda_{m+n}$ choose a simple open path to that boundary, and let $y$ be its first point on $\partial\Lambda_m$. Its initial segment witnesses $0\leftrightarrow\partial\Lambda_m$ through $y$, inside $\Lambda_m$. The remaining segment eventually reaches maximum-norm distance at least $n$ from $y$, because its endpoint has norm $m+n$ while $\|y\|_\infty=m$. Stop that segment when it first reaches $y+\partial\Lambda_n$. These two segments use disjoint [edges](../../../../../../edge-of-a-graph.md).

For fixed $y$, let $A_y$ be connection from zero to $y$ inside $\Lambda_m$, and $B_y$ be connection from $y$ to $y+\partial\Lambda_n$ inside $y+\Lambda_n$. Then $\mathbb P_p(A_y)\le\beta_m$ and, by translation invariance, $\mathbb P_p(B_y)=\beta_n$. The [union bound](../../../../../../boole-s-inequality.md) and the stated disjoint-occurrence inequality give

$$
\boxed{\beta_{m+n}\le\sum_{y\in\partial\Lambda_m}\mathbb P_p(A_y\mathbin\square B_y)\le|\partial\Lambda_m|\beta_m\beta_n.}
$$

Set $x_n=\log\beta_n$ and $\alpha_n=\log|\partial\Lambda_n|$. The previous part applies, since

$$
|\partial\Lambda_n|=(2n+1)^d-(2n-1)^d=O_d(n^{d-1}),\qquad \alpha_n/n\longrightarrow0.
$$

Moreover a straight path of $n$ open bonds has [probability](../../../../../../probability.md) $p^n$, so $p^n\le\beta_n\le1$. Thus the limit is finite and

$$
\boxed{\gamma=\lim_{n\to\infty}\frac{\log\beta_n}{n}\in[\log p,0],\qquad
\beta_n\ge|\partial\Lambda_n|^{-1}e^{n\gamma}.}
$$

Equivalently, for the nonnegative decay rate $\kappa=-\gamma$, the bound is $\beta_n\ge|\partial\Lambda_n|^{-1}e^{-n\kappa}$.

The printed final exponent has the opposite sign while retaining the definition of $\gamma$ as the limit of $n^{-1}\log\beta_n$. With that definition it cannot be correct in general. Indeed, if $(2d-1)p<1$, count self-avoiding paths of length $\ell\ge n$ to get

$$
\beta_n\le\sum_{\ell\ge n}2d(2d-1)^{\ell-1}p^\ell
=\frac{2d}{2d-1}\frac{((2d-1)p)^n}{1-(2d-1)p}.
$$

Hence $\gamma\le\log((2d-1)p)<0$. A lower bound with $e^{-n\gamma}$ would eventually exceed one, because the boundary factor grows only polynomially. **The valid bound is the boxed expression with $e^{n\gamma}$, or the equivalent expression using $\kappa=-\gamma$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
