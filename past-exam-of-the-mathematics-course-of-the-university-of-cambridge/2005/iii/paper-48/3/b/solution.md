<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $h=\Delta x$, $k=\Delta t$ and march backward from the terminal payoff. At the interior grid point $(x_i,t_j)$ use

$$
D_xu_i^j=\frac{u_{i+1}^j-u_{i-1}^j}{2h},\qquad
D_{xx}u_i^j=\frac{u_{i+1}^j-2u_i^j+u_{i-1}^j}{h^2}.
$$

The [central finite difference](../../../../../../central-finite-difference.md) spatial approximation and backward-in-calendar-time [explicit Euler method](../../../../../../euler-method.md) give

$$
\boxed{u_i^{j-1}=u_i^j+k\left[a_i^j\frac{u_{i+1}^j-2u_i^j+u_{i-1}^j}{h^2}
+b_i^j\frac{u_{i+1}^j-u_{i-1}^j}{2h}\right].}
$$

Here $a_i^j=\sigma(e^{x_i},t_j)^2/2$, $b_i^j=r-a_i^j$, and $u_i^m=(e^{x_i}-K)^+$. At a far-left boundary use $u\simeq0$; at a far-right boundary the call asymptotics are $u\simeq e^{r(T-t)}e^x-K$. These boundary values are inserted into the adjacent interior updates. Smooth-solution Taylor expansion gives consistency order $O(k+h^2)$ in the evolution equation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
