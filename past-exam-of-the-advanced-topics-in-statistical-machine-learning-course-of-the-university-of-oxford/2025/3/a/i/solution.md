<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [transformer block](../../../../../transformer-block.md) has two principal sublayers: [multi-head attention](../../../../../multi-head-attention.md) and a positionwise [feedforward neural network](../../../../../feedforward-neural-network.md). Each sublayer has a [residual connection](../../../../../residual-connection.md) and [layer normalization](../../../../../layer-normalization.md). To make the components explicit, let $X\in\mathbb R^{L\times d_{\rm model}}$ contain the representations of $L$ sequence positions. For head $h$, learned projections form

$$
Q_h=XW_h^Q,\qquad K_h=XW_h^K,\qquad V_h=XW_h^V.
$$

The [scaled dot-product attention](../../../../../scaled-dot-product-attention.md) output is

$$
A_h=\operatorname{softmax}\left(\frac{Q_hK_h^T}{\sqrt{d_k}}+B\right)V_h,
$$

where the [softmax function](../../../../../softmax-function.md) acts along each row and $B$ is an optional attention mask. For [causal self-attention](../../../../../causal-self-attention.md), disallowed future positions receive $-\infty$ before the [softmax function](../../../../../softmax-function.md), giving zero attention weights. In [self-attention](../../../../../self-attention.md), queries, keys, and values all come from the same input sequence. The [multi-head attention](../../../../../multi-head-attention.md) output concatenates the heads and projects them:

$$
\operatorname{MHA}(X)=\operatorname{Concat}(A_1,\ldots,A_H)W^O.
$$

A standard post-normalization [transformer block](../../../../../transformer-block.md) can then be written

$$
\boxed{U=\operatorname{LN}(X+\operatorname{MHA}(X)),\qquad Y=\operatorname{LN}(U+\operatorname{FFN}(U))}.
$$

Here [layer normalization](../../../../../layer-normalization.md) normalizes the feature coordinates of each position separately, within each example, and applies learned scales and shifts. The positionwise [feedforward neural network](../../../../../feedforward-neural-network.md) applies the same two affine maps and [activation function](../../../../../activation-function.md) at every position, for example

$$
\operatorname{FFN}(z)=\rho(zW_1+b_1)W_2+b_2.
$$

Thus **attention mixes information between positions, while the feedforward sublayer transforms each position's features**. The [residual connections](../../../../../residual-connection.md) support propagation through a deep stack, and [dropout](../../../../../dropout.md) is often used during training. Pre-normalization variants move [layer normalization](../../../../../layer-normalization.md) before the sublayer. A model's [positional encoding](../../../../../positional-encoding.md) supplies order information to the sequence representation or attention mechanism; a decoder in an encoder-decoder model also has a cross-attention sublayer between its [self-attention](../../../../../self-attention.md) and [feedforward neural network](../../../../../feedforward-neural-network.md) sublayers.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
