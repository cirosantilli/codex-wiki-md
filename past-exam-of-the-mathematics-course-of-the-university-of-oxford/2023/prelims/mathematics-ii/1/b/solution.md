<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose $M$ with $|b_n|\leq M$. Every [tail of a sequence](../../../../../../tail-of-a-sequence.md) is nonempty and bounded, so its [supremum](../../../../../../supremum.md) $c_n$ exists and lies in $[-M,M]$. Removing one term cannot increase a [supremum](../../../../../../supremum.md), hence $c_{n+1}\leq c_n$. The [bounded monotone sequence theorem](../../../../../../bounded-monotone-sequence-theorem.md), applied to $-c_n$, proves

$$
c_n\longrightarrow L=\inf_n c_n=\limsup_{n\to\infty}b_n.
$$

Thus $L$ is the [limit superior](../../../../../../limit-superior.md) of $(b_n)$.

For $\varepsilon>0$, eventually $c_n<L+\varepsilon$, and then $b_n\leq c_n<L+\varepsilon$. Only finitely many indices can satisfy $b_n\geq L+\varepsilon$. If only finitely many satisfied $b_n>L-\varepsilon$, some entire [tail of a sequence](../../../../../../tail-of-a-sequence.md) would have $b_n\leq L-\varepsilon$. Its [supremum](../../../../../../supremum.md) would also be at most $L-\varepsilon$, contradicting $c_n\geq L$.

Inductively choose $n_k>n_{k-1}$ so late that $c_{n_k}<L+1/k$ and $b_{n_k}>L-1/k$. There are infinitely many choices for the latter inequality, so both requirements can be met. Then $|b_{n_k}-L|<1/k$, proving $\boxed{b_{n_k}\to L}$. This constructs a [subsequence](../../../../../../subsequence.md) attaining the [limit superior](../../../../../../limit-superior.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
