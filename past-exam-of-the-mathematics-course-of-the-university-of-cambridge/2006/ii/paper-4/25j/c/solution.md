<h1 id="25j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a fixed $c>0$, the functions $|f_n|\mathbf1_{\{|f_n|\le c\}}$ tend pointwise to zero and are dominated by the [Lebesgue integrable](../../../../../../lebesgue-integrable-function.md) constant $c$, since $\mu(\Omega)<\infty$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) therefore gives convergence of their integrals to zero. Split

$$
\int|f_n|d\mu\le
\int |f_n|\mathbf1_{\{|f_n|\le c\}}d\mu+
\sup_k\int_{|f_k|>c}|f_k|d\mu.
$$

Take the upper limit in $n$ and then send $c\to\infty$. The specified [uniform integrability](../../../../../../uniform-integrability.md) condition makes the right side zero. It also ensures integrability of each $f_n$, by the same split for a sufficiently large $c$. Hence **$\int|f_n|d\mu\to0$**, and in particular $\int f_n d\mu\to0$.

For a counterexample without the tail condition, use Lebesgue measure on $(0,1)$ and $f_n(x)=n\mathbf1_{(0,1/n)}(x)$. Every fixed positive $x$ eventually lies outside the shrinking interval, so $f_n(x)\to0$, but $\int_0^1f_n dx=1$ for every $n$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [25J](../../25j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
