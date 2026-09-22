<h1 id="30k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a symmetric matrix,  
$\operatorname{range}V=(\ker V)^\perp$. Since $q\notin\operatorname{range}V$, there is  
$\eta\in\ker V$ with $\eta^Tq\ne0$. For any target excess mean $h$, set

$$
\theta=\frac{h}{\eta^Tq}\eta.
$$

Then $\theta^Tq=h$ and

$$
\operatorname{Var}(X_1)=\theta^TV\theta=0.
$$

Thus the required minimum is zero for every $m,x$.

Choose the sign of $\eta$ so that $\eta^Tq>0$, buy the risky portfolio $\eta$, and finance it by borrowing its time-zero cost in the bank. Its initial wealth is zero, while its terminal excess payoff has variance zero and positive mean $\eta^Tq$, so it is a strictly positive constant almost surely. This is an [arbitrage](../../../../../../arbitrage.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30K](../../30k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
