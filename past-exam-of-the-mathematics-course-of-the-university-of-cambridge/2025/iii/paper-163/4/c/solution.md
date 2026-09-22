<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set

$$
F_\tau(x)=\sum_{\substack{\theta\in\Theta(R)\\\theta\subset\tau}}f_\theta(x)w_{r^{2/3}}(x).
$$

Freeze $x_3$. In the $(x_1,x_2)$ Fourier variables, the functions $F_\tau(\cdot,\cdot,x_3)$ are supported in caps of tangential length $r^{-1/3}$ and normal width $r^{-2/3}$ along the parabola. Apply part a with decoupling scale $R'=r^{2/3}$ and critical exponent $p=6$. Since $(R')^{1/2-3/6}=1$, for each fixed $x_3$,

$$
\left\|\sum_\tau F_\tau(\cdot,\cdot,x_3)\right\|_{L^6(\mathbb R^2)}^6
\lesssim_\epsilon r^\epsilon
\left(\sum_\tau\|F_\tau(\cdot,\cdot,x_3)\|_{L^6(\mathbb R^2)}^2\right)^3.
$$

Integrate in $x_3$. Minkowski's inequality in $L^3(dx_3)$ gives

$$
\int_{\mathbb R^3}\left|\sum_\theta f_\theta w_{r^{2/3}}\right|^6
\lesssim_\epsilon r^\epsilon
\left(\sum_{\tau\in\Theta(r)}
\left(\int_{\mathbb R^3}|F_\tau|^6\right)^{2/6}\right)^{6/2},
$$

which is exactly the claimed inequality after absorbing a change in $\epsilon$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 163](../../../paper-163-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
