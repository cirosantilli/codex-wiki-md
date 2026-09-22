<h1 id="13e/solution">Solution</h1>

↑ **Parent:** [13E](../13e.md)

Cauchy's formula gives $|f'(z_0)|\le M_R/R$ for an [entire function](../../../../../entire-function.md) bounded by $M$ on every radius-$R$ circle. If $f$ is globally bounded, letting $R\to\infty$ gives $f'=0$, proving Liouville's theorem.

Set $h(w)=f(1/w)$. Its [limit](../../../../../limit-of-a-function.md) at zero makes the singularity removable, so

$$
h(w)=a+c_1w+c_2w^2+\cdots.
$$

Consequently $f(z)=a+c_1/z+O(z^{-2})$ and $z^2f'(z)\to-c_1=:b$.

The [argument principle](../../../../../argument-principle.md) on a large circle gives number of zeros minus poles equal to the winding number of $g$, which is zero because $g\to1$. Thus $m=n$. The [function](../../../../../function-split.md)

$$
G(z)=g(z)\frac{\prod_i(z-p_i)}{\prod_j(z-q_j)}
$$

has removable singularities everywhere and tends to one at infinity. Liouville gives $G=1$, hence

$$
\boxed{g(z)=\frac{\prod_j(z-q_j)}{\prod_i(z-p_i)}.}
$$

## ↑ Ancestors (10)

1. [13E](../13e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
