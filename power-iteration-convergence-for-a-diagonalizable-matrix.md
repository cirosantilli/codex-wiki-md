# Power iteration convergence for a diagonalizable matrix

↑ **Parent:** [Power iteration](power-iteration.md)

Suppose $A\in\mathbb C^{n\times n}$ is a [diagonalizable matrix](diagonalizable-matrix.md), $n\ge2$, with an [eigenbasis](eigenbasis.md) $v_1,\ldots,v_n$ and [spectral decomposition](spectral-decomposition.md)

$$
A=V\Lambda V^{-1},\qquad V=(v_1\ \cdots\ v_n),\qquad \Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).
$$

Assume the [dominant eigenvalue](dominant-eigenvalue.md) $\lambda_1$ is a [simple eigenvalue](simple-eigenvalue.md) and

$$
|\lambda_1|>|\lambda_2|\ge\cdots\ge|\lambda_n|,\qquad x_0=\sum_{j=1}^n c_jv_j,\qquad c_1\ne0.
$$

Then the normalized [power iteration](power-iteration.md) approaches the one-dimensional [eigenspace](eigenspace.md) of $\lambda_1$. Its asymptotic direction-error bound has factor $\gamma=|\lambda_2/\lambda_1|<1$. This [spectral gap](spectral-gap.md) is a gap in [modulus](modulus.md): if $g=|\lambda_1|-|\lambda_2|$, then $\gamma=1-g/|\lambda_1|$. A small relative gap gives slow convergence.[Power Method](templates-for-the-solution-of-algebraic-eigenvalue-problems-a-practical-guide/power-method.md)

The short proof is the exact [eigenbasis](eigenbasis.md) identity

$$
\frac{A^kx_0}{c_1\lambda_1^k}=v_1+\sum_{j=2}^n\frac{c_j}{c_1}\left(\frac{\lambda_j}{\lambda_1}\right)^kv_j.
$$

The remaining sum has [norm](norm.md) bounded by a constant times $\gamma^k$. This proves convergence of direction, allowing a changing sign or complex factor. A tiny $c_1$ or a poorly conditioned, [nonorthogonal](nonorthogonal-vectors.md) [eigenbasis](eigenbasis.md) can delay visible convergence: the [condition number](condition-number.md) of $V$ affects constants, while $\gamma$ controls the eventual rate. The bound need not be an equality; if the initial coefficient of the second-largest [eigenvalue](eigenvalue.md) vanishes, the [active spectrum of the power method](active-spectrum-of-the-power-method.md) gives a faster rate. When $\gamma=0$, all unwanted components disappear after one multiplication.[§1, PDF pp. 1–2: diagonalizable expansion and nonzero first coordinate of the starting vector](numerical-analysis-spring-2022/power-iteration-2022-03-07-lecture-notes.md)

The hypothesis is $c_1=(V^{-1}x_0)_1\ne0$, not an ordinary nonzero [inner product](inner-product.md) with the right [eigenvector](eigenvector.md). Let $w_1^*$ be the first row of $V^{-1}$, a [left eigenvector](left-eigenvector.md) normalized so $w_1^*v_j$ is $1$ for $j=1$ and $0$ otherwise; $*$ denotes [conjugate transpose](conjugate-transpose.md). Then $c_1=w_1^*x_0$. For a [Hermitian matrix](hermitian-operator.md), choose an [orthonormal eigenbasis](orthonormal-eigenbasis.md) and the criterion becomes $v_1^*x_0\ne0$: the starting [vector](vector.md) must be [nonorthogonal](nonorthogonal-vectors.md) to the dominant [eigenvector](eigenvector.md). For a general [diagonalizable matrix](diagonalizable-matrix.md), the [nonorthogonal](nonorthogonal-vectors.md) [eigenbasis](eigenbasis.md) makes these two tests different, as illustrated under [power iteration failure cases](power-iteration-failure-cases.md).

**Table of contents**

- [Power iteration direction error](power-iteration-direction-error.md)

## ↑ Ancestors (7)

1. [Power iteration](power-iteration.md)
2. [Numerical linear algebra](numerical-linear-algebra.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Power iteration direction error](power-iteration-direction-error.md)
- [Power iteration eigenpair diagnostics](power-iteration-eigenpair-diagnostics.md)
- [Sign and phase in power iteration](sign-and-phase-in-power-iteration.md)
