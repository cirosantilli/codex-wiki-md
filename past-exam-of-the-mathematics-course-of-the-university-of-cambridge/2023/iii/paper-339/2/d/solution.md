<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The assertion uses the positive parameters required for $M$ to be a preconditioner: assume $\alpha>0$ and $\beta>0$. For $x\in\mathbb R^n$ and $z\in\mathbb R^m$, complete the square:

$$
\begin{aligned}
\binom{x}{z}^{\!T}
M\binom{x}{z}
&=\alpha\|x\|_2^2+2\langle Ax,z\rangle+\beta\|z\|_2^2\\
&=\beta\left\|z+\frac{Ax}{\beta}\right\|_2^2
+x^T\left(\alpha I-\frac{A^TA}{\beta}\right)x.
\end{aligned}
$$

The [matrix 2-norm](../../../../../../matrix-2-norm.md) bound $\|Ax\|_2\leq\|A\|_2\|x\|_2$ shows that

$$
x^T\left(\alpha I-\frac{A^TA}{\beta}\right)x
\geq\left(\alpha-\frac{\|A\|_2^2}{\beta}\right)\|x\|_2^2>0
$$

for $x\ne0$ when $\alpha\beta>\|A\|_2^2$. If $x=0$ and $z\ne0$, the square contributes $\beta\|z\|_2^2>0$. Thus $\boxed{M\text{ is positive definite}}$. Equivalently, the [Schur complement](../../../../../../schur-complement.md) of the lower-right block is $\alpha I-A^TA/\beta\succ0$.

Taken literally without the positivity inherited from part b, the product condition alone is insufficient: $A=0$ and $\alpha=\beta=-1$ is a counterexample. Thus $\alpha,\beta>0$ is a necessary implicit hypothesis.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
