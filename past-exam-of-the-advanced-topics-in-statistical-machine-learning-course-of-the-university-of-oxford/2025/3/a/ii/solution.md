<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [recurrent neural network](../../../../../recurrent-neural-network.md) processes positions through a recurrence such as $h_t=F(h_{t-1},x_t)$. Computing $h_t$ requires $h_{t-1}$, so the standard computation is sequential across sequence positions, although different examples in a batch can be processed in parallel. Information from position $s$ to $t$ must pass through $t-s$ recurrent steps, and backpropagated [gradients](../../../../../gradient.md) involve products of that many step [Jacobian matrices](../../../../../jacobian-matrix.md). This creates [vanishing gradients](../../../../../vanishing-gradient-problem.md) or [exploding gradients](../../../../../exploding-gradient-problem.md) and can make long-range dependencies difficult to learn. Gating can mitigate these difficulties while retaining the recurrent dependence.

In a [transformer block](../../../../../transformer-block.md), all queries, keys, and values for an available input sequence can be formed in parallel. The [self-attention](../../../../../self-attention.md) weights are computed by [matrix multiplication](../../../../../matrix-multiplication.md), so positions within one layer can be processed together; layers themselves remain sequential. With unrestricted [self-attention](../../../../../self-attention.md), one position can directly receive information from any other position in one layer, giving a constant-length route across distant positions rather than one proportional to their separation. With [causal self-attention](../../../../../causal-self-attention.md), there is the same direct route to any permitted earlier position.

**A [transformer model](../../../../../transformer-model.md) supports parallel training across known sequence positions and short routes for long-range dependencies.** Even a causal model can compute all training positions together when the entire training sequence is supplied and the attention mask excludes future positions. However, ordinary autoregressive generation still generates one new token at a time. Full [self-attention](../../../../../self-attention.md) also constructs $L^2$ pairwise scores, with quadratic time and storage in sequence length for the direct implementation; a standard [recurrent neural network](../../../../../recurrent-neural-network.md) has linear sequential work in sequence length at fixed hidden width. Neither architecture guarantees that a useful long-range dependency will actually be learned.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
