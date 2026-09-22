<h1 id="b/4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If the first trial is accepted, $\alpha_k=\alpha_{\mathrm{init}}$. Otherwise the preceding trial was rejected and so exceeded $\alpha_{\max}$, since part (ii) guarantees acceptance below that threshold. The accepted step, reduced by the factor $\tau$, consequently exceeds $\tau\alpha_{\max}$. In either case,

$$
\alpha_k\geq\min(\alpha_{\mathrm{init}},\tau\alpha_{\max}).
$$

The angle condition $-g_k^Tp_k\geq\varepsilon\|g_k\|_2\|p_k\|_2$ gives $\alpha_{\max}\geq2\varepsilon(1-\beta)\|g_k\|_2/(\gamma\|p_k\|_2)$. Hence the [backtracking line search](../../../../../backtracking-line-search.md) has the lower bound

$$
\boxed{\alpha_k\geq\min\left(\alpha_{\mathrm{init}},\frac{2\tau\varepsilon(1-\beta)\|g_k\|_2}{\gamma\|p_k\|_2}\right).}
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
