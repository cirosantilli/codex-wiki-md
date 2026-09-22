<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

Let $F(x)=\sqrt{2+\sqrt x}$ for $x\geq0$. This is an increasing [continuous function](../../../../../continuous-function.md). Starting at $a_1=\sqrt2$, induction gives $\sqrt2\leq a_n\leq2$: if $a_n\leq2$, then $a_{n+1}\leq\sqrt{2+\sqrt2}<2$, and every iterate is at least $\sqrt2$.

The first step has $a_2>\sqrt2=a_1$. Since $F$ is increasing, $a_n\geq a_{n-1}$ implies $a_{n+1}=F(a_n)\geq F(a_{n-1})=a_n$. Thus this [sequence](../../../../../sequence.md) is increasing and bounded above. Let $L_-=\sup_n a_n$. For every $\varepsilon>0$, a term exceeds $L_--\varepsilon$; all later terms lie between it and $L_-$. This proves convergence, the elementary [bounded monotone sequence theorem](../../../../../bounded-monotone-sequence-theorem.md).

For the second starting value, write the iterates as $b_1=4$ and $b_{n+1}=F(b_n)$. Here $b_2=2<4$. Monotonicity of $F$ propagates this inequality, so $b_n$ is decreasing. It is bounded below by $\sqrt2$ because every positive iterate is at least that value. Hence it converges to its [infimum](../../../../../infimum.md) $L_+$. From $b_2=2$ onward all terms lie in $[\sqrt2,2]$.

[Continuity](../../../../../continuous-function.md) of $F$ permits passing to each [limit](../../../../../limit-of-a-function.md) in the recurrence, giving $L_\pm^2=2+\sqrt{L_\pm}$. To prove that these [fixed points](../../../../../fixed-point.md) agree, suppose $r,s\geq\sqrt2$ both satisfy that equality. Subtracting the two equations and rationalizing gives

$$
0=(r-s)\left(r+s-\frac1{\sqrt r+\sqrt s}\right).
$$

The second factor is positive: $r+s\geq2\sqrt2$, whereas $(\sqrt r+\sqrt s)^{-1}\leq1/(2\sqrt{\sqrt2})<2\sqrt2$. Thus $r=s$. Therefore

$$
\boxed{L_-=L_+=L,\qquad \sqrt2<L<2,\qquad L^2=2+\sqrt L.}
$$

Existence has been supplied by the two convergent [sequences](../../../../../sequence.md), and the subtraction argument gives the required uniqueness in their common interval.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
