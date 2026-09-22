<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each continuous $f_\alpha$ of polynomial growth defines a regular [tempered distribution](../../../../../../tempered-distribution.md) by

$$
\langle f_\alpha,\varphi\rangle=\int_{\mathbb R^n}f_\alpha(x)\varphi(x)\,dx.
$$

Choosing an integer $L>M_\alpha+n$ gives

$$
|\langle f_\alpha,\varphi\rangle|\leq C_\alpha\int(1+|x|)^{M_\alpha-L}\,dx\ \sup_x(1+|x|)^L|\varphi(x)|,
$$

which is bounded by finitely many [Schwartz space](../../../../../../schwartz-space.md) seminorms. Its [distributional derivative](../../../../../../distributional-derivative.md) satisfies

$$
\langle D^\alpha f_\alpha,\varphi\rangle=(-1)^{|\alpha|}\langle f_\alpha,D^\alpha\varphi\rangle
$$

and is therefore tempered. A finite sum of continuous linear forms is continuous, so

$$
\boxed{\sum_{|\alpha|\leq N}D^\alpha f_\alpha\in\mathcal S'(\mathbb R^n)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
