<h1 id="p/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The printed product omits the node $x_0$: its lower index must be zero for the stated formula to hold. For example, with $n=1$, nodes $0,1$, and data $f_0=0,f_1=1,g_0=g_1=0$, the printed $L_{1,1}=1$ gives $h=1$, which fails the first value condition. Use the corrected [Lagrange basis polynomials](../../../../../lagrange-cardinal-polynomial.md)

$$
L_k(x)=\prod_{\substack{0\le i\le n\\i\ne k}}\frac{x-x_i}{x_k-x_i}.
$$

They satisfy $L_k(x_j)=\delta_{kj}$. Define $H_k=L_k^2[1-2(x-x_k)L_k'(x_k)]$ and $K_k=L_k^2(x-x_k)$. At a node with $j\ne k$, the double zero of $L_k^2$ gives $H_k(x_j)=H_k'(x_j)=K_k(x_j)=K_k'(x_j)=0$. At $x_k$, direct differentiation gives

$$
H_k(x_k)=1,\quad H_k'(x_k)=0,\quad K_k(x_k)=0,\quad K_k'(x_k)=1.
$$

Both [polynomials](../../../../../polynomial-split.md) have degree at most $2n+1$. Consequently $h=\sum_k(f_kH_k+g_kK_k)$ has the specified values and [derivatives](../../../../../derivative.md), and is the required [Hermite interpolating polynomial](../../../../../hermite-interpolating-polynomial.md). The source product is retained literally in the private transcription; this solution identifies its necessary correction.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
