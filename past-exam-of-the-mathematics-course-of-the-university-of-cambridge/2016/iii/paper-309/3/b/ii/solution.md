<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On [smooth functions](../../../../../../../smooth-function.md), the [Lie derivative of a function](../../../../../../../lie-derivative-of-a-function.md) satisfies

$$
[\mathcal L_X,\mathcal L_Y]f=X(Y(f))-Y(X(f))=[X,Y](f)=\mathcal L_{[X,Y]}f.
$$

On an arbitrary [vector field](../../../../../../../vector-field.md) $W$, the [Lie derivative of a vector field](../../../../../../../lie-derivative-of-a-vector-field.md) gives

$$
[\mathcal L_X,\mathcal L_Y]W=[X,[Y,W]]-[Y,[X,W]]=[[X,Y],W]=\mathcal L_{[X,Y]}W.
$$

The middle equality follows from the [Jacobi identity](../../../../../../../jacobi-identity.md) for the [Lie bracket of vector fields](../../../../../../../lie-bracket-of-vector-fields.md). One can verify that identity without assuming the result being proved: view [vector fields](../../../../../../../vector-field.md) as derivations acting on [smooth functions](../../../../../../../smooth-function.md), expand their [commutators](../../../../../../../commutator.md), and cancel the six compositions. Equality as derivations implies equality as [vector fields](../../../../../../../vector-field.md).

For the second identity, let $A,B,C$ be any operators on either [smooth functions](../../../../../../../smooth-function.md) or [vector fields](../../../../../../../vector-field.md). Associativity of composition gives

$$
\begin{aligned}
[[A,B],C]&=ABC-BAC-CAB+CBA,\\
[[B,C],A]&=BCA-CBA-ABC+ACB,\\
[[C,A],B]&=CAB-ACB-BCA+BAC.
\end{aligned}
$$

Each term cancels in the sum. Applying this to $A=\mathcal L_X$, $B=\mathcal L_Y$, $C=\mathcal L_Z$ proves **both requested identities on both kinds of arguments**:

$$
\boxed{[\mathcal L_X,\mathcal L_Y]=\mathcal L_{[X,Y]},\qquad
[[\mathcal L_X,\mathcal L_Y],\mathcal L_Z]+[[\mathcal L_Y,\mathcal L_Z],\mathcal L_X]+[[\mathcal L_Z,\mathcal L_X],\mathcal L_Y]=0.}
$$

The [commutator identity for Lie derivatives](../../../../../../../commutator-identity-for-lie-derivatives.md) expresses that the [Lie derivative of a tensor field](../../../../../../../lie-derivative-of-a-tensor-field.md) represents the [Lie bracket of vector fields](../../../../../../../lie-bracket-of-vector-fields.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 309](../../../../paper-309-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
