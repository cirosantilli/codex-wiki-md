<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For integer knots, the recurrence simplifies to

$$
N_{i,k}(t)=\frac{t-i}{k-1}N_{i,k-1}(t)
+\frac{i+k-t}{k-1}N_{i+1,k-1}(t).
$$

Order-two [splines](../../../../../../spline-mathematics.md) are triangular: $N_{i,2}(i)=N_{i,2}(i+2)=0$ and $N_{i,2}(i+1)=1$. Applying the recurrence once more gives

$$
\begin{array}{c|ccc}
t&1&2&3\\ \hline
N_{0,3}(t)&1/2&1/2&0\\
N_{1,3}(t)&0&1/2&1/2.
\end{array}
$$

For example $N_{0,3}(1)=\frac12N_{0,2}(1)+N_{1,2}(1)=1/2$ and $N_{0,3}(2)=N_{0,2}(2)+\frac12N_{1,2}(2)=1/2$. Thus the [Cardinal cubic B-spline](../../../../../../cardinal-cubic-b-spline.md) values are

$$
\begin{aligned}
N_{0,4}(1)&=\frac13\frac12+\frac33\,0=\frac16,\\
N_{0,4}(2)&=\frac23\frac12+\frac23\frac12=\frac23,\\
N_{0,4}(3)&=\frac33\,0+\frac13\frac12=\frac16.
\end{aligned}
$$

Therefore

$$
\boxed{(N_{0,4}(1),N_{0,4}(2),N_{0,4}(3))=(1/6,\,2/3,\,1/6).}
$$

In particular its actual maximum is $2/3$ in this standard normalization; dividing by that maximum would change the requested recurrence normalization.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
