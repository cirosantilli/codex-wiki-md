<h1 id="p/p3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**The printed product omits the node with index zero.** The correct cardinal polynomial is

$$
L_k(x)=\prod_{\substack{0\le i\le n\\i\ne k}}\frac{x-x_i}{x_k-x_i}.
$$

For example, with two nodes zero and one, values zero and one, and both derivative data zero, the printed index range gives $L_1=1$ and its displayed interpolant is the constant one, which fails the value condition at zero. Thus the source formula cannot be proved literally.

With the corrected product, $L_k(x_j)=\delta_{kj}$. For $j\ne k$, $L_k^2$ has a double zero at $x_j$, so both [basis](../../../../../basis.md) functions and their derivatives vanish there. At $x_k$, put $\ell=L_k'(x_k)$. The value [basis](../../../../../basis.md) $H_k=L_k^2[1-2(x-x_k)\ell]$ satisfies $H_k(x_k)=1$ and $H_k'(x_k)=2\ell-2\ell=0$. The derivative [basis](../../../../../basis.md) $K_k=L_k^2(x-x_k)$ satisfies $K_k(x_k)=0$ and $K_k'(x_k)=1$. Both have degree at most $2n+1$. Consequently

$$
\boxed{h(x)=\sum_{k=0}^n(f_kH_k(x)+g_kK_k(x))}
$$

has every prescribed value and derivative, proving membership in the interpolation class after the required index correction. This corrected Hermite interpolant is used in the following parts.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
