<h1 id="2/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Write $\ell=r/2$; the requested expression requires the positive even integer $r\geq2$. Split the thin [singular value decomposition](../../../../../singular-value-decomposition.md) after $\ell$ columns:

$$
A=U_aD_aV_a^T+U_bD_bV_b^T,\qquad
\Omega_a=V_a^TX\in\mathbb R^{\ell\times r},\qquad
\Omega_b=V_b^TX\in\mathbb R^{(n-\ell)\times r}.
$$

Here $\|D_b\|_2=\sigma_{\ell+1}=\|A-A_\ell\|_2$. Each column of a [Gaussian random matrix](../../../../../gaussian-random-matrix.md) is an [orthogonally invariant random vector](../../../../../orthogonally-invariant-random-vector.md): its [probability density function](../../../../../probability-density-function.md) is proportional to $\exp(-\|z\|_2^2/2)$, and an [orthogonal matrix](../../../../../orthogonal-matrix.md) preserves both $\|z\|_2$ and volume. Thus $V^TX$, where $V=[V_a,V_b]$, again has [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md) [standard normal](../../../../../standard-normal-distribution.md) entries. In particular both displayed blocks have the Gaussian distributions needed below.

First prove a [deterministic error bound for a randomized range finder](../../../../../deterministic-error-bound-for-a-randomized-range-finder.md). Put $P=QQ^T$ and suppose $\Omega_a$ has [full row rank](../../../../../full-row-rank.md). Its [Moore-Penrose pseudoinverse](../../../../../moore-penrose-inverse.md) is $\Omega_a^\dagger=\Omega_a^T(\Omega_a\Omega_a^T)^{-1}$, so $\Omega_a\Omega_a^\dagger=I_\ell$. The [QR decomposition](../../../../../qr-decomposition.md) implies $(I_m-P)AX=0$, hence

$$
(I_m-P)U_aD_a\Omega_a=-(I_m-P)U_bD_b\Omega_b.
$$

Multiplication by $\Omega_a^\dagger$ expresses the missed leading columns in terms of the trailing columns. Substitution into $(I_m-P)A$ gives the exact identity

$$
(I_m-P)A=(I_m-P)U_bD_b
\begin{pmatrix}-\Omega_b\Omega_a^\dagger&I_{n-\ell}\end{pmatrix}V^T.
$$

For any [matrix](../../../../../matrix.md) $F$, the [spectral norm](../../../../../matrix-2-norm.md) of $[-F\ I]$ is $\sqrt{1+\|F\|_2^2}$, because its product with its [transpose](../../../../../transpose.md) is $FF^T+I$. Using [submultiplicativity of the operator norm](../../../../../submultiplicativity-of-the-operator-norm.md), the [orthonormality](../../../../../orthonormal-set.md) of $U_b$, and the contraction property of the [orthogonal projection](../../../../../orthogonal-projection.md), we obtain

$$
\boxed{\|A-PA\|_2\leq\sigma_{\ell+1}
\sqrt{1+\|\Omega_b\Omega_a^\dagger\|_2^2}}.
$$

This estimate is deterministic and also covers rank-deficient $A$; if $\sigma_{\ell+1}=0$, its right-hand side vanishes.

Now use the paper's permitted [singular value](../../../../../singular-value.md) estimates. Apply the lower estimate to the tall [matrix](../../../../../matrix.md) $\Omega_a^T$ of size $r\times\ell$, rather than to its wide [transpose](../../../../../transpose.md). It gives

$$
\sigma_{\min}(\Omega_a)\geq\sqrt r-\sqrt\ell
=\sqrt r(1-1/\sqrt2)>0,\qquad
\|\Omega_a^\dagger\|_2\leq\frac1{\sqrt r-\sqrt\ell}.
$$

The upper estimate for $\Omega_b$, transposing if necessary, gives

$$
\|\Omega_b\|_2\leq\sqrt{n-\ell}+\sqrt r\leq2\sqrt n.
$$

Thus, with $K=2/(1-1/\sqrt2)$,

$$
\|\Omega_b\Omega_a^\dagger\|_2\leq K\sqrt{n/r}.
$$

Since $n/r>1$, the deterministic estimate yields

$$
\boxed{\|A-\widehat A\|_2
\leq C\sqrt{\frac nr}\,\|A-A_{r/2}\|_2},\qquad C=\sqrt{1+K^2}.
$$

This proves the requested conclusion under the explicitly authorized estimates.

**The probabilistic qualification is necessary.** A [Gaussian random matrix](../../../../../gaussian-random-matrix.md) does not always have all its [singular values](../../../../../singular-value.md) between the two endpoints printed in the hint. Already a $1\times1$ example would require $|Z|\leq2$ for every [standard normal random variable](../../../../../standard-normal-random-variable.md) $Z$, which fails with positive [probability](../../../../../probability.md). The proof above holds on the event where the two block estimates hold. In a probabilistic formulation one supplies estimates for that event, usually allowing a positive margin in both endpoints; no failure probability is specified by the paper.

Nor can the requested inequality with one universal $C$ hold almost surely for every $A$. For example, take $n=m=3$, $r=2$, $A=\operatorname{diag}(L,1,1)$ with $L>1$, and a sampling [matrix](../../../../../matrix.md)

$$
X_0=\begin{pmatrix}0&0\\1&0\\0&1\end{pmatrix}.
$$

At $X_0$, the sampled [column space](../../../../../column-space.md) misses the first coordinate, so $\|A-\widehat A\|_2=L$, whereas $\|A-A_1\|_2=1$. Choose $L>C\sqrt{3/2}$. Because $AX_0$ has [full column rank](../../../../../full-column-rank.md), its [orthogonal projection](../../../../../orthogonal-projection.md) depends continuously on $X$ near $X_0$ through $AX(X^TA^TAX)^{-1}X^TA^T$. The strict violation persists in an open neighborhood of $X_0$. The joint Gaussian [probability density function](../../../../../probability-density-function.md) is positive there, so that neighborhood has positive [probability](../../../../../probability.md). This identifies the missing qualification without weakening the conditional calculation.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
