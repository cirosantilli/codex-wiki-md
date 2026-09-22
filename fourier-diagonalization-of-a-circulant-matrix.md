# Fourier diagonalization of a circulant matrix

↑ **Parent:** [Circulant matrix](circulant-matrix.md)

Use the negative-exponential forward [discrete Fourier transform](discrete-fourier-transform.md) and the $1/N$-normalized [inverse discrete Fourier transform](inverse-discrete-fourier-transform.md):

$$
F_{kn}=e^{-2\pi ikn/N},
\qquad
(F^{-1})_{nk}=\frac1N e^{2\pi ink/N}.
$$

For the circulant [matrix](matrix.md) with first column $c$, the [discrete Fourier mode](discrete-fourier-mode.md) $w^{(k)}_n=e^{2\pi ikn/N}$ is an [eigenvector](eigenvector.md) with [eigenvalue](eigenvalue.md)

$$
\boxed{\lambda_k=\sum_{\ell=0}^{N-1}c_\ell e^{-2\pi ik\ell/N}=(Fc)_k.}
$$

Indeed, substitution into [circular convolution](circular-convolution.md) gives

$$
(Cw^{(k)})_n
=\sum_{\ell=0}^{N-1}c_\ell e^{2\pi ik(n-\ell)/N}
=w^{(k)}_n\lambda_k.
$$

The columns of $F^{-1}$ are $w^{(k)}/N$, so the [diagonalization of a matrix](diagonalization-of-a-matrix.md) takes the form

$$
C=F^{-1}\operatorname{diag}(\lambda_0,\ldots,\lambda_{N-1})F.
$$

The [roots of unity](root-of-unity.md) give [orthogonality](orthogonal-vectors.md) of these [eigenvectors](eigenvector.md); dividing each $w^{(k)}$ by $\sqrt N$ makes the [basis](basis.md) [orthonormal](orthonormal-set.md). Consequently, every complex circulant [matrix](matrix.md) is a [normal matrix](normal-matrix.md), including ones that are not [Hermitian matrices](hermitian-operator.md).

The sign convention matters. For $c=(1,2,0,0)^T$, the circulant [matrix](matrix.md) is

$$
C=\begin{pmatrix}
1&0&0&2\\
2&1&0&0\\
0&2&1&0\\
0&0&2&1
\end{pmatrix},
\qquad
(\lambda_0,\lambda_1,\lambda_2,\lambda_3)=(3,1-2i,-1,1+2i).
$$

Changing the direction of the shift or the sign in the [discrete Fourier transform](discrete-fourier-transform.md) changes which complex [eigenvalue](eigenvalue.md) goes with which [discrete Fourier mode](discrete-fourier-mode.md). A real symmetric example alone would conceal that distinction.

For a [linear system](system-of-linear-equations.md) $Cx=b$, put $\widehat x=Fx$ and $\widehat b=Fb$. The equation becomes $N$ independent scalar equations

$$
\lambda_k\widehat x_k=\widehat b_k.
$$

If every $\lambda_k$ is nonzero, divide to find the unique [vector](vector.md) $x$ and apply the [inverse discrete Fourier transform](inverse-discrete-fourier-transform.md). If some $\lambda_k=0$, a [vector](vector.md) $x$ satisfying the [linear system](system-of-linear-equations.md) exists exactly when $\widehat b_k=0$ at every such index; the corresponding $\widehat x_k$ remain free. This is a concrete version of the [Fredholm alternative](fredholm-alternative.md) in a finite-dimensional setting.

With an appropriate [Fast Fourier transform](fast-fourier-transform.md), multiplication or a compatible solve takes $O(N\log N)$ arithmetic operations, instead of forming a dense [matrix](matrix.md) and applying general [Gaussian elimination](gaussian-elimination.md). The gain comes from the periodic structure; an arbitrary [matrix](matrix.md) does not have this shared [basis](basis.md) of [discrete Fourier modes](discrete-fourier-mode.md).[Strang, MIT 18.065 Lecture 31: Fourier eigenvectors and fast computation](https://ocw.mit.edu/courses/18-065-matrix-methods-in-data-analysis-signal-processing-and-machine-learning-spring-2018/resources/lecture-31-eigenvectors-of-circulant-matrices-fourier-matrix/)

## ↑ Ancestors (6)

1. [Circulant matrix](circulant-matrix.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Circulant matrix](circulant-matrix.md)
- [Laplacian matrix](laplacian-matrix.md)
- [Periodic Poisson equation on a four-point cycle](periodic-poisson-equation-on-a-four-point-cycle.md)
