<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose $R>0$ with $\operatorname{supp}\phi\subset[-R,R]$. Evenness of $f$ changes the symmetrically truncated integral into

$$
\int_{|x|>\varepsilon}\frac{f(x)}x\phi(x)\,dx
=\int_\varepsilon^R f(x)\frac{\phi(x)-\phi(-x)}x\,dx.
$$

The [mean value theorem](../../../../../mean-value-theorem.md) gives $|\phi(x)-\phi(-x)|\leq2x\|\phi'\|_\infty$. Since $f$ is continuous, it is bounded on $[0,R]$. Thus the [Cauchy principal value](../../../../../cauchy-principal-value.md) exists and

$$
\boxed{\left\langle\operatorname{pv}\frac{f(x)}x,\phi\right\rangle
=\int_0^R f(x)\frac{\phi(x)-\phi(-x)}x\,dx.}
$$

This expression is linear in the [test function](../../../../../test-function.md) and satisfies

$$
\left|\left\langle\operatorname{pv}\frac{f(x)}x,\phi\right\rangle\right|
\leq2R\max_{[0,R]}|f|\,\|\phi'\|_\infty.
$$

For each fixed [compact support](../../../../../compact-support.md), choose one $R$ once and for all. The estimate proves that the [even-weight principal-value distribution](../../../../../even-weight-principal-value-distribution.md) has [order of a distribution](../../../../../order-of-a-distribution.md) at most one.

If $\phi(0)=0$, the [mean value theorem](../../../../../mean-value-theorem.md) also gives $|\phi(x)|\leq|x|\|\phi'\|_\infty$. Hence $f(x)\phi(x)/x$ is absolutely integrable near zero and has [compact support](../../../../../compact-support.md). The truncated integrals tend to its ordinary [Lebesgue integral](../../../../../lebesgue-integral.md), so

$$
\boxed{\left\langle\operatorname{pv}\frac{f(x)}x,\phi\right\rangle
=\int_{\mathbb R}\frac{f(x)}x\phi(x)\,dx\quad\text{if }\phi(0)=0.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
