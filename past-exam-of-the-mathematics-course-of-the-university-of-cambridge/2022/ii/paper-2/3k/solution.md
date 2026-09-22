<h1 id="3k/solution">Solution</h1>

↑ **Parent:** [3K](../3k.md)

A [discrete memoryless channel](../../../../../discrete-memoryless-channel.md) has finite input alphabet $\mathcal A$, finite output alphabet $\mathcal B$, and transition probabilities $P(y\mid x)$; successive outputs are conditionally independent given the corresponding inputs. The [Shannon second coding theorem](../../../../../noisy-channel-coding-theorem.md) states that rates below

$$
C=\max_{P_X}I(X;Y)
$$

admit block codes with error probability tending to zero, whereas rates above $C$ cannot have vanishing error.

For any joint input law of $(X_1,X_2)$, conditional independence of the product channel gives

$$
\begin{aligned}
I(X_1,X_2;Y_1,Y_2)
&=H(Y_1,Y_2)-H(Y_1,Y_2\mid X_1,X_2)\\
&\leq H(Y_1)+H(Y_2)-H(Y_1\mid X_1)-H(Y_2\mid X_2)\\
&=I(X_1;Y_1)+I(X_2;Y_2)
\leq C_1+C_2.
\end{aligned}
$$

Choose $X_1$ and $X_2$ independently with capacity-achieving input laws for their respective channels. Then the inequality becomes equality, so the product-channel capacity is

$$
\boxed{C_1+C_2}.
$$

## ↑ Ancestors (10)

1. [3K](../3k.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
