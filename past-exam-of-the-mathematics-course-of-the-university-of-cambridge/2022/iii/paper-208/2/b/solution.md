<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [bounded differences property](../../../../../../bounded-differences-property.md) with constants $c_i$ means

$$
|f(x)-f(x')|\leq c_i
$$

whenever $x$ and $x'$ differ only in coordinate $i$. Conditional on $X_{-i}$, the range of $Z$ is therefore at most $c_i$. The range bound on variance gives

$$
\operatorname{Var}(Z\mid X_{-i})\leq\frac{c_i^2}{4}.
$$

Substitution into the [Efron–Stein inequality](../../../../../../efron-stein-inequality.md) yields

$$
\boxed{\operatorname{Var}(Z)\leq\frac14\sum_{i=1}^nc_i^2.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
