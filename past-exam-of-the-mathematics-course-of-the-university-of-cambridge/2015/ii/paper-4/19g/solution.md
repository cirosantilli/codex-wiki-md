<h1 id="19g/solution">Solution</h1>

↑ **Parent:** [19G](../19g.md)

Use an [inner product](../../../../../inner-product.md) linear in the first variable. For each $y$, the bounded linear functional $x\mapsto\langle Tx,y\rangle$ is represented uniquely by a vector $T^*y$ under the [Riesz representation theorem](../../../../../riesz-representation-theorem.md), so $\langle Tx,y\rangle=\langle x,T^*y\rangle$. Uniqueness and the conjugate-linearity in the second argument imply $T^*(ay+bz)=aT^*y+bT^*z$. Furthermore

$$
\|T^*y\|=\sup_{\|x\|=1}|\langle Tx,y\rangle|\leq\|T\|\|y\|.
$$

Thus the [adjoint operator](../../../../../adjoint-operator.md) exists, is linear and bounded, and is unique because a vector orthogonal to every $x$ is zero.

A [normal operator](../../../../../normal-operator.md) satisfies $T^*T=TT^*$. The unilateral [unilateral shift operator](../../../../../unilateral-shift-operator.md) $S(x_1,x_2,\ldots)=(0,x_1,x_2,\ldots)$ on $\ell^2$ is bounded but not normal: $S^*S=I$, whereas $SS^*=I-P_{e_1}$. For general $T$,

$$
\|Tx\|^2-\|T^*x\|^2=\langle(T^*T-TT^*)x,x\rangle.
$$

Normality implies equality of norms. Conversely equality for every $x$ makes this self-adjoint operator's quadratic form zero; the [polarization identity](../../../../../polarization-identity.md) then gives $T^*T-TT^*=0$.

An [approximate eigenvalue](../../../../../approximate-eigenvalue.md) $\lambda$ has unit vectors $x_n$ with $\|(T-\lambda I)x_n\|\to0$. It is necessarily in the [spectrum](../../../../../spectrum-functional-analysis.md), since a bounded inverse would prevent this. Conversely suppose $\lambda$ is not an approximate eigenvalue. Then $A=T-\lambda I$ is bounded below, $\|Ax\|\geq c\|x\|$. It is injective and has closed range: a convergent sequence $Ax_n$ forces $x_n$ to be Cauchy. The operator $A$ is normal, so $\|A^*x\|=\|Ax\|$ and $\ker A^*=0$. The identity $(\operatorname{ran}A)^\perp=\ker A^*$ makes its range dense. Closed and dense means surjective, and its inverse is bounded by $1/c$. Hence $\lambda$ is in the resolvent. This proves $\boxed{\sigma(T)=\sigma_{\rm ap}(T)}$.

## ↑ Ancestors (10)

1. [19G](../19g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
