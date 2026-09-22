<h1 id="12f/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose $x\in X$ and iterate $x_{n+1}=f(x_n)$. The [contraction mapping](../../../../../../../contraction-mapping.md) estimate

$$
d(x_{n+1},x_n)\leq\lambda^nd(x_1,x_0)
$$

makes $(x_n)$ Cauchy by a [geometric series](../../../../../../../geometric-series.md). Its limit $x_0$ satisfies $f(x_0)=x_0$ because $f$ is Lipschitz. Two fixed points would satisfy $d(x_0,y_0)\leq\lambda d(x_0,y_0)$, so they coincide. This proves the [Banach fixed-point theorem](../../../../../../../contraction-mapping-theorem.md).

Now suppose the final assertion failed. There would be $m_k,n_k\to\infty$ with $f(a_{m_k})=a_{n_k}$. Since $a_n\to a$ and $f$ is continuous, the two sides tend respectively to $f(a)$ and $a$, so $f(a)=a$. Uniqueness would give $a=x_0$, a contradiction. Hence the required **$\ell$ and $m$ exist**.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [12F](../../../12f.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
