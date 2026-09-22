<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [feedforward neural network](../../../../../../feedforward-neural-network.md) has three input coordinates, two hidden [sigmoid function](../../../../../../sigmoid-function.md) units and two output [softmax function](../../../../../../softmax-function.md) units. Every input is connected to each hidden unit, and each hidden unit to each output unit; each hidden and output unit also has a bias. A layer diagram is

$$
\underbrace{\begin{pmatrix}\mathrm{income}\\\mathrm{age}\\\mathrm{amount}\end{pmatrix}}_{\text{3 inputs}}
\xrightarrow{\ W\in\mathbb R^{2\times3},\ b\in\mathbb R^2\ }
\underbrace{\begin{pmatrix}h_1\\h_2\end{pmatrix}}_{\text{2 sigmoid units}}
\xrightarrow{\ V\in\mathbb R^{2\times2},\ a\in\mathbb R^2\ }
\underbrace{\begin{pmatrix}p_0\\p_1\end{pmatrix}}_{\text{2 softmax outputs}}.
$$

Algebraically, with $x_i=(\mathrm{income}_i,\mathrm{age}_i,\mathrm{amount}_i)^T$,

$$
h_{ij}=\frac1{1+\exp[-b_j-\sum_{r=1}^3W_{jr}x_{ir}]},\quad j=1,2,\qquad o_{ic}=a_c+\sum_{j=1}^2V_{cj}h_{ij},\quad c=0,1,
$$



$$
\boxed{p_{ic}=\frac{e^{o_{ic}}}{e^{o_{i0}}+e^{o_{i1}}},\qquad Y_i\mid x_i\sim\operatorname{Bernoulli}(p_{i1}),\quad i=1,\ldots,3000,}
$$

with responses conditionally independent. The fourteen displayed weight and bias parameters comprise six input weights, two hidden biases, four output weights and two output biases. The one-hot encoding supplies targets $t_{i0}=1-Y_i$, $t_{i1}=Y_i$, and the [categorical cross-entropy loss](../../../../../../categorical-cross-entropy-loss.md) is the negative of $\ell=\sum_i\sum_ct_{ic}\log p_{ic}$. There is [softmax non-identifiability](../../../../../../softmax-non-identifiability.md) under a common shift of both output logits, but the predicted probabilities are well defined.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
