<h1 id="3/iii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The first component obeys $\dot x_1=\lambda_1x_1$, so $x_1(t)=e^{\lambda_1t}x_1(0)$. Variation of constants in

$$
\dot x_2=x_1+\lambda_2x_2
$$

then gives

$$
x_2(t)=e^{\lambda_2t}x_2(0)
+\frac{e^{\lambda_1t}-e^{\lambda_2t}}
{\lambda_1-\lambda_2}x_1(0).
$$

Hence the [matrix exponential](../../../../../../../matrix-exponential.md) is

$$
\boxed{
A=e^{tL}
=\begin{pmatrix}
e^{\lambda_1t}&0\\
\dfrac{e^{\lambda_1t}-e^{\lambda_2t}}
{\lambda_1-\lambda_2}&e^{\lambda_2t}
\end{pmatrix}}.
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Iii](../../iii.md)
3. [3](../../../3.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
