<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

For a [binary symmetric channel](../../../../../binary-symmetric-channel.md) with crossover [probability](../../../../../probability.md) $p$, Shannon's noisy coding theorem gives capacity $C=1-h_2(p)$ bits per use, where $h_2(p)=-p\log_2p-(1-p)\log_2(1-p)$. For any rate below capacity there are block codes with block length tending to infinity and decoding error tending to zero. Conversely, vanishing-error transmission cannot have asymptotic rate above capacity. At $p=1/2$ the capacity is zero; the formula also covers $p>1/2$ by complementing the output.

For discrete [random variables](../../../../../random-variable-split.md), [mutual information](../../../../../mutual-information.md) is

$$
I(X;Y)=\sum_{x,y}p_{xy}\log_2\frac{p_{xy}}{p_xp_y}
=H(X)+H(Y)-H(X,Y).
$$

The formula is symmetric. To prove nonnegativity, apply $\log t\leq t-1$ to $t=p_xp_y/p_{xy}$ for positive joint masses. Multiplication by $p_{xy}$ and summation gives $-I\log2\leq\sum_{p_{xy}>0}p_xp_y-1\leq0$. Hence $I\geq0$, with equality precisely for [independence](../../../../../independent-random-variables.md). The channel information capacity is $\sup_{p_X}I(X;Y)$, over input distributions.

For the ternary channel every conditional output row has entropy $h_{\rm row}=-(1-2\beta)\log_2(1-2\beta)-2\beta\log_2\beta$, independent of the input. Therefore $I=H(Y)-h_{\rm row}\leq\log_23-h_{\rm row}$. Uniform input produces uniform output, since the matrix is doubly stochastic, and attains the bound. Thus

$$
\boxed{C=\log_23+(1-2\beta)\log_2(1-2\beta)+2\beta\log_2\beta.}
$$

Use $0\log0=0$ at the endpoints. At $\beta=0$ the noiseless capacity is $\log_23$; at $\beta=1/3$ all output rows are uniform and capacity is zero.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
