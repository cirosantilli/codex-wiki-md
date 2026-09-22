<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For hidden layers $h^{(r)}=\phi_r(W_rh^{(r-1)}+b_r)$ with $h^{(0)}=x$, the output logits are $z=W_{R+1}h^{(R)}+b_{R+1}$ and the [softmax function](../../../../../../softmax-function.md) gives

$$
\boxed{p_\ell(x)=\frac{e^{z_\ell}}{\sum_{j=1}^Le^{z_j}}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
