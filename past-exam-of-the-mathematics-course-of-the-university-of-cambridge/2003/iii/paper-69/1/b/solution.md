<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At a sampling point $j/n$, the given [polynomial](../../../../../../polynomial-split.md) has value $f_{nm}(j/n)=n^{-m}j^{\underline m}$, where $j^{\underline m}=j(j-1)\cdots(j-m+1)$ is a [falling factorial](../../../../../../falling-factorial.md). It vanishes when $j<m$. The [binomial coefficient](../../../../../../binomial-coefficient.md) identity $j^{\underline m}\binom nj=n^{\underline m}\binom{n-m}{j-m}$ therefore gives

$$
\begin{aligned}
B_n(f_{nm},x)&=\frac{n^{\underline m}}{n^m}\sum_{j=m}^n\binom{n-m}{j-m}x^j(1-x)^{n-j}\\
&=\frac{n^{\underline m}}{n^m}x^m\sum_{r=0}^{n-m}\binom{n-m}{r}x^r(1-x)^{n-m-r}\\
&=\boxed{f_{nm}(1)x^m}.
\end{aligned}
$$

The last step is the [binomial theorem](../../../../../../binomial-theorem.md), and $n^{\underline m}/n^m=\prod_{r=0}^{m-1}(1-r/n)=f_{nm}(1)$. For $m=0$ the empty product is one and the identity is simply $B_n1=1$. This is the [Bernstein falling-factorial identity](../../../../../../bernstein-falling-factorial-identity.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
