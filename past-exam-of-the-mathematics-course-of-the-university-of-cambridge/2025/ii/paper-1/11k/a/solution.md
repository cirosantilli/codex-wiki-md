<h1 id="11k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Huffman's algorithm repeatedly merges the two least probable current symbols, labels the two new edges $0,1$, and replaces the pair by a compound symbol whose probability is their sum. Reading paths from the final root gives a prefix code.

For optimality, first observe that in some optimal full binary tree the two least probable symbols are sibling leaves at maximum depth: exchange them with any deepest sibling pair, putting the smaller probabilities at no smaller depths, without increasing expected length. Contract that sibling pair to one symbol of combined probability. The original expected length equals the contracted tree's expected length plus the pair's combined probability. Induction on the alphabet size now proves that choosing the two least probabilities and recursing is optimal, which is precisely Huffman's algorithm.

If a symbol has length one, it must be $a_1$. At the three-weight stage, the other two weights $x,y$ must be merged while $p_1$ survives, so $x,y\leq p_1$. Thus $1-p_1=x+y\leq2p_1$, proving $p_1\geq1/3$. Therefore $p_1<1/3$ forces every length to be at least two.

For the other bound, suppose $p_1$ is first merged at the three-weight stage, with weights $p_1,q,r$, where $q\leq p_1\leq r$. The preceding merge created $r=x+y$ from two weights no larger than the surviving $q$, so $r\leq2q$. Since also $r\geq p_1$, we have $q\geq p_1/2$, and hence

$$
1=p_1+q+r\geq p_1+\frac{p_1}{2}+p_1=\frac52p_1.
$$

Thus this can happen only when $p_1\leq2/5$. If $p_1>2/5$, it survives until the final merge and receives a length-one word. At equality, ties can support either tree shape.

For code (a), take

$$
 (p_1,p_2,p_3,p_4)=\left(\frac25,\frac15,\frac15,\frac15\right).
$$

Huffman merging produces lengths $(1,2,3,3)$ and expected length $2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11K](../../11k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
