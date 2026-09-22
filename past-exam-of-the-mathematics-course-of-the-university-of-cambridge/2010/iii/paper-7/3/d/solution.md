<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The positive sign printed in the exponential uses the [skew-adjoint](../../../../../../skew-adjoint-generator.md) convention for the [Dirac operator](../../../../../../dirac-operator.md): $D^*=-D$, so $D_-=-D_+^*$. Put $A=D_+$ and define the nonnegative [self-adjoint operators](../../../../../../self-adjoint-operator.md)

$$
P=A^*A=-D_-D_+,\qquad Q=AA^*=-D_+D_-.
$$

For $t>0$, the assumed [compact elliptic spectral theorem](../../../../../../compact-elliptic-spectral-theorem.md) for these [elliptic differential operators](../../../../../../elliptic-differential-operator.md) gives discrete [eigenvalues](../../../../../../eigenvalue.md), finite multiplicities and [trace-class operators](../../../../../../trace-class-operator.md) $e^{-tP}$, $e^{-tQ}$.

If $Pu=\lambda u$ with $\lambda>0$, then $Q(Au)=A(Pu)=\lambda Au$ and $Au\ne0$. Conversely $A^*$ sends the $\lambda$ [eigenspace](../../../../../../eigenspace.md) of $Q$ to that of $P$. On these [eigenspaces](../../../../../../eigenspace.md) the inverse of $A$ is $\lambda^{-1}A^*$. Thus the positive spectra agree with multiplicity, and absolute convergence of the [operator traces](../../../../../../operator-trace.md) permits cancellation term by term:

$$
\operatorname{Tr}e^{-tP}-\operatorname{Tr}e^{-tQ}
=\dim\ker P-\dim\ker Q
=\dim\ker A-\dim\ker A^*.
$$

The last expression is the [Fredholm index](../../../../../../fredholm-index.md) of $A$, since its closed range has [orthogonal complement](../../../../../../orthogonal-complement.md) $\ker A^*$. Consequently

$$
\boxed{\operatorname{ind}D_+=\operatorname{Tr}(e^{tD_-D_+})-\operatorname{Tr}(e^{tD_+D_-}),\qquad t>0.}
$$

This is the [supertrace](../../../../../../supertrace.md) cancellation used in Question 1. If the [Dirac operator](../../../../../../dirac-operator.md) is instead defined to be [self-adjoint](../../../../../../self-adjoint-operator.md), $D_-=(D_+)^*$ and the heat exponentials must have a minus sign. With that convention the positive exponentials in the printed formula are generally unbounded and have no finite [operator trace](../../../../../../operator-trace.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
