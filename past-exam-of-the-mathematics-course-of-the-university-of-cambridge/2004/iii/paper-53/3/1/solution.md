<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $c=\langle R_0|R_1\rangle$. The joint state after the environment interaction is $\alpha|0\rangle|R_0\rangle+\beta|1\rangle|R_1\rangle$. Taking its [partial trace](../../../../../../partial-trace.md) over the environment gives the exact reduced [density operator](../../../../../../density-matrix.md)

$$
\rho'=\begin{pmatrix}|\alpha|^2&\alpha\overline\beta\,\overline c\\\overline\alpha\beta\,c&|\beta|^2\end{pmatrix}.
$$

The conjugate in the upper off-diagonal entry follows from tracing $|R_0\rangle\langle R_1|$. Normalization of the environment states and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) imply $|c|\leq1$.

For comparison, a [phase-flip channel](../../../../../../phase-flip-channel.md) sends $\rho$ to $(1-p)\rho+pZ\rho Z$, multiplying its off-diagonal entries by the real number $1-2p$. Consequently the claimed representation is valid, for a general input, **provided the environment overlap is real**, with

$$
\boxed{p=\frac{1-c}{2},\qquad c\in[-1,1].}
$$

This is a genuine probability between zero and one. The environment maps printed in the question do not themselves imply that $c$ is real. For example, choose $|R_1\rangle=i|R_0\rangle$, so $c=i$, and take $\alpha=\beta=1/\sqrt2$. The qubit becomes $(|0\rangle+i|1\rangle)/\sqrt2$, whose imaginary off-diagonal entries cannot come from any probabilistic mixture of $\rho$ and $Z\rho Z$. These environment maps are a valid isometry and can be extended to a unitary interaction, so this is an actual counterexample to the unrestricted premise.

The general [complex environment overlap in qubit dephasing](../../../../../../complex-environment-overlap-in-qubit-dephasing.md) has an exact corrected description. Write $c=re^{i\varphi}$, $0\leq r\leq1$, and let $D_\varphi=\operatorname{diag}(1,e^{i\varphi})$. Then

$$
\boxed{\rho'=D_\varphi\bigl[(1-q)\rho+qZ\rho Z\bigr]D_\varphi^\dagger,\qquad q=\frac{1-r}{2}.}
$$

At $r=0$, choose any phase. The [dephasing channel](../../../../../../dephasing-channel.md) includes both random phase errors and, when the overlap is complex, a coherent diagonal rotation. The subsequent probability formulas use the intended real-overlap phase-flip model.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
