<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let an $m$-clique on vertex set $Z$ belong to

$$
\delta_\cap(\langle A\rangle,\langle B\rangle)
=(\langle A\rangle\cap\langle B\rangle)-\langle A\cap B\rangle.
$$

Then $Z$ contains minimal members $X\in A$ and $Y\in B$, but contains no member of $A\cap B$. If $|X\cup Y|\leq l$, upward closure of both closed families would put $X\cup Y$ in $A\cap B$, a contradiction. Hence $|X\cup Y|>l$, so either $|X|>l/2$ or $|Y|>l/2$.

Using the minimal-member bound from part (ii), the number of possible $Z$ is at most

$$
2\sum_{k=\lceil(l+1)/2\rceil}^l
(r-1)^k\binom{n-k}{m-k}.
$$

After division by $\binom nm$ and use of $2(r-1)m\leq n$, this is at most

$$
\boxed{2\binom nm
\sum_{k=\lceil(l+1)/2\rceil}^\infty2^{-k}
\leq4\,2^{-l/2}\binom nm.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
