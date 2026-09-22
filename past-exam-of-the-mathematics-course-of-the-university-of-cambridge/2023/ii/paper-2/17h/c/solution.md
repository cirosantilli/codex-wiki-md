<h1 id="17h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $d=d(G)$ and suppose

$$
c_0I+c_1A+\cdots+c_dA^d=0.
$$

If some coefficient is nonzero, let $k$ be the largest index with $c_k\ne0$. Choose a path

$$
v_0,v_1,\ldots,v_d
$$

whose endpoints realize the [graph diameter](../../../../../../graph-diameter.md). Every initial segment is a shortest path, since a shorter route from $v_0$ to $v_k$ could be followed by the remaining segment to shorten the path from $v_0$ to $v_d$. Thus

$$
d(v_0,v_k)=k.
$$

By the [walk count from powers of an adjacency matrix](../../../../../../walk-count-from-powers-of-an-adjacency-matrix.md),

$$
(A^j)_{v_0v_k}=0\quad(j<k),
\qquad
(A^k)_{v_0v_k}>0.
$$

Taking the $(v_0,v_k)$ entry of the assumed relation and using maximality of $k$ gives

$$
c_k(A^k)_{v_0v_k}=0,
$$

a contradiction. Every coefficient is therefore zero, proving the [linear independence of adjacency powers up to the diameter](../../../../../../linear-independence-of-adjacency-powers-up-to-the-diameter.md):

$$
\boxed{I,A,A^2,\ldots,A^{d(G)}\ \text{are linearly independent}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17H](../../17h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
