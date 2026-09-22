<h1 id="15f/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [conjugacy classes](../../../../../../../conjugacy-class.md) are $\{1\}$, $\{a^n\}$, $\{a^r,a^{-r}\}$ for $1\leq r\leq n-1$, and two classes containing respectively $ba^{2s}$ and $ba^{2s+1}$, each of size $n$. Conjugation by $b$ inverts powers of $a$, while conjugation by $a$ changes the exponent of $ba^r$ by two; these facts prove the list and sizes. The sizes total $4n$.

The complete [character table](../../../../../../../character-table.md) is specified by the following array, with one column for every $r$ and one row for every $j$ in the indicated ranges:

$$
\boxed{\begin{array}{c|ccccc}
\text{class}&1&a^n&\{a^r,a^{-r}\}&\{ba^{2s}\}&\{ba^{2s+1}\}\\
\text{size}&1&1&2&n&n\\\hline
\chi_{\alpha,\beta}&1&\alpha^n&\alpha^r&\beta&\alpha\beta\\
\chi_j&2&2(-1)^j&2\cos(\pi jr/n)&0&0
\end{array}}
$$

Here $1\leq r,j\leq n-1$; the four pairs $(\alpha,\beta)$ are those in part (ii). In particular, this formula displays both parity cases without concealing the different values $\pm i$ when $n$ is odd. The zero entries follow because the two-dimensional [matrices](../../../../../../../matrix.md) representing $ba^r$ are off-diagonal.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [15F](../../../15f.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
