<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $h=(b-a)/n$, $g_i=g(x_i)$, and $z_0=0$. Under the endpoint-slope convention suggested by the requested connection, the recurrence is $z_{i+1}=z_i+\tfrac h2(g_i+g_{i+1})$. Summing telescopes, so

$$
\boxed{z_n=\frac{b-a}{n}\left[\frac{g_0+g_n}2+\sum_{i=1}^{n-1}g_i\right]=T_n(g).}
$$

Since $G(b)=\int_a^b g(x)\,dx$ by the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md), this recurrence gives exactly the [composite trapezoidal rule](../../../../../composite-trapezoidal-rule.md). It replaces the average derivative over each strip by the arithmetic mean of its endpoint derivatives.

**For the standard [midpoint method](../../../../../midpoint-method.md), the literal endpoint-only request is not valid for general $g$.** Both the explicit and implicit one-step midpoint formulas here give instead

$$
\boxed{z_n=h\sum_{i=0}^{n-1}g(x_i+h/2)=M_n(g),}
$$

the [composite midpoint quadrature rule](../../../../../composite-midpoint-quadrature-rule.md). It requires half-grid samples. These samples cannot be recovered exactly from $g_0,\ldots,g_n$ for arbitrary smooth $g$: the zero function and $g(x)=\prod_{j=0}^n(x-x_j)^2$ have identical grid values but different midpoint sums. For a smooth $g$, replacing each half-grid sample by $(g_i+g_{i+1})/2$ is an additional approximation, giving $T_n$ with an $O(h^2)$ total difference, rather than an identity. A precise useful relation, obtained by splitting the finer trapezoidal sum into old nodes and midpoints, is

$$
\boxed{T_{2n}(g)=\tfrac12[T_n(g)+M_n(g)],\qquad M_n(g)=2T_{2n}(g)-T_n(g).}
$$

Here $T_{2n}$ uses the finer half-grid, so it does not eliminate the missing data.

If “Mid-Point Method” means the two-step [explicit midpoint linear multistep method](../../../../../explicit-midpoint-linear-multistep-method.md), the recurrence is $z_{i+1}=z_{i-1}+2hg_i$. It gives $z_{2r}=2h\sum_{j=1}^{r}g_{2j-1}$ and $z_{2r+1}=z_1+2h\sum_{j=1}^{r}g_{2j}$, so an odd final index additionally needs a starting value $z_1$. For even $n=2r$, the result is the midpoint quadrature on $r$ double-width strips; equivalently $z_n=2T_n-T_{n/2}$. The question specifies neither even $n$ nor a starter. Thus the trapezoidal expression above is the natural endpoint-average interpretation, while the other common midpoint meanings require the qualifications just given. The ambiguity is present in the original PDF.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
