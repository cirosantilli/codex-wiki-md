<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\Pi$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the good [linear subspace](../../../../../../vector-subspace.md) $\mathcal G$, and let $|\psi\rangle$ be a prepared unit vector with $p=\langle\psi|\Pi|\psi\rangle$. For $0<p<1$, define

$$
\sin\theta=\sqrt p,\qquad
|g\rangle=\frac{\Pi|\psi\rangle}{\sqrt p},\qquad
|b\rangle=\frac{(I-\Pi)|\psi\rangle}{\sqrt{1-p}}.
$$

The [amplitude amplification theorem](../../../../../../amplitude-amplification.md) states that, if the [reflection operators](../../../../../../reflection-operator.md) about the initial state and the good subspace can be implemented, the iteration

$$
Q=(2|\psi\rangle\langle\psi|-I)(I-2\Pi)
$$

satisfies

$$
\boxed{Q^j|\psi\rangle=\sin((2j+1)\theta)|g\rangle+\cos((2j+1)\theta)|b\rangle.}
$$

To prove it, the two reflections preserve the [linear span](../../../../../../linear-span.md) of $|g\rangle,|b\rangle$. In this ordered [orthonormal basis](../../../../../../orthonormal-basis.md), direct multiplication gives

$$
Q=\begin{pmatrix}\cos2\theta&\sin2\theta\\-\sin2\theta&\cos2\theta\end{pmatrix}.
$$

Multiplying this [rotation matrix](../../../../../../rotation-matrix.md) by $(\sin\alpha,\cos\alpha)^T$ replaces $\alpha$ by $\alpha+2\theta$, proving the formula by [mathematical induction](../../../../../../mathematical-induction.md).

For known $0<p\leq1/2$, choose $j$ to be a nearest nonnegative integer to $\pi/(4\theta)-1/2$. Then $|(2j+1)\theta-\pi/2|\leq\theta$, so measurement finds the good subspace with probability at least $1-p$, using $O(p^{-1/2})$ iterations. For $p>1/2$, measurement of the initial state already has constant success probability. If $p=1$ success is certain; if $p=0$ these reflections cannot create any good component. If $|\psi\rangle=A|0\rangle$, the initial-state reflection is $A(2|0\rangle\langle0|-I)A^\dagger$, implemented using [quantum state preparation](../../../../../../quantum-state-preparation.md) and its [inverse quantum circuit](../../../../../../inverse-quantum-circuit.md).

<a id="2/a/image-amplitude-amplification-as-a-rotation"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324-amplitude-amplification.png)

**[Figure 1](#2/a/image-amplitude-amplification-as-a-rotation). Amplitude amplification as a rotation**. Each iteration adds the angle $2\theta$ in the good-bad plane. The probability rises near one and then falls again, so the stopping time matters.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
