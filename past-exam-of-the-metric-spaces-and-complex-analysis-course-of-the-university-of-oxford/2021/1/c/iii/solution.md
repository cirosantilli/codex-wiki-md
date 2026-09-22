<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

For $0\leq t\leq1$, the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
|p_n(t)-p(t)|\leq\sum_k|a_{n,k}-a_k|t^k\leq\sum_k|a_{n,k}-a_k|=\rho(p_n,p).
$$

Taking the [supremum](../../../../../supremum.md) proves $\boxed{d(p_n,p)\leq\rho(p_n,p)}$. Hence convergence for $\rho$ implies convergence for $d$.

The converse is false. For $n\geq1$, take $q_n(t)=(1-t)^n/n$ and $p=0$. Its [supremum norm](../../../../../supremum-norm.md) is $d(q_n,0)=1/n\to0$, whereas the [binomial theorem](../../../../../binomial-theorem.md) gives

$$
\rho(q_n,0)=\frac1n\sum_{k=0}^n\binom nk=\frac{2^n}{n}\longrightarrow\infty.
$$

The alternating coefficients cancel on $[0,1]$; the [polynomial coefficient sum norm](../../../../../polynomial-coefficient-sum-norm.md) measures their [absolute values](../../../../../absolute-value.md) before any cancellation.

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [c](../../c.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
