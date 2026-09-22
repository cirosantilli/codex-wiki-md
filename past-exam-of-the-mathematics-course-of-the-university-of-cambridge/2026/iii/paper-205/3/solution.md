<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A real [positive-semidefinite kernel](../../../../../positive-semidefinite-kernel.md) is a symmetric function $k$ such that every finite Gram matrix $K_{ij}=k(x_i,x_j)$ is positive semidefinite. The [representer theorem](../../../../../representer-theorem.md) says that any minimizer in a [Reproducing kernel Hilbert space](../../../../../reproducing-kernel-hilbert-space.md) of an objective depending on $f$ only through $f(x_1),\ldots,f(x_n)$ and a strictly increasing function of $\lVert f\rVert_{\mathcal H}$ lies in

$$
\operatorname{span}\{k(x_1,\mathord\cdot),\ldots,k(x_n,\mathord\cdot)\}.
$$

Indeed, write $f=f_\parallel+f_\perp$ relative to this span. The reproducing property gives $f_\perp(x_i)=0$ for every $i$, while the [Pythagorean theorem in an inner-product space](../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives $\lVert f\rVert^2=\lVert f_\parallel\rVert^2+\lVert f_\perp\rVert^2$. Removing a nonzero perpendicular component preserves all data values and strictly decreases the penalty, proving the theorem.

Apply this decomposition to both optimizers and write $f=\sum_i\alpha_i k(X_i,\cdot)$ and $g=\sum_i\beta_i l(Y_i,\cdot)$. If $K$ and $L$ are the two [Gram matrices](../../../../../gram-matrix.md), then

$$
\sum_i f(X_i)g(Y_i)=\alpha^TKL\beta,
\qquad \lVert f\rVert_{\mathcal H}^2=\alpha^TK\alpha,
\qquad \lVert g\rVert_{\mathcal G}^2=\beta^TL\beta.
$$

Writing $u=K^{1/2}\alpha$ and $v=L^{1/2}\beta$, with pseudoinverses on the respective ranges, turns the supremum into

$$
\sup_{\lVert u\rVert_2,\lVert v\rVert_2\leq1}u^TK^{1/2}L^{1/2}v
=\sigma_{\max}(K^{1/2}L^{1/2}).
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
