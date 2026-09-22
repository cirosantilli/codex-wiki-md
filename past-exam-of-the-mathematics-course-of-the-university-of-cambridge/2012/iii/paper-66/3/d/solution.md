<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

This is the [dephased Bell-state mixture](../../../../../../dephased-bell-state-mixture.md) with coherence parameter $2x$. The [Pauli correlation tensor](../../../../../../pauli-correlation-tensor.md) is

$$
T_{ij}=\operatorname{Tr}[\rho(x)\,\sigma_i\otimes\sigma_j],
\qquad T=\operatorname{diag}(2x,-2x,1),
$$

so spin measurements along unit vectors have $E(\mathbf a,\mathbf b)=\mathbf a^TT\mathbf b$. Choose

$$
\mathbf a=\mathbf e_z,\qquad \mathbf a'=\mathbf e_x,\qquad
\mathbf b=\frac{\mathbf e_z+2x\mathbf e_x}{\sqrt{1+4x^2}},\qquad
\mathbf b'=\frac{-\mathbf e_z+2x\mathbf e_x}{\sqrt{1+4x^2}}.
$$

Then $E(a,b)-E(a,b')=2/\sqrt{1+4x^2}$ and $E(a',b)+E(a',b')=8x^2/\sqrt{1+4x^2}$. The [CHSH inequality](../../../../../../chsh-inequality.md) expression is therefore

$$
\boxed{S(x)=2\sqrt{1+4x^2}>2\quad\text{for every }0<x\leq\tfrac12.}
$$

These axes also attain the [CHSH optimum from the correlation tensor](../../../../../../chsh-optimum-from-the-correlation-tensor.md), since the two largest [eigenvalues](../../../../../../eigenvalue.md) of $T^TT$ are $1$ and $4x^2$. At $x=1/2$ the value is $2\sqrt2$; at $x=0$ the explicit [LHV model](../../../../../../local-hidden-variable-theory.md) in part (c) applies. Thus **exactly $0<x\leq1/2$ has correlations incompatible with a local hidden-variable description**.

Arbitrarily small positive coherence suffices in this particular one-parameter family, with optimally chosen axes; the violation above two tends to zero quadratically as $x\to0$. This does not imply that every entangled mixed state violates a [CHSH inequality](../../../../../../chsh-inequality.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
