<h1 id="38a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $A$ be the interior-grid [matrix](../../../../../../matrix.md) representing $\Gamma_9$, with zero boundary error. It is real symmetric and has the stated [sine](../../../../../../sine.md) eigenbasis. Put $s=\sin^2(k\pi h/2)$ and $t=\sin^2(\ell\pi h/2)$; the negative of its [eigenvalue](../../../../../../eigenvalue.md) is

$$
-\lambda_{k\ell}=4s+4t-\frac83st.
$$

This increases in each variable on $[0,1]^2$. With $s_1=\sin^2(\pi h/2)\geq h^2$, the smallest absolute [eigenvalue](../../../../../../eigenvalue.md) is at least $8s_1-(8/3)s_1^2\geq(16/3)h^2$. Hence its [Euclidean norm](../../../../../../euclidean-norm.md) [operator norm](../../../../../../operator-norm.md) satisfies

$$
\|A^{-1}\|_2\leq\frac3{16h^2}.
$$

The corrected scheme has an unscaled residual $r$ whose individual entries are uniformly $O(h^6)$. There are $m^2$ entries and $m<h^{-1}$, so $\|r\|_2=O(h^5)$. Subtracting the exact nodal equations from the numerical equations gives $Ae=-r$ (with sign depending on the residual convention), and therefore

$$
\boxed{\|e\|_2\leq\|A^{-1}\|_2\|r\|_2=O(h^3).}
$$

Choose a constant slightly larger than the resulting bound to obtain the requested strict $\|e\|<ch^3$ for all sufficiently small $h$. Uniform smoothness is needed for an $h$-independent constant; unspecified smoothness only in the interior would not by itself guarantee it.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [38A](../../38a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
