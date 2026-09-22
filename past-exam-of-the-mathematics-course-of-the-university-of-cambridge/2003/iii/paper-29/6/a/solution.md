<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret the comparison at $N$ on $\{N<\infty\}$; values at an infinite [stopping time](../../../../../../stopping-time.md) are not required. The [stopping time](../../../../../../stopping-time.md) events make $Y_n$ adapted, and $|Y_n|\leq|X_n^1|+|X_n^2|$ gives [integrability](../../../../../../integrability.md). On $\{N\leq n\}$ the next value is $X_{n+1}^2$. On $\{N>n\}$ it is $X_{n+1}^1$ unless $N=n+1$, and on that latter event switching only decreases the value. Consequently the pointwise inequality

$$
Y_{n+1}\leq\mathbf1_{\{N>n\}}X_{n+1}^1+\mathbf1_{\{N\leq n\}}X_{n+1}^2
$$

holds even though $\{N=n+1\}$ need not be known at time $n$. Both indicators displayed here are $\mathcal F_n$-[measurable](../../../../../../measurability.md). Taking [conditional expectations](../../../../../../conditional-expectation.md) and using the two [supermartingale](../../../../../../supermartingale.md) inequalities therefore gives

$$
\mathbb E[Y_{n+1}\mid\mathcal F_n]\leq\mathbf1_{\{N>n\}}X_n^1+\mathbf1_{\{N\leq n\}}X_n^2=Y_n.
$$

Thus $\boxed{Y\text{ is a supermartingale}.}$ This proves [pasting supermartingales with downward jumps](../../../../../../pasting-supermartingales-with-downward-jumps.md) without incorrectly treating the future switching event as predictable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
