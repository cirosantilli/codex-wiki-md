<h1 id="4/ii/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $0\leq\epsilon<1$ and $\delta>0$. By the [asymptotic equipartition property](../../../../../../../asymptotic-equipartition-property.md), all sufficiently large $n$ satisfy $\Pr(Z^{(n)}\notin T_\delta^n)\leq(1-\epsilon)/2$. For any [epsilon-sufficient set](../../../../../../../epsilon-sufficient-set.md) $S_n$,

$$
\Pr(Z^{(n)}\in S_n\cap T_\delta^n)\geq\Pr(Z^{(n)}\in S_n)-\Pr(Z^{(n)}\notin T_\delta^n)\geq\frac{1-\epsilon}{2}.
$$

Each word in this intersection has probability at most $2^{-n(H(Z)-\delta)}$. Hence

$$
\frac{1-\epsilon}{2}\leq|S_n\cap T_\delta^n|\,2^{-n(H(Z)-\delta)}\leq|S_n|\,2^{-n(H(Z)-\delta)},
$$

which gives the [minimum size of a sufficient set for an IID source](../../../../../../../minimum-size-of-a-sufficient-set-for-an-iid-source.md):

$$
\boxed{|S_n|\geq\frac{1-\epsilon}{2}\,2^{n(H(Z)-\delta)}.}
$$

The [Chebyshev inequality](../../../../../../../chebyshev-inequality.md) used above supplies the sufficient quantitative condition $n\geq2v/[\delta^2(1-\epsilon)]$. No assumption that $S_n$ itself is a [typical set](../../../../../../../typical-set.md) is needed; its intersection with one provides the bound.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Ii](../../ii.md)
3. [4](../../../4.md)
4. [Paper 66](../../../../paper-66-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
