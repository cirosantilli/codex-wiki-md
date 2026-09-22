<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Assume the [self-adjoint](../../../../../../self-adjoint-operator.md) interpretation of [positive-definite operator](../../../../../../positive-definite-operator.md) from the preceding part. For $v,w\in H$ and real $\varepsilon$, expand the [quadratic functional](../../../../../../quadratic-functional.md):

$$
I(v+\varepsilon w)=I(v)+2\varepsilon\langle Lv-f,w\rangle
+\varepsilon^2\langle Lw,w\rangle.
$$

The [first variation](../../../../../../first-variation.md) therefore vanishes in every direction precisely when $\langle Lv-f,w\rangle=0$ for every $w$, or **$Lv=f$**. This is its [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) and its [weak formulation](../../../../../../weak-formulation.md). For any weak solution $u$, write $v=u+w$. Self-adjointness and $Lu=f$ cancel the cross terms and give the exact identity

$$
\boxed{I(v)-I(u)=\langle L(v-u),v-u\rangle.}
$$

Strict positivity makes this difference positive unless $v=u$, so **every weak solution is the unique global minimizer**, and conversely every minimizer is a weak solution. If $L$ is uniformly positive, the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) additionally gives existence for every $f\in H$ and $\|u\|\leq\|f\|/\gamma$. The identity above then gives the quantitative gap $I(v)-I(u)\geq\gamma\|v-u\|^2$.

The hypotheses matter. On $\mathbb R^2$, let

$$
L=\begin{pmatrix}1&-1\\1&1\end{pmatrix},\qquad f=\begin{pmatrix}1\\0\end{pmatrix}.
$$

Then $\langle Lv,v\rangle=\|v\|^2>0$ for nonzero $v$, but $I$ is minimized at $v=f$, whereas $L^{-1}f=(1/2,-1/2)^T$. Thus real quadratic positivity without symmetry does not imply the requested variational assertion: the [symmetric part determines a real quadratic functional](../../../../../../symmetric-part-determines-a-real-quadratic-functional.md).

Also, strict [self-adjoint](../../../../../../self-adjoint-operator.md) positivity does not imply existence for arbitrary $f$. On $H=\ell^2$, take $(Lv)_j=v_j/j$ and $f_j=1/j$. The operator is bounded, [self-adjoint](../../../../../../self-adjoint-operator.md) and strictly positive, and $f\in\ell^2$; a solution would have $u_j=1$, which is not in $\ell^2$. In fact the trial vectors with their first $N$ coordinates equal to one give $I(v)=-\sum_{j=1}^N1/j\to-\infty$. The printed conclusion about a weak solution is valid whenever that solution exists; an unconditional existence assertion needs uniform positivity.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
