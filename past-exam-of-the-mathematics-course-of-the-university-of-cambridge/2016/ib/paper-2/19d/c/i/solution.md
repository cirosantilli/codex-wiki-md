<h1 id="19d/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First rotate rows $2,3$ with $c=4/5$, $s=3/5$. The second column pair $(4,3)$ becomes $(5,0)$ and the corresponding third column pair $(1,2)$ becomes $(2,1)$. Next rotate rows $3,4$ with $c=4/5$, $s=3/5$, sending the third column pair $(1,3/4)$ to $(5/4,0)$. Thus $R=G_{34}G_{23}A$ and $Q=G_{23}^TG_{34}^T$. **One exact [QR decomposition](../../../../../../../qr-decomposition.md) is**

$$
\boxed{R=\begin{pmatrix}3&1&1\\0&5&2\\0&0&5/4\\0&0&0\end{pmatrix},\qquad
Q=\begin{pmatrix}
1&0&0&0\\
0&4/5&-12/25&9/25\\
0&3/5&16/25&-12/25\\
0&0&3/5&4/5
\end{pmatrix}.}
$$

The construction proves $Q^TQ=I$, and direct multiplication checks $QR=A$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [19D](../../../19d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
