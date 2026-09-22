<h1 id="33c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Adopt the boundary convention $a_0=a_n=0$. Since $L$ has nonzero entries only on its first off-diagonals and $B$ only on its second off-diagonals, $BL$ and $LB$ can contribute to $[B,L]$ only on the first and third off-diagonals. On the upper first off-diagonal,

$$
(BL)_{j,j+1}=a_ja_{j+1}^2,
\qquad
(LB)_{j,j+1}=a_{j-1}^2a_j,
$$

so

$$
[B,L]_{j,j+1}=a_j(a_{j+1}^2-a_{j-1}^2).
$$

The lower first off-diagonal is equal to this by part (a). On the third off-diagonal the two products cancel:

$$
(BL)_{j,j+3}=a_ja_{j+1}a_{j+2}=(LB)_{j,j+3}.
$$

The diagonal and every remaining entry vanish. Therefore, if

$$
c_j=a_j(a_{j+1}^2-a_{j-1}^2),
$$

then

$$
\boxed{
[B,L]=
\begin{pmatrix}
0&c_1&0&\
c_1&0&c_2&\
0&c_2&0&\
&&&\ddots
\end{pmatrix}.
}
$$

This is the commutator calculation in the [Zero-diagonal Jacobi Lax pair for the finite Volterra lattice](../../../../../../../zero-diagonal-jacobi-lax-pair-for-the-finite-volterra-lattice.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [33C](../../../33c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
