<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The subspace spanned by $e_4,e_5,e_6$ is the [center of a Lie algebra](../../../../../center-of-a-lie-algebra.md). Each of their tensor squares is therefore invariant. On tensor products the infinitesimal [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md) acts by a derivation, $D_x(u\otimes v)=[x,u]\otimes v+u\otimes[x,v]$. Write $u\odot v=u\otimes v+v\otimes u$ and let $S=e_1\odot e_5+e_3\odot e_6-e_2\odot e_4$. The only potentially nonzero checks are

$$
D_{e_1}S=e_4\odot e_6-e_6\odot e_4=0,\quad
D_{e_2}S=-e_6\odot e_5+e_5\odot e_6=0,\quad
D_{e_3}S=-e_4\odot e_5+e_5\odot e_4=0.
$$

The remaining generators are central, so they act trivially. This proves every claimed tensor invariant.

These tensors are contravariant. To obtain an ordinary [metric tensor](../../../../../metric-tensor.md), take an invertible linear combination and invert it. For arbitrary real $a_4,a_5,a_6$ and $t\ne0$, set

$$
Q=tS+a_4e_4\otimes e_4+a_5e_5\otimes e_5+a_6e_6\otimes e_6.
$$

In the ordered basis $(e_1,e_2,e_3;e_4,e_5,e_6)$ its matrix is

$$
Q=\begin{pmatrix}0&tK\\tK^T&A\end{pmatrix},\qquad
K=\begin{pmatrix}0&1&0\\-1&0&0\\0&0&1\end{pmatrix},\qquad A=\operatorname{diag}(a_4,a_5,a_6).
$$

Since $K^TK=I$, $\det Q=-t^6\ne0$, and

$$
Q^{-1}=\begin{pmatrix}-t^{-2}KAK^T&t^{-1}K\\t^{-1}K^T&0\end{pmatrix}.
$$

Let $\lambda^a$ be the dual left-invariant coframe. The resulting [neutral invariant metrics on the free two-step Lie algebra on three generators](../../../../../neutral-invariant-metrics-on-the-free-two-step-lie-algebra-on-three-generators.md) are

$$
\boxed{g=t^{-1}(\lambda^1\odot\lambda^5+\lambda^3\odot\lambda^6-\lambda^2\odot\lambda^4)
-t^{-2}\bigl[a_5(\lambda^1)^2+a_4(\lambda^2)^2+a_6(\lambda^3)^2\bigr].}
$$

Here $(\lambda^a)^2=\lambda^a\otimes\lambda^a$. Infinitesimal invariance of $Q$ implies that its inverse is an adjoint-invariant [bilinear form](../../../../../bilinear-form.md). Its left-translated metric is right-invariant on a connected $G$, giving the desired **four-parameter family of bi-invariant metrics**. A change of variables removes the central $A$ block from the quadratic form, leaving three off-diagonal two-dimensional blocks. Each has one positive and one negative eigenvalue. Thus the [metric signature](../../../../../metric-signature.md) is $(3,3)$; these are [bi-invariant pseudo-Riemannian metrics](../../../../../bi-invariant-pseudo-riemannian-metric.md), not positive-definite ones.

Connectedness, conventionally understood here, matters for the passage from infinitesimal to full group invariance. If $G$ is disconnected, its other components must preserve $Q$ separately. For example the [Lie algebra automorphism](../../../../../automorphism-of-a-lie-algebra.md) reversing $e_1,e_4,e_6$ and fixing $e_2,e_3,e_5$ preserves all brackets but sends $S$ to $-S$. In the semidirect product of the simply connected group with this order-two automorphism, none of these nondegenerate $t\ne0$ tensors is invariant under that component. Thus the Lie-algebra data alone give the stated family on the identity component, rather than an unconditional extension to every disconnected realization.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
