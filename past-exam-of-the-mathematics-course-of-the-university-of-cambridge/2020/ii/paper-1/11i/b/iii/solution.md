<h1 id="11i/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For column $j$, let $N_j$ of the $M$ codewords have a one. A pair contributes a one in that column exactly when one word is chosen from those $N_j$ words and the other from the remaining $M-N_j$. Hence column $j$ contains

$$
N_j(M-N_j)
$$

ones among all pairwise sums. Part (i), summed over the $n$ columns, gives the upper bound

$$
\#1(A)\le
\begin{cases}
nM^2/4,&M\text{ even},\\
n(M^2-1)/4,&M\text{ odd}.
\end{cases}
$$

There are $\binom M2$ rows, one for each unordered pair of codewords. By part (ii), every row has weight equal to that pair's distance, which is at least $d$. Therefore

$$
\boxed{\#1(A)\ge d\binom M2=\frac{dM(M-1)}2}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [11I](../../../11i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
