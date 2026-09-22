<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Each of the three input values has two possible outputs, so their union has at most six elements. The preceding union formula also gives this bound. Choose noise values $0,3$, whose two translated input [alphabets](../../../../../alphabet.md) are disjoint. With columns ordered $0,1,2,3,4,5$ the [transition matrix](../../../../../stochastic-matrix.md) is

$$
M=\begin{pmatrix}
1/2&0&0&1/2&0&0\\
0&1/2&0&0&1/2&0\\
0&0&1/2&0&0&1/2
\end{pmatrix}.
$$

Thus **$|\mathcal Y|=6$**. Every output determines its input, explicitly $X=Y\bmod3$, so $H(X\mid Y)=0$. Consequently $I(X;Y)=H(X)\leq\log_2 3$, with equality for a uniform input. Therefore

$$
\boxed{C=\log_2 3\ \text{bits per use},\qquad p_X=(1/3,1/3,1/3).}
$$

The extra uncertainty of which noise value occurred does not reduce information about the input: the two possible outputs for each input remain distinguishable from those of every other input.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
