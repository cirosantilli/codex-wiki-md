<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Addition preserves the condition because

$$
\operatorname{ord}(a_n+b_n)\geq
\min\{\operatorname{ord}(a_n),\operatorname{ord}(b_n)\}.
$$

For multiplication, write $c_n=\sum_{i+j=n}a_ib_j$. Given $q$, choose $N$ so that $a_i,b_i\in p^q\mathbb Z_p$ for $i\geq N$. If $n\geq2N$, every pair $i+j=n$ has $i\geq N$ or $j\geq N$, so every summand lies in $p^q\mathbb Z_p$. Hence $\operatorname{ord}(c_n)\to\infty$, proving that $\mathbb Z_p\langle T\rangle$ is a subring of the [formal power series ring](../../../../../../formal-power-series.md) $\mathbb Z_p[[T]]$.

The $(p)$-adic completion is

$$
\widehat{\mathbb Z[T]}
=\varprojlim_q\mathbb Z[T]/p^q\mathbb Z[T]
=\varprojlim_q(\mathbb Z/p^q\mathbb Z)[T].
$$

A compatible system of polynomials determines coefficients $a_n\in\mathbb Z_p$. For each $q$, its reduction has finite degree, so all but finitely many $a_n$ lie in $p^q\mathbb Z_p$. This is exactly $\operatorname{ord}(a_n)\to\infty$. Conversely, every such restricted series reduces modulo $p^q$ to a polynomial and hence defines a compatible system. Therefore

$$
\boxed{\widehat{\mathbb Z[T]}^{(p)}\simeq\mathbb Z_p\langle T\rangle.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
