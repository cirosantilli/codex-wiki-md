<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a sequence $J$ in $\mathbb F_p^2$, write $(r\mid J)$ for the number of $r$-term subsequences whose sum is zero. We use the following consequence of the [Chevalley-Warning theorem](../../../../../../chevalley-warning-theorem.md): if $|J|=3p-1$, then

$$
\boxed{1-(p\mid J)+(2p\mid J)\equiv0\pmod p.}
$$

Indeed, with one variable $x_i$ for each term $(a_i,b_i)$, apply Chevalley--Warning to

$$
\sum_i x_i^{p-1},
\qquad
\sum_i a_ix_i^{p-1},
\qquad
\sum_i b_ix_i^{p-1}.
$$

Their degree sum is $3(p-1)<3p-1$. A common zero has support of size $0,p$, or $2p$ modulo $p$, and each fixed support contributes $(p-1)^{|S|}$ assignments. Reducing modulo $p$ gives the displayed congruence.

Now let the given $3p$ terms have total sum zero. If no $p$ of them summed to zero, delete any one term and apply the congruence to the remaining $3p-1$ terms. It gives

$$
(2p\mid J)\equiv-1\pmod p,
$$

so those remaining terms contain a zero-sum $2p$-subsequence. Its complement in the original $3p$ terms has size $p$ and sum zero, contradicting the assumption. Therefore the required $p$ terms exist.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
