<h1 id="1/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We use [mathematical induction](../../../../../../../mathematical-induction.md) on $n$. The identity is immediate for the empty partition. Add a removable corner $(r,s)$ to a partition of $n-1$, and put $c=s-r$. Only the new hook and the hooks to its left in row $r$ or above it in column $s$ change. Each old affected hook length increases by one. If $S$ is the sum of those old hook lengths, direct substitution in the hook formula gives

$$
S=\sum_{j<s}(s-j+\lambda'_j-r)
+\sum_{i<r}(\lambda_i-s+r-i)
=n-\frac{r+s}{2}+\frac{(s-r)^2}{2}.
$$

There are $r+s-2$ affected old hooks, so the increase in the sum of squared hook lengths is

$$
1+(r+s-2)+2S=2n-1+c^2.
$$

The increase in $n^2+\sum c_{i,j}^2$ is likewise $n^2-(n-1)^2+c^2=2n-1+c^2$. The induction closes and proves

$$
\boxed{\sum_{(i,j)\in\lambda}h_{i,j}^2
=n^2+\sum_{(i,j)\in\lambda}c_{i,j}^2.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Paper 160](../../../../paper-160-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
