<h1 id="2/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the [residual of an inverse problem](../../../../../../../residual-of-an-inverse-problem.md) as $r_k=Ku_\delta^{(k)}-f^\delta$. The iteration can be rearranged as

$$
u_\delta^{(k+1)}-u_\delta^{(k)}=-\tau K^*r_{k+1}.
$$

Applying $K$ gives $(I+\tau KK^*)r_{k+1}=r_k$. Since $KK^*$ is a [positive operator](../../../../../../../positive-operator.md), its [resolvent operator](../../../../../../../resolvent-of-an-operator.md) $(I+\tau KK^*)^{-1}$ has [operator norm](../../../../../../../operator-norm.md) at most one. Hence

$$
\boxed{\|r_{k+1}\|\leq\|r_k\|.}
$$

More explicitly, taking the [inner product](../../../../../../../inner-product.md) of the residual equation with $r_{k+1}$ gives

$$
\|r_{k+1}\|^2+\tau\|K^*r_{k+1}\|^2
=\operatorname{Re}\langle r_k,r_{k+1}\rangle
\leq\|r_k\|\,\|r_{k+1}\|.
$$

This directly proves the same monotonicity by the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md), including the case $r_{k+1}=0$. An unresolvable data component in $\mathcal R(K)^\perp$ remains unchanged.

## ↑ Ancestors (12)

1. [D](../d.md)
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
