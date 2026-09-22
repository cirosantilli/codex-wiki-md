<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Conditional independence](../../../../../../conditional-independence.md) $A\perp B\mid D$ means that, for almost every $d$,

$$
p(a,b\mid d)=p(a\mid d)p(b\mid d),
$$

equivalently $p(a\mid b,d)=p(a\mid d)$ wherever the conditional probabilities are defined.

Now use the chain rule and both assumed independences:

$$
\begin{aligned}
p(a,b,c\mid d)
&=p(a\mid b,c,d)p(b,c\mid d)\\
&=p(a\mid b,d)p(b,c\mid d)\\
&=p(a\mid d)p(b,c\mid d).
\end{aligned}
$$

This is exactly $A\perp(B,C)\mid D$, proving the [contraction axiom for conditional independence](../../../../../../contraction-axiom-for-conditional-independence.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
