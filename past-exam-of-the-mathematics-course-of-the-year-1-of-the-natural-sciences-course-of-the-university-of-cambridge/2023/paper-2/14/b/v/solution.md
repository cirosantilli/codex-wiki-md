<h1 id="14/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For first-bin size $k$, choose its contents in $\binom6k$ ways. Each choice arises from $k!(6-k)!$ [permutations](../../../../../../permutation.md), obtained by ordering the two bins internally. The seven ordered size choices give

$$
\begin{array}{c|r|r|r}
\text{bin sizes}&\text{partitions}&\text{orderings per partition}&\text{product}\\\hline
\{0,6\}&1&720&720\\
\{1,5\}&6&120&720\\
\{2,4\}&15&48&720\\
\{3,3\}&20&36&720\\
\{4,2\}&15&48&720\\
\{5,1\}&6&120&720\\
\{6,0\}&1&720&720
\end{array}
$$

Here $0!=1$. Each row expresses the same [binomial coefficient](../../../../../../binomial-coefficient-split.md) identity $\binom6k k!(6-k)!=6!$. Even for $\{3,3\}$ the bins retain their first/second labels, so the number is twenty rather than ten; the braces denote bin sizes in the question's convention, not interchangeable bins.

## ↑ Ancestors (14)

1. [V](../v.md)
2. [B](../../b.md)
3. [14](../../../14.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
