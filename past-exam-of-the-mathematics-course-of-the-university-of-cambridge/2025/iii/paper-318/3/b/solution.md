<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [Leibniz rule for divided differences](../../../../../../leibniz-rule-for-divided-differences.md) to $(x-t)_+^{k-1}=(x-t)(x-t)_+^{k-2}$. Only the zeroth and first divided differences of the linear factor survive. After applying the normalization, this gives the [Cox-de Boor recursion formula](../../../../../../cox-de-boor-recursion-formula.md)

$$
\boxed{N_{i,k}(t)=\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)
+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
