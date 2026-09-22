<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [highest-weight vector](../../../../../../highest-weight-vector.md) is a nonzero vector $v_0$ satisfying $J_3v_0=jv_0$ and $J_+v_0=0$; its eigenvalue $j$ is the [highest weight](../../../../../../highest-weight-of-a-representation.md). Existence does not require the [Lie algebra representation](../../../../../../lie-algebra-representation.md) to be antihermitian. Since $V$ is a nonzero finite-dimensional complex [vector space](../../../../../../vector-space-split.md), $J_3$ has an eigenvector $v$ with some eigenvalue $\lambda$. The [commutator](../../../../../../commutator.md) with $J_+$ shows that each nonzero $J_+^kv$ has eigenvalue $\lambda+k$. Infinitely many such vectors would have distinct eigenvalues and be linearly independent, which is impossible. The last nonzero vector in this raising chain is therefore a [highest-weight vector](../../../../../../highest-weight-vector.md) $v_0$.

Put $v_\ell=J_-^\ell v_0$. The [ladder operator](../../../../../../ladder-operator.md) relations give $J_3v_\ell=(j-\ell)v_\ell$. The raising coefficient follows by expanding the commutator of $J_+$ with a power of $J_-$:

$$
\begin{aligned}
J_+v_\ell&=[J_+,J_-^\ell]v_0
=\sum_{r=0}^{\ell-1}J_-^rJ_3J_-^{\ell-1-r}v_0\\
&=\sum_{r=0}^{\ell-1}(j-\ell+1+r)v_{\ell-1}
=\frac{\ell(2j-\ell+1)}2v_{\ell-1}.
\end{aligned}
$$

The factor $1/2$ is essential: these [ladder operators](../../../../../../ladder-operator.md) have $[J_+,J_-]=J_3$, rather than the convention with $2J_3$. The same finite-dimensionality argument gives a last nonzero lowered vector $v_r$, with $J_-v_r=v_{r+1}=0$. Applying $J_+$ to $v_{r+1}=0$ yields

$$
0=\frac{(r+1)(2j-r)}2v_r,
$$

so **$2j=r\in\mathbb Z_{\ge0}$**. All $v_0,\ldots,v_r$ are nonzero and have distinct eigenvalues. Their span is invariant under $J_3,J_+,J_-$ and therefore under the original three generators. Irreducibility of the [Lie algebra representation](../../../../../../lie-algebra-representation.md) makes this span equal to $V$. Hence

$$
\boxed{j\in\left\{0,\tfrac12,1,\ldots\right\},\quad \dim V=2j+1,\quad V=\operatorname{span}\{J_-^\ell|j,j\rangle:0\le\ell\le2j\}.}
$$

In particular, the initial construction produces the largest eigenvalue of $J_3$, since its full spectrum is now $j,j-1,\ldots,-j$. This establishes the [highest weight](../../../../../../highest-weight-of-a-representation.md) without assuming beforehand that all eigenvalues are real or that $J_3$ is diagonalizable.

For the additional antihermitian [Lie algebra representation](../../../../../../lie-algebra-representation.md), the given definitions imply $J_3^\dagger=J_3$ and $J_+^\dagger=J_-$. Thus distinct $J_3$ eigenvalues give orthogonal [weight vectors](../../../../../../weight-vector.md). With $\|v_0\|=1$, write $N_\ell=\|v_\ell\|^2$. The adjoint relation and the raising coefficient give

$$
N_\ell=\langle v_{\ell-1},J_+J_-v_{\ell-1}\rangle
=\frac{\ell(2j-\ell+1)}2N_{\ell-1},\qquad N_0=1.
$$

Multiplying this recursion proves the [normalized highest-weight lowering formula](../../../../../../normalized-highest-weight-lowering-formula.md) in the present normalization:

$$
\boxed{N_\ell=\frac{(2j)!\,\ell!}{2^\ell(2j-\ell)!},\qquad |j,m\rangle=\frac{J_-^{j-m}|j,j\rangle}{\sqrt{N_{j-m}}}.}
$$

Every factorial argument is an integer, even for half-integral $j$. The displayed states have unit norm, mutually distinct eigenvalues, and span $V$, so they form an [orthonormal basis](../../../../../../orthonormal-basis.md). Their phase convention also fixes the positive ladder amplitudes

$$
J_\pm|j,m\rangle=\sqrt{\frac{(j\mp m)(j\pm m+1)}2}\,|j,m\pm1\rangle,
$$

with the endpoint actions interpreted as zero. These amplitudes will determine the [Clebsch-Gordan coefficients](../../../../../../clebsch-gordan-coefficients.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
