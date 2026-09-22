# Frobenius rank inequality

↑ **Parent:** [Rank inequality for a composition](rank-inequality-for-a-composition.md)

For compatible [matrices](matrix.md) $P,Q,R$, the inequality is $\operatorname{rank}(PQ)+\operatorname{rank}(QR)\leq\operatorname{rank}(Q)+\operatorname{rank}(PQR)$. One proof uses the block [matrix](matrix.md) $M=\begin{pmatrix}PQ&0\\Q&QR\end{pmatrix}$. Subtract $P$ times its lower block row from its upper block row and then subtract its first block column times $R$ from its second. The result is $\begin{pmatrix}0&-PQR\\Q&0\end{pmatrix}$, with rank $\operatorname{rank}(Q)+\operatorname{rank}(PQR)$. On the other hand, choose independent columns of $PQ$ from the first block column and independent columns of $QR$ from the second. The corresponding columns of $M$ are independent: project a relation onto the upper block first, and then onto the lower block. Thus $\operatorname{rank}(M)\geq\operatorname{rank}(PQ)+\operatorname{rank}(QR)$.

## ↑ Ancestors (6)

1. [Rank inequality for a composition](rank-inequality-for-a-composition.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/9e/solution.md)
