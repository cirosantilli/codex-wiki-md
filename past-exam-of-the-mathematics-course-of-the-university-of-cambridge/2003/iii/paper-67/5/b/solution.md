<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [circulant matrix](../../../../../../circulant-matrix.md) is singular, so the meaning of convergence needs care. If $C$ is the cyclic shift, $A=C+C^{-1}-2I$ has Fourier [eigenvalues](../../../../../../eigenvalue.md) $-4\sin^2(\pi j/n)$. Its [null space](../../../../../../kernel-of-a-linear-map.md) consists of constants. Therefore $Ax=b$ is solvable exactly when $\sum_jb_j=0$, and any solution is determined only up to a constant. Neither iteration can converge to a unique solution for arbitrary right-hand sides.

For a compatible $b$, fix one solution $x_*$ and examine the error. The [iteration matrix](../../../../../../iteration-matrix.md) of the [Jacobi method](../../../../../../jacobi-method.md) is $(C+C^{-1})/2$, with [eigenvalues](../../../../../../eigenvalue.md) $\cos(2\pi j/n)$. The constant mode has [eigenvalue](../../../../../../eigenvalue.md) one. For odd $n$ all other [eigenvalues](../../../../../../eigenvalue.md) have modulus less than one, so the iterates converge to $x_*+c\mathbf1$, with the constant selected by the initial mean. For even $n$, the alternating vector has [eigenvalue](../../../../../../eigenvalue.md) $-1$, producing an undamped oscillation. With $b=0$ and alternating initial vector this is an explicit nonconvergent example. For even $n$ convergence occurs only when that error component vanishes. When $\sum b_j\ne0$, the mean instead drifts by $-(\sum b_j)/(2n)$ at each step, so Jacobi cannot converge.

For [Gauss-Seidel iteration](../../../../../../gauss-seidel-method.md), put $K=-A=D+L+U$, so $K$ is positive semidefinite with diagonal two. The homogeneous error iteration is $e^+=Be$, $B=-(D+L)^{-1}U$. Updating a coordinate exactly minimizes $E(e)=e^TKe/2$ in that coordinate; completing the square gives an energy decrement $|\Delta e_j|^2$. Summing within a sweep gives

$$
E(e)-E(Be)=\sum_{j=1}^n|\Delta e_j|^2\geq0.
$$

The same identity holds for the Hermitian energy of complex vectors. If $Be=\lambda e$ and $e$ is nonconstant, its energy is positive, so $|\lambda|\leq1$. Equality forces every update to be zero, whence $Ke=0$ and $e$ is constant, a contradiction. Thus all nonconstant eigenmodes have modulus strictly below one.

The [eigenvalue](../../../../../../eigenvalue.md) one has only the constant [eigenspace](../../../../../../eigenspace.md). To exclude a generalized eigenvector at one, observe that

$$
w=(D+L)^T\mathbf1=(0,1,\ldots,1,2)^T,\qquad w^TB=w^T,\quad w^T\mathbf1=n.
$$

If $(B-I)v=\mathbf1$, multiplication by $w^T$ would give $0=n$. Hence the constant [eigenvalue](../../../../../../eigenvalue.md) is algebraically simple, and

$$
B^r\longrightarrow\mathbf1w^T/n.
$$

For compatible $b$, Gauss-Seidel therefore converges from every start to some solution, for either parity of $n$. Its limit differs from $x_*$ by $\mathbf1w^T(x^{(0)}-x_*)/n$. For an incompatible $b$, the affine update gives $w^Tx^{(r+1)}-w^Tx^{(r)}=-\sum_jb_j$, so the iterates again cannot converge.

Thus [semiconvergence of cyclic Poisson iterations](../../../../../../semiconvergence-of-cyclic-poisson-iterations.md) gives the precise answer:

$$
\boxed{\begin{array}{l}
\sum b_j\ne0:\ \text{neither iteration converges};\\
\sum b_j=0:\ \text{Gauss-Seidel converges to a solution for all }n;\\
\text{Jacobi converges from every start iff }n\text{ is odd}.
\end{array}}
$$

Both have spectral radius one on the unrestricted space, so neither meets the strict stationary-iteration criterion for a unique limit independent of the starting constant. A spectral radius of one alone is not a proof that Gauss-Seidel's compatible iterates fail to converge. A normalization or projection removing the constant mode makes this distinction explicit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
