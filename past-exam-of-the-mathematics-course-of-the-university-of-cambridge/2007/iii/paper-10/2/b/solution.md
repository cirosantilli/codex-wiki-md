<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Give $G(H)$ its natural [trace-class](../../../../../../trace-class-operator.md) topology: differentiability means $F(t+h)=F(t)+h\dot F(t)+o_1(h)$, with remainder small in [trace norm](../../../../../../trace-norm.md). The [Fredholm determinant](../../../../../../fredholm-determinant.md) is the continuous extension of finite-rank [determinants](../../../../../../determinant.md); it is multiplicative by finite-rank approximation and satisfies

$$
\det(I+K)=1+\operatorname{Tr}K+O(\|K\|_1^2)
$$

near zero. For example its exterior-power [series](../../../../../../series-mathematics.md) bounds the remainder by $e^{\|K\|_1}-1-\|K\|_1$, proving that estimate directly.

Factor $F(t+h)=F(t)[I+hF(t)^{-1}\dot F(t)+o_1(h)]$. Multiplicativity and the preceding expansion give

$$
\boxed{\frac d{dt}\det F(t)=\det F(t)\operatorname{Tr}(F(t)^{-1}\dot F(t)).}
$$

The [determinant](../../../../../../determinant.md) is nonzero for invertible $F$, so division yields the required logarithmic [derivative](../../../../../../derivative.md). Differentiability only in the bounded-operator [norm](../../../../../../norm.md) would not justify this [trace](../../../../../../matrix-trace.md) formula; the specified topology is essential.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
