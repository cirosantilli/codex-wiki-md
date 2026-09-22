<h1 id="10e/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For hitting zero before four, the success probabilities are

$$
h_i=\frac{4-i}{4}.
$$

Conditioning each transition on eventual success gives

$$
\begin{array}{c|cc}
\text{state}&\text{down}&\text{up}\\ \hline
1&2/3&1/3\\
2&3/4&1/4\\
3&1&0.
\end{array}
$$

Thus the conditional expected hitting times satisfy

$$
e_1=1+\frac13e_2,
\qquad
e_2=1+\frac34e_1+\frac14e_3,
\qquad
e_3=1+e_2.
$$

Solving this linear system gives

$$
\boxed{\mathbb E(T\mid B)=e_1=\frac73}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [10E](../../../10e.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
