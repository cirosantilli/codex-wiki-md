<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the norm to be the [Euclidean norm](../../../../../../euclidean-norm.md). The solution is $\mathbf q(t)=e^{tA}\mathbf q(0)$, so optimal growth is the [operator norm](../../../../../../operator-norm.md) $G(t)=\|e^{tA}\|_2$, equivalently the largest [singular value](../../../../../../singular-value.md) of the [matrix exponential](../../../../../../matrix-exponential.md). Let $s(A)$ be the [spectral abscissa](../../../../../../spectral-abscissa.md) and let $w(A)=\lambda_{\max}((A+A^*)/2)$ be the [numerical abscissa](../../../../../../euclidean-logarithmic-norm.md). The [Euclidean semigroup growth bounds](../../../../../../euclidean-semigroup-growth-bounds.md) are

$$
\boxed{e^{ts(A)}\leq G(t)\leq e^{tw(A)},\qquad t\geq0.}
$$

For the lower bound, the [spectral radius](../../../../../../spectral-radius.md) of $e^{tA}$ is $e^{ts(A)}$ and is bounded by its [operator norm](../../../../../../operator-norm.md). For the upper bound, differentiating $\|\mathbf q\|_2^2$ gives $2\operatorname{Re}(\mathbf q^*A\mathbf q)\leq2w(A)\|\mathbf q\|_2^2$, and integration gives the result. A [non-normal matrix](../../../../../../non-normal-matrix.md) can have $w(A)>s(A)$, allowing transient amplification even when all its [eigenvalues](../../../../../../eigenvalue.md) have negative [real parts](../../../../../../real-part.md).

For the triangular matrix, $s(M)=-1/R$. The [eigenvalues](../../../../../../eigenvalue.md) of its [Hermitian part](../../../../../../hermitian-part-of-a-matrix.md) are $-3/(2R)\pm\tfrac12\sqrt{1+R^{-2}}$, so

$$
\boxed{e^{-t/R}\leq G(t)\leq\exp\left[\left(-\frac{3}{2R}+\frac12\sqrt{1+\frac1{R^2}}\right)t\right].}
$$

The upper exponent becomes positive when $R>\sqrt8$, even though the long-time spectrum is stable.

The two equations are $q_1'=-q_1/R$ and $q_2'=q_1-2q_2/R$. Solve the first, then use an [integrating factor](../../../../../../integrating-factor.md) in the second. Writing $s=t/R$, $a=e^{-s}$, $b=e^{-2s}$ and $c=R(a-b)$ gives

$$
\boxed{B(t)=e^{tM}=\begin{pmatrix}a&0\\c&b\end{pmatrix}.}
$$

The maximizing initial state is the unit [eigenvector](../../../../../../eigenvector.md) of $B^*B$ belonging to its largest [eigenvalue](../../../../../../eigenvalue.md). Here

$$
B^*B=\begin{pmatrix}a^2+c^2&cb\\cb&b^2\end{pmatrix},\qquad G(t)^2=\frac{T+\sqrt{T^2-4a^2b^2}}2,\qquad T=a^2+b^2+c^2.
$$

For $t>0$, define

$$
d=\frac{a^2+c^2-b^2}{2cb}=\frac{e^s+1}{2R}+\frac R2(e^s-1),\qquad r=\sqrt{1+d^2}-d.
$$

The [optimal initial state for triangular stable shear](../../../../../../optimal-initial-state-for-triangular-stable-shear.md) is therefore

$$
\boxed{\mathbf q_{\rm opt}(0)=\frac1{\sqrt{1+r^2}}\begin{pmatrix}1\\r\end{pmatrix}.}
$$

Multiplication by any nonzero complex [scalar](../../../../../../scalar.md) gives the same growth ratio; at $t=0$, every nonzero initial state is optimal.

For $t\gg R$, $d\to\infty$ and $r\to0$. Thus **the optimal initial state tends to $(1,0)^T$**, and $G(t)\sim e^{-t/R}\sqrt{1+R^2}$. The initial first component excites the slower eigenmode and its amplified second component.

For $t\ll R$, the exact expression gives $d=(R^{-1}+t/2)[1+O(t/R)]$. Accordingly the [short-relative-time optimal state for triangular shear](../../../../../../short-relative-time-optimal-state-for-triangular-shear.md) uses

$$
\boxed{r\sim\sqrt{1+\left(\frac1R+\frac t2\right)^2}-\left(\frac1R+\frac t2\right).}
$$

This retains both the unequal damping rates and the shear. If $R\gg1$, it reduces to $r\sim(\sqrt{t^2+4}-t)/2$, the maximizing direction for the shear matrix $\begin{pmatrix}1&0\\t&1\end{pmatrix}$. If time also tends to zero at fixed $R$, it instead tends to $r=\sqrt{1+R^{-2}}-R^{-1}$, the largest-[eigenvalue](../../../../../../eigenvalue.md) direction of the [Hermitian part](../../../../../../hermitian-part-of-a-matrix.md) of $M$. Merely setting $t/R$ small does not justify setting $t$ small; the exact formula resolves both possibilities.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
