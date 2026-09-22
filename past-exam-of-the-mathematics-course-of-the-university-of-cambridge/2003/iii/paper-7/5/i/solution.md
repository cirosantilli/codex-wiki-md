<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Boolean function](../../../../../../boolean-function.md) takes each vector of bits to either zero or one. Use independent uniform input bits; the [influence of a variable](../../../../../../influence-of-a-variable.md) is the probability that flipping that bit changes the value. A [quite fair Boolean function](../../../../../../quite-fair-boolean-function.md) has $1/4\leq\mathbb Ef\leq3/4$. All logarithms in the estimates below are natural, except where a base is explicitly written.

Here is a [balanced tribes construction with unused coordinates](../../../../../../balanced-tribes-construction-with-unused-coordinates.md) valid for every $n\geq2$. For each $w\geq1$ put $m_w=\lfloor(\log2)2^w\rfloor$, and choose the largest $w$ with $wm_w\leq n$. Partition $wm_w$ of the bits into $m=m_w$ blocks of size $w$. Let $f$ be one when at least one block is all ones, and ignore the other bits. This is a [tribes function](../../../../../../tribes-function.md). With $s=2^{-w}$, its zero probability is $(1-s)^m$.

For $w=1$ the function is a single bit and has mean $1/2$. For $w\geq2$, $m s\leq\log2$ and $m s\geq\log2-s$. The elementary inequalities $-s/(1-s)\leq\log(1-s)\leq-s$ give

$$
(1-s)^m\geq\exp\left(-\frac{\log2}{1-s}\right)\geq\frac14,\qquad (1-s)^m\leq e^{-\log2+s}\leq\frac{e^{1/4}}2<\frac34.
$$

Thus both output probabilities are between one quarter and three quarters.

A used bit is pivotal exactly when the other $w-1$ bits of its block are one and every other block fails. Hence its influence is $2^{1-w}(1-2^{-w})^{m-1}\leq2^{1-w}$; unused bits have zero influence. Maximality of $w$ gives $n<(w+1)m_{w+1}\leq(w+1)(\log2)2^{w+1}$. Also $w\leq\log_2n$ for $n\geq2$: this is immediate for $w=1$, while for $w\geq2$ one has $wm_w\geq2^w$. Therefore

$$
\operatorname{Inf}_j(f)\leq2^{1-w}<\frac{4(\log2)(w+1)}n\leq\frac{4(\log n+\log2)}n\leq\boxed{\frac{8\log n}n<\frac{10\log n}n}.
$$

This proves the requested existence with room in the constant. The dimension-one boundary case cannot satisfy the printed logarithmic bound: a quite fair function of one bit is nonconstant and has influence one, whereas $10\log1=0$. Thus the statement requires the usual nontrivial range $n\geq2$ (or its intended large-$n$ interpretation).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
