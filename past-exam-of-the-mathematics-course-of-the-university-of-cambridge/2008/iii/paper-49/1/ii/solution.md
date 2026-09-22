<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $v=(x,y)^T$ and $B(\rho)=\left(\begin{smallmatrix}\cosh\rho&\sinh\rho\\\sinh\rho&\cosh\rho\end{smallmatrix}\right)$. Matrix multiplication gives

$$
(\rho,v)(\rho',v')=(\rho+\rho',v+B(\rho)v').
$$

Thus $G$ is a [semidirect product](../../../../../../semidirect-product.md) of the translation plane by the one-parameter [Lorentz boost](../../../../../../lorentz-boost.md) group. Differentiating left multiplication at the identity gives the [left-invariant vector fields](../../../../../../left-invariant-vector-field.md)

$$
\boxed{X_0=\partial_\rho,\qquad
X_1=\cosh\rho\,\partial_x+\sinh\rho\,\partial_y,\qquad
X_2=\sinh\rho\,\partial_x+\cosh\rho\,\partial_y.}
$$

They obey $[X_0,X_1]=X_2$, $[X_0,X_2]=X_1$ and $[X_1,X_2]=0$.

Their dual [coframe](../../../../../../coframe.md) is $d\rho$, $\cosh\rho\,dx-\sinh\rho\,dy$, and $-\sinh\rho\,dx+\cosh\rho\,dy$. The [Haar measure from a left-invariant coframe](../../../../../../haar-measure-from-a-left-invariant-coframe.md) is their absolute wedge product. Since $\det B(\rho)=1$,

$$
\boxed{d\mu=C\,d\rho\,dx\,dy,\qquad C>0.}
$$

One can also check this directly: left multiplication has Jacobian determinant one. Right multiplication has a block triangular Jacobian with determinant one too, so the same measure is both left and right [Haar measure](../../../../../../haar-measure.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
