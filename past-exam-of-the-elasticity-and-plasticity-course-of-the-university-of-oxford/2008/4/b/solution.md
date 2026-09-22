<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For any admissible $v$, put $q=v-w$. At endpoints $q=0$. On the [contact set](../../../../contact-set-of-an-obstacle-problem.md), $w=f$ and $v\geq f$ imply $q\geq0$, while away from contact the reaction $r=p-Tw''$ is zero. Hence $rq\geq0$ everywhere. [Integration by parts](../../../../integration-by-parts.md) gives

$$
\begin{aligned}
T\int_{-1}^1w'(v'-w')\,dx+\int_{-1}^1p(v-w)\,dx
&=\int_{-1}^1(p-Tw'')(v-w)\,dx\\
&=\int_{-1}^1r(v-w)\,dx\geq0.
\end{aligned}
$$

Rearranging proves the requested [variational inequality](../../../../variational-inequality.md). Piecewise integration is legitimate because the [slope](../../../../slope.md) is continuous at the contact boundary, so there are no omitted point-force terms.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
