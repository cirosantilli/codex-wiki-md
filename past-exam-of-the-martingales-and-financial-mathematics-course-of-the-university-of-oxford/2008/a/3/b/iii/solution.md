<h1 id="a/3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In any proposed decomposition, $Z_n'=X_n-Y_n'$ is integrable. Its increment is $\mathcal F_{n-1}$-measurable by predictability. Taking [conditional expectation](../../../../../../conditional-expectation.md) of the difference equation gives

$$
G_n=\mathbb E(X_n-X_{n-1}\mid\mathcal F_{n-1})
=\mathbb E(Y_n'-Y_{n-1}'\mid\mathcal F_{n-1})+(Z_n'-Z_{n-1}')
=Z_n'-Z_{n-1}'.
$$

The martingale increment has conditional mean zero, and a measurable integrable variable equals its own conditional expectation. Starting from $Z_0'=0$, summation gives $Z_n'=\sum_{j=0}^nG_j=Z_n$. Hence $Y_n'=X_n-Z_n'=Y_n$. Thus **the normalized predictable decomposition is unique**, with a common probability-one event available for all integer times by countability.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
