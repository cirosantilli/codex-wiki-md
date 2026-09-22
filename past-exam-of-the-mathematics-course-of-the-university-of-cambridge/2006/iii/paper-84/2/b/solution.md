<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Nonlinear [hidden units](../../../../../../hidden-unit.md) create useful intermediate features, allowing the output to combine features rather than classify the original inputs directly. For example, two [binary threshold units](../../../../../../binary-threshold-unit.md) can compute OR and AND of two binary inputs; thresholding OR minus twice AND at $1/2$ gives XOR. A single monotone threshold of an affine function of the original two inputs cannot implement XOR: the two positive examples lie opposite each other and cannot be separated from the two negative examples by one line. Hidden features can also detect edges or other local patterns before a subsequent layer combines them into object-level features.

If hidden [activation functions](../../../../../../activation-function.md) are identities, substitute $z_j=x_j=\sum_iw_{ij}z_i$ into the output input to obtain

$$
x_k=\sum_i\left(\sum_jw_{jk}w_{ij}\right)z_i.
$$

With biases included this is still one affine map. **Linear hidden layers collapse into a single effective layer and add no nonlinear feature-building ability.** The output may remain nonlinear, but its preactivation is just an affine function of the inputs. With standard monotone output activations this still cannot solve XOR or parity by one output unit. An artificially chosen nonmonotone output function could itself encode a complicated scalar decision rule, but that would not be a benefit of the linear hidden layer.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
