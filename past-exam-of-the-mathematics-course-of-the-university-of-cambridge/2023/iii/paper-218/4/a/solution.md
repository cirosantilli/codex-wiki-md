<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With $f=\mathbf1_{\{\mathrm{font}=\mathrm{serif}\}}$ and $d=\mathbf1_{\{\mathrm{display}=\mathrm{popup}\}}$, the model-matrix input is

$$
x=(f,d,fd)^T\in\mathbb R^3.
$$

The [feedforward neural network](../../../../../../feedforward-neural-network.md) has three inputs, a fully connected layer of two [ReLU](../../../../../../rectified-linear-unit.md) units, and a fully connected two-class [softmax](../../../../../../softmax-function.md) output. Algebraically,

$$
h=\operatorname{ReLU}(Wx+b),
\qquad
z=Vh+c,
\qquad
p_k=\frac{e^{z_k}}{e^{z_0}+e^{z_1}},
$$

where $W\in\mathbb R^{2\times3}$, $b\in\mathbb R^2$, $V\in\mathbb R^{2\times2}$, and $c\in\mathbb R^2$. The coding is $0$ for no click and $1$ for a click. There are

$$
2(3)+2+2(2)+2=14
$$

parameters.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
