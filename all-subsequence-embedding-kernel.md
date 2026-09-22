# All-subsequence embedding kernel

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel-split.md)

Here $\phi_u(x)$ counts increasing position embeddings of the word $u$ as a [subsequence](subsequence.md) of $x$. Counting embeddings retains repeated-letter multiplicities. The empty word has one embedding in every string. Prefix [dynamic programming](dynamic-programming.md) computes this [positive-semidefinite kernel](positive-semidefinite-kernel-split.md) by $F(i,j)=F(i-1,j)+F(i,j-1)-F(i-1,j-1)+\mathbf1_{\{x_i=y_j\}}F(i-1,j-1)$ with boundary values one. The [time complexity](time-complexity.md) is $O(|x||y|)$ arithmetic operations, and rolling rows require $O(\min(|x|,|y|))$ integer cells. Counting pairs of position subsets bounds output bit length by $O(|x|+|y|)$.

## ↑ Ancestors (5)

1. [Positive-semidefinite kernel](positive-semidefinite-kernel-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-learning-theory/2/d/solution.md)
