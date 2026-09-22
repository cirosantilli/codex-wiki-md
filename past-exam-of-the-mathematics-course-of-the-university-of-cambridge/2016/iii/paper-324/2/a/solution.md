<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $|\psi\rangle$ to be normalized and let $\Pi_{\mathcal G}$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the good subspace. The two [reflection operators](../../../../../../reflection-operator.md) are

$$
\boxed{I_\psi=I-2|\psi\rangle\langle\psi|,\qquad I_{\mathcal G}=I-2\Pi_{\mathcal G}.}
$$

The first fixes the hyperplane orthogonal to $|\psi\rangle$ and negates its normal direction. The second fixes $\mathcal G^\perp$ and negates $\mathcal G$. Both are [Hermitian operators](../../../../../../hermitian-operator.md) and [unitary operators](../../../../../../unitary-operator.md), since their defining projectors square to themselves. For a non-normalized nonzero vector, divide $|\psi\rangle\langle\psi|$ by $\langle\psi|\psi\rangle$.

Put $p=\langle\psi|\Pi_{\mathcal G}|\psi\rangle=\sin^2\theta$, with $0<\theta<\pi/2$, and define normalized orthogonal good and bad vectors

$$
|g\rangle=\frac{\Pi_{\mathcal G}|\psi\rangle}{\sqrt p},\qquad
|b\rangle=\frac{(I-\Pi_{\mathcal G})|\psi\rangle}{\sqrt{1-p}}.
$$

Then $|\psi\rangle=\sin\theta|g\rangle+\cos\theta|b\rangle$. **The [amplitude amplification theorem](../../../../../../amplitude-amplification.md) states** that the iterate $Q=-I_\psi I_{\mathcal G}$ satisfies, for every nonnegative integer $m$,

$$
\boxed{Q^m|\psi\rangle=\sin((2m+1)\theta)|g\rangle+\cos((2m+1)\theta)|b\rangle,\qquad
p_m=\sin^2((2m+1)\theta).}
$$

To prove it, the span of $|g\rangle,|b\rangle$ is invariant under both [reflection operators](../../../../../../reflection-operator.md). In that ordered orthonormal basis,

$$
I_{\mathcal G}=\begin{pmatrix}-1&0\\0&1\end{pmatrix},\qquad
Q=\begin{pmatrix}\cos2\theta&\sin2\theta\\-\sin2\theta&\cos2\theta\end{pmatrix}.
$$

Multiplying the second matrix into $(\sin\theta,\cos\theta)^T$ advances the angle by $2\theta$. Induction proves the formula, and projecting onto $\mathcal G$ gives $p_m$. The minus sign in $Q$ is just a global phase choice, but it makes the displayed state formula exact.

If $p$ is known, choose $m$ nearest to $\pi/(4\theta)-1/2$, with $m\geq0$. The final angle is within $\theta$ of $\pi/2$, so $p_m\geq\cos^2\theta=1-p$. For $p\leq1/2$, this is at least $1/2$ after $O(1/\sqrt p)$ iterations, and is close to one when $p$ is small. For $p>1/2$, measuring the initial state already has success above $1/2$. Repeated independent attempts with a success test give any fixed desired success probability. This is the quadratic improvement of [amplitude amplification](../../../../../../amplitude-amplification.md) over repeated sampling, which takes $O(1/p)$ attempts. At $p=0$ there is no good component to amplify, and at $p=1$ the initial state is already entirely good; these endpoint cases do not require the undefined normalized component vectors.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
