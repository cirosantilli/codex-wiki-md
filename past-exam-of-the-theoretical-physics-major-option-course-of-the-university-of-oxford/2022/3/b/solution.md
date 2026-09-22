<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [probability](../../../../probability.md) column vector as $\mathbf p=(p_0,p_A,p_B)^T$, with $0$ denoting the uncharged state. The arrows in the original figure give transitions $0\to A$ at rate $f_1$, $A\to B$ at rate $f_2$, $B\to0$ at rate $f_3$, and $B\to A$ at rate $f_4$. Exclusion of double occupation means injection occurs only from state $0$. Thus the [master equation](../../../../master-equation.md) is

$$
\boxed{\frac{d}{dt}\begin{pmatrix}p_0\\p_A\\p_B\end{pmatrix}=\begin{pmatrix}-f_1&0&f_3\\f_1&-f_2&f_4\\0&f_2&-(f_3+f_4)\end{pmatrix}\begin{pmatrix}p_0\\p_A\\p_B\end{pmatrix}.}
$$

For example, $\dot p_B=f_2p_A-(f_3+f_4)p_B$. Every allowed jump adds to one [probability](../../../../probability.md) and subtracts from another, which verifies the zero column sums.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
