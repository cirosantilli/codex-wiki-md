<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With the [determinant-normalized slash operator](../../../../../../determinant-normalized-slash-operator.md), let $W_N=\begin{pmatrix}0&-1\\N&0\end{pmatrix}$ and $Jf=i^k(f|_kW_N)=g$. Conjugation by $W_N$ preserves $\Gamma_1(N)$, and rational slash operators preserve [modular cusp](../../../../../../cusp-of-a-modular-group.md) holomorphy and vanishing. Hence $g$ is also a [cusp form](../../../../../../cusp-form.md) at that level. Direct substitution gives $J^2f=f$; the factor $i^k$ cancels the central weight sign.

Put $F(y)=f(iy/\sqrt N)$ and $G(y)=g(iy/\sqrt N)$. The defining formula gives the exact relations

$$
\boxed{G(y)=y^{-k}F(1/y),\qquad F(y)=y^{-k}G(1/y).}
$$

In the initial half-plane of absolute convergence, termwise integration of the Fourier series and the [gamma function](../../../../../../gamma-function.md) yield the [Mellin transform of a cusp-form L-function](../../../../../../mellin-transform-of-a-cusp-form-l-function.md)

$$
\Lambda(f,s)=\int_0^\infty F(y)y^{s-1}\,dy.
$$

The scaling of $y$ accounts for $N^{s/2}$ in the completion. At infinity $F$ and $G$ decay exponentially. At zero the boxed relation expresses $F$ as a power times an exponentially decaying function of $1/y$. Thus this integral converges locally uniformly for every complex $s$, including after differentiation in $s$, and defines an entire function.

Splitting at one and changing $y$ to $1/y$ in the lower integral gives

$$
\boxed{\Lambda(f,s)=\int_1^\infty\bigl(F(y)y^{s-1}+G(y)y^{k-s-1}\bigr)\,dy.}
$$

Applying the same formula to $g$ interchanges $F,G$, because $J^2=1$. It proves the [phase-normalized Fricke functional equation](../../../../../../phase-normalized-fricke-functional-equation.md)

$$
\boxed{\Lambda(f,s)=\Lambda(g,k-s)\quad\text{for every }s\in\mathbb C.}
$$

The entire function here is the completion, despite the apparent [poles](../../../../../../pole.md) of the gamma factor in its initial product formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
