<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Again put $a=(1+\lambda)/2$, $b=(1-\lambda)/2$. If computational strings $z,y$ differ in $h$ places, the matrix element of $U_\phi^{\otimes n}$ between them is $a^{n-h}b^h$: an unchanged bit contributes $a$, and a flipped bit contributes $b$. Hence the given operator is

$$
\boxed{U_\phi^{(n)}=U_\phi^{\otimes n}.}
$$

The printed factored expression $a^n(b/a)^h$ is undefined at $a=0$, namely $\phi=1/2$. Its polynomial form $a^{n-h}b^h$ gives the natural continuous extension there, $U_{1/2}^{(n)}=X^{\otimes n}$. For $n\ge2$ the strict promise $\phi<1/n$ avoids that singular value; for $n=1$ the extension is needed to include the allowed phase $1/2$. This is a removable defect of the formula, not a failure of unitarity of the tensor-product operator.

Prepare $|-\rangle^{\otimes n}$. Its [eigenvalue](../../../../../../eigenvalue.md) is $\lambda^n=e^{2\pi in\phi}$, giving [tensor-product eigenphase amplification](../../../../../../tensor-product-eigenphase-amplification.md). Write $n=2^s$. If $s<m$, then

$$
n\phi=\frac{x}{2^{m-s}},\qquad 0\le x<2^{m-s},
$$

where the upper bound is exactly the promise $\phi<1/n$. Thus the amplified phase has only $m-s$ unknown binary digits and no modulo-one aliasing. Run [exact quantum phase estimation](../../../../../../exact-quantum-phase-estimation.md) with $m-s$ controls on the controlled-$U_\phi^{(n)}$ black box. It returns $x$ exactly, after which division by the original $2^m$ recovers $\phi$.

The number of joint black-box uses is

$$
\boxed{2^{m-s}-1=\frac{2^m}{n}-1=O(2^m/n).}
$$

If $s\ge m$, the dyadic promise and $\phi<1/n$ force $x=0$, so output $\phi=0$ without querying the oracle. This covers the zero-control edge case without an invalid negative number of phase bits. The improvement counts one supplied controlled-$U_\phi^{(n)}$ call as one query. Implementing such a joint call from $n$ individual controlled-$U_\phi$ calls would remove the claimed factor-$n$ primitive-query saving, and preparing the $n$ target [qubits](../../../../../../qubit.md) is a separate gate cost.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
