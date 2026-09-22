<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With column vectors and learned biases,

$$
h_1=\operatorname{ReLU}(W_1x+b_1),\quad
h_2=\operatorname{ReLU}(W_2h_1+b_2),\quad
h_3=\operatorname{ReLU}(W_3h_2+b_3),
$$



$$
z=W_4h_3+b_4,
\qquad \widehat p_l=\frac{e^{z_l}}{\sum_{r=1}^{26}e^{z_r}}.
$$

The dimensions are $16\to100\to75\to50\to26$. The number of parameters is

$$
\boxed{16\cdot100+100+100\cdot75+75+75\cdot50+50+50\cdot26+26.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
