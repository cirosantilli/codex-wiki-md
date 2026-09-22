<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
q=p_0+p_1=1-p.
$$

The length process $L_n=\ell(X_n)$ is a nearest-neighbour chain on the nonnegative integers: away from zero it moves up with probability $q$ and down with probability $p$, while at zero it moves up with probability $q$ and stays put with probability $p$.

Returns of the original chain to the root are exactly returns of $L_n$ to zero, so their recurrence classifications agree. The [reflected biased random walk on the nonnegative integers](../../../../../../reflected-biased-random-walk-on-the-nonnegative-integers.md) is transient when $q>p$, null recurrent when $q=p$, and positive recurrent when $q<p$. Since $p=1-q$, the conditions are respectively

$$
\begin{array}{c|c}
\text{classification}&\text{condition}\\ \hline
\text{transient}&p_0+p_1>\tfrac12,\\
\text{null recurrent}&p_0+p_1=\tfrac12,\\
\text{positive recurrent}&p_0+p_1<\tfrac12.
\end{array}
$$

Irreducibility transfers the classification from the root to every state.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
