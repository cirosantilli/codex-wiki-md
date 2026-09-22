<h1 id="18d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Insert an exact solution into the [linear multistep method](../../../../../../linear-multistep-method.md) and use $f(t,y(t))=y'(t)$. Its local residual is

$$
R_h(t)=\sum_{\ell=0}^s\rho_\ell y(t+\ell h)-h\sum_{\ell=0}^s\sigma_\ell y'(t+\ell h).
$$

Expanding both terms by [Taylor theorem](../../../../../../taylor-theorem.md) gives

$$
R_h(t)=C_0y(t)+\sum_{k=1}^p\frac{h^k}{k!}C_k y^{(k)}(t)+O(h^{p+1}),\qquad C_0=\sum_\ell\rho_\ell,\quad C_k=\sum_\ell\ell^k\rho_\ell-k\sum_\ell\ell^{k-1}\sigma_\ell.
$$

Consequently $C_0=\cdots=C_p=0$ is sufficient for order at least $p$. It is also necessary: test the residual on the polynomials $y(t)=1,t,\ldots,t^p$, evaluating at $t=0$. For $y(t)=t^k$, it equals $h^k C_k$ (and equals $C_0$ for the constant), which can be $O(h^{p+1})$ only if $C_k=0$. These functions can be realized as exact solutions of suitable smooth [ordinary differential equations](../../../../../../ordinary-differential-equation.md), so this is a genuine necessity test. Thus **the order conditions are**

$$
\boxed{\sum_{\ell=0}^s\rho_\ell=0,\qquad \sum_{\ell=0}^s\ell^k\rho_\ell=k\sum_{\ell=0}^s\ell^{k-1}\sigma_\ell\quad(1\leq k\leq p).}
$$

This is a statement about local order; [zero-stability](../../../../../../zero-stability.md) is the separate condition that turns it into convergent approximation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18D](../../18d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
