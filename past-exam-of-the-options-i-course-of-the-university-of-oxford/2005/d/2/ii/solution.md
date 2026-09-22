<h1 id="d/2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A useful differentiation theorem says: if $f(t,x)$ is integrable in $x$, differentiable in $t$ for almost every $x$, and on a [neighborhood](../../../../../neighbourhood-mathematics.md) of each parameter value the derivative is [bounded](../../../../../boundedness.md) in absolute value by one [integrable function](../../../../../lebesgue-integrable-function.md) of $x$, then the integral is differentiable and its derivative is the integral of $\partial_tf$. The proof applies [dominated convergence](../../../../../dominated-convergence-theorem.md) to difference quotients, [bounded](../../../../../boundedness.md) by that same majorant by the [mean value theorem](../../../../../mean-value-theorem.md).

Fix $t_0>0$ and choose $0<a<t_0<b$. For $t\in[a,b]$,

$$
|e^{-x}x^{t-1}\log x|\leq\begin{cases}x^{a-1}|\log x|,&0<x\leq1,\\ e^{-x}x^{b-1}\log x,&x\geq1.\end{cases}
$$

The first part is integrable by part (i). The second is integrable by the permitted hypothesis for $h_b$; alternatively [exponential decay](../../../../../exponential-decay.md) dominates its [polynomial](../../../../../polynomial-split.md) and logarithmic factors. The theorem therefore applies locally at every $t_0$, giving

$$
\boxed{\Gamma'(t)=\int_0^\infty e^{-x}x^{t-1}\log x\,dx\qquad(t>0).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [D](../../../d.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
