<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $m=|w|$ and $\ell=|r|$. In fact minimality yields the stronger bound $m\leq\lfloor\ell/2\rfloor$. Suppose instead that

$$
m\geq k:=\lfloor\ell/2\rfloor+1.
$$

Because $|u|>\ell/2$, the first $k$ letters of the matched segment $u$ form a [relator](../../../../../../relator.md) segment $v$ of length $k$. They also form a segment of the periodic word $w^n$. Since $k\leq m$, that segment is contained in one cyclic permutation $w'$ of $w$, starting at the same position in the period. A cyclic permutation represents a conjugate and has length $m$.

Rotate the symmetrized [relator](../../../../../../relator.md) to write it as $vs$. Replacing the prefix $v$ of $w'$ by $s^{-1}$ preserves the represented element and gives a word of length at most

$$
m-k+(\ell-k)=m+\ell-2k<m.
$$

[Free reduction](../../../../../../free-reduction.md) can only shorten further. This contradicts the choice of $w$. Thus

$$
\boxed{|w|\leq\lfloor|r|/2\rfloor\leq |r|/2+2.}
$$

The periodic-segment argument treats matches that cross a boundary between copies of $w$; it would be incorrect simply to assume that the entire long segment $u$ lies in the original written copy of $w$. 

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
