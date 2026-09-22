<h1 id="b/7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Each row sum is a sum of $k$ independent random signs. For $s>0$, its moment generating [function](../../../../../../function-split.md) is

$$
\mathbb Ee^{sY_j}=(\cosh s)^k\le e^{ks^2/2}.
$$

For example, $\log\cosh s\le s^2/2$ follows by integrating $\tanh s\le s$ for $s\ge0$. [Markov's inequality](../../../../../../markov-s-inequality.md) yields $\mathbb P(Y_j\ge t)\le\exp(-st+ks^2/2)$. Choosing $s=t/k$ gives $e^{-t^2/(2k)}$ for $t>0$. The distribution is symmetric, so the same bound applies to its negative tail. A [union bound](../../../../../../boole-s-inequality.md) proves

$$
\boxed{\mathbb P(|Y_j|\ge t)\le2e^{-t^2/(2k)}}
$$

for $t\ge0$, including the trivial endpoint $t=0$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
