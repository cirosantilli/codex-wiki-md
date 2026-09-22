<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Translate the output [alphabet](../../../../../alphabet.md) by $-\min(z_1,z_2)$ and put $d=|z_2-z_1|\geq1$. The reachable outputs become

$$
\{0,1,2\}\cup\{d,d+1,d+2\},\qquad |\mathcal Y|=3+\min(d,3).
$$

For $d=1$ the two sets overlap in two points; for $d=2$ in one; for $d\geq3$ they are disjoint. In particular **$|\mathcal Y|\geq4$**, and choosing noise values $0,1$ attains four.

With rows indexed by inputs $0,1,2$ and columns by outputs $0,1,2,3$, [independence](../../../../../independent-random-variables.md) and uniform two-point noise give

$$
M=\begin{pmatrix}
1/2&1/2&0&0\\
0&1/2&1/2&0\\
0&0&1/2&1/2
\end{pmatrix}.
$$

Every conditional output distribution has [information entropy](../../../../../information-entropy-split.md) one [bit](../../../../../bit.md), so $I(X;Y)=H(Y)-1\leq\log_2 4-1=1$. The input [probability mass function](../../../../../probability-mass-function.md) $(1/2,0,1/2)$ makes all four outputs equiprobable, attaining that bound. Thus

$$
\boxed{C=1\ \text{bit per use},\qquad p_X=(1/2,0,1/2).}
$$

Using a zero-probability _input_ in a channel-capacity maximization is legitimate; it is unrelated to the strictly positive source weights needed for the tree-shape claims in Question 2.

## ↑ Ancestors (13)

1. [I](../i.md)
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
