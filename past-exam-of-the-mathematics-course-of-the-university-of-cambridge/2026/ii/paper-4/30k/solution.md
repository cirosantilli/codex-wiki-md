<h1 id="30k/solution">Solution</h1>

↑ **Parent:** [30K](../30k.md)

[Gradient](../../../../../gradient.md) boosting initializes a constant score and iterates: compute logistic negative [gradients](../../../../../gradient.md) $r_i^{(m)}=2y_i/[1+e^{2y_if_{m-1}(x_i)}]$ (for loss $\log(1+e^{-2yf})$), fit the base regressor $h_m$ to these pseudo-responses, choose a line-search step, and set $f_m=f_{m-1}+\nu\rho_mh_m$. For a stump $\beta\operatorname{sgn}(x_j-\alpha)$, sort each coordinate once. Sweeping the $n-1$ split positions while maintaining left and right sums gives the optimal $\beta$ and squared error in $O(n)$ per coordinate, hence $O(np)$ overall.

## ↑ Ancestors (10)

1. [30K](../30k.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
