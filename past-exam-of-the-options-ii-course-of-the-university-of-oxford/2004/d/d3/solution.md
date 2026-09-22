<h1 id="d/d3/solution">Solution</h1>

↑ **Parent:** [D3](../d3.md)

The [monotone convergence theorem](../../../../monotone-convergence-theorem.md) says that if $0\leq f_j\uparrow f$ almost everywhere on a measure space, then $\int f_j\uparrow\int f$, allowing infinity. The [dominated convergence theorem](../../../../dominated-convergence-theorem.md) says that if $g_j\to g$ almost everywhere and $|g_j|\leq H$ for an integrable $H$, then $g$ is integrable and $\int g_j\to\int g$.

For $a\ne0$, the truncated functions $f_a\mathbf1_{[-j,j]}$ increase to $f_a$. Each has the elementary integral $2\arctan(|a|j)/|a|$. Thus monotone convergence gives

$$
\boxed{\int_{\mathbb R}f_a(x)\,dx=\frac\pi{|a|}<\infty.}
$$

For fixed $x$, eventually $|x|\leq n\pi/2$ and $n\sin(x/n)\to x$, so $g_n(x)\to1/(1+x^2)$. Inside the support the supplied inequality yields $n^2\sin^2(x/n)\geq4x^2/\pi^2$. Outside the support $g_n=0$. Consequently the global bound is

$$
0\leq g_n(x)\leq\frac1{1+4x^2/\pi^2},
$$

and this majorant is integrable by the already proved formula with $a=2/\pi$. Dominated convergence now gives $\boxed{\int g_n\to\int(1+x^2)^{-1}dx=\pi}$. The majorant is independent of $n$, including on the moving support.

## ↑ Ancestors (12)

1. [D3](../d3.md)
2. [D](../../d.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
