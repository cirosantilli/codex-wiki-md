<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Stone theorem for the circle group](../../../../../../stone-theorem-for-the-circle-group.md) says that a strongly continuous [unitary representation](../../../../../../unitary-representation.md) $U$ of $\mathbb T=\{z:|z|=1\}$ has an orthogonal decomposition

$$
\boxed{H=\bigoplus_{n\in\mathbb Z}H_n,\qquad U_z|_{H_n}=z^nI.}
$$

Equivalently, $U_z=\sum_nz^nP_n$ strongly, with mutually [orthogonal projections](../../../../../../orthogonal-projection.md) $P_n$ summing strongly to the identity. Define these [projections](../../../../../../projection-linear-algebra.md) using normalized [Haar measure](../../../../../../haar-measure.md):

$$
P_n\xi=\int_{\mathbb T}z^{-n}U_z\xi\,dz.
$$

Haar invariance gives $U_wP_n=w^nP_n$. Changing $z$ to $z^{-1}$ in the adjoint integral proves $P_n^*=P_n$. Applying the defining integral to $P_m\xi$ gives $P_nP_m=\delta_{nm}P_m$ by [orthogonality](../../../../../../orthogonal-vectors.md) of the characters $z^k$. Thus $P_n$ are [orthogonal projections](../../../../../../orthogonal-projection.md), and their ranges are exactly the indicated character subspaces.

It remains to prove completeness of these subspaces. The [Fejér kernel](../../../../../../fejer-kernel.md) has the finite expansion

$$
K_N(e^{it})=\sum_{|n|<N}\left(1-\frac{|n|}{N}\right)e^{-int}
=\frac1N\left|\sum_{j=0}^{N-1}e^{ijt}\right|^2.
$$

It is nonnegative, has normalized integral one, and its integral outside any fixed neighborhood of the identity tends to zero, since the denominator in the usual geometric-sum formula is bounded away from zero there. Strong [continuity](../../../../../../continuous-function.md) therefore gives

$$
\int K_N(z)U_z\xi\,dz\longrightarrow\xi:
$$

split the integral into that neighborhood, where $\|U_z\xi-\xi\|$ is small, and its complement, where it is bounded by $2\|\xi\|$. The integral on the left is $\sum_{|n|<N}(1-|n|/N)P_n\xi$. Hence the closed span of all $H_n$ is $H$. [Orthogonality](../../../../../../orthogonal-vectors.md) then gives the unweighted strong sum and the stated representation formula.

Conversely, any orthogonal decomposition indexed by the integers gives this representation; [continuity](../../../../../../continuous-function.md) follows first on finite sums and then on all [vectors](../../../../../../vector.md) by the uniform unitary [norm](../../../../../../norm.md) bound. With $z=e^{it}$ its generator is

$$
A\xi=\sum_nnP_n\xi,\qquad
D(A)=\left\{\xi:\sum_nn^2\|P_n\xi\|^2<\infty\right\}.
$$

This diagonal operator is [self-adjoint](../../../../../../self-adjoint-operator.md) and $U_{e^{it}}=e^{itA}$. Thus the circle theorem is the integer-spectrum version of the one-parameter theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
