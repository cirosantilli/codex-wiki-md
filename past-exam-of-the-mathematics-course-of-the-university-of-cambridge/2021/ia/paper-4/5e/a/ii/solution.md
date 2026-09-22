<h1 id="5e/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We use induction on $k$. If $k=0$, then $\delta f=0$, so the integer-valued function $f$ is constant. For $k>0$, the integer-valued function $\delta f$ satisfies $\delta^k(\delta f)=0$. By induction it is an integer linear combination of

$$
\binom n{k-1},\binom n{k-2},\ldots,\binom n1,1.
$$

Part (i) shows that replacing each $\binom nr$ by $\binom n{r+1}$ gives an integer-valued [discrete antiderivative](../../../../../../../discrete-antiderivative.md). Subtracting the resulting integer linear combination from $f$ leaves a function with zero forward difference, hence an integer constant. This gives

$$
f(n)=c_0\binom nk+c_1\binom n{k-1}+\cdots+c_{k-1}\binom n1+c_k
$$

with every $c_j\in\mathbb Z$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5E](../../../5e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
