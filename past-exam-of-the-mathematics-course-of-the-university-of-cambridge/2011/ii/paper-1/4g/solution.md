<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

Use [binary search](../../../../../binary-search.md): maintain the interval of possible integers and ask whether $n$ is at least the first integer in its upper half. Each answer reduces the number of possibilities to at most its previous number divided by two, rounded up. After $q$ questions at most $\lceil10^6/2^q\rceil$ possibilities remain. Since $2^{20}=1\,048\,576>10^6$, **twenty questions suffice**.

A yes/no [decision tree](../../../../../decision-tree.md) of depth twenty has at most $2^{20}$ leaves, whereas the possible finishing orders number $15!=1\,307\,674\,368\,000$. Thus **twenty questions cannot identify the finishing order of fifteen horses**, assuming no ties. With unrestricted yes/no questions, the exact minimum for $n$ horses is $\lceil\log_2(n!)\rceil$: the leaf count is a lower bound, and repeatedly partitioning the remaining [permutations](../../../../../permutation.md) into two nearly equal sets attains it. In particular fifteen horses require 41 questions.

By [Stirling's formula](../../../../../stirling-formula.md),

$$
\boxed{\log_2(n!)=n\log_2n-(\log_2e)n+\frac12\log_2(2\pi n)+O(n^{-1}),}
$$

so the leading number of questions is $n\log_2n$. These questions may ask about whole sets of possible orders; restricting them to pairwise comparisons is a different model.

## ↑ Ancestors (11)

1. [4G](../4g.md)
2. [Section I](../section-i.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
