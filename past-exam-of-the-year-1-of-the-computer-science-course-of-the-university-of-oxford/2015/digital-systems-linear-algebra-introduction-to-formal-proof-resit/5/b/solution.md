<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the state order Tall, Medium, Short and **column [probability distributions](../../../../../probability-distribution-split.md)**, so that $\mathbf p_{n+1}=P\mathbf p_n$. The $j$th column records the child's [probability distribution](../../../../../probability-distribution-split.md) given parent state $j$. Thus the [transition matrix](../../../../../stochastic-matrix.md) is

$$
\boxed{P=\begin{pmatrix}
0.6&0.2&0.1\\
0.2&0.7&0.3\\
0.2&0.1&0.6
\end{pmatrix}.}
$$

Every entry is nonnegative and every column sums to one. This convention also gives the requested property $P^T(1,1,1)^T=(1,1,1)^T$. A row-distribution convention would use the transposed [transition matrix](../../../../../stochastic-matrix.md) consistently instead. The stated [Markov chain](../../../../../markov-chain-split.md) is the mathematical model to analyze; no additional biological assumptions are needed.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
