<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

For ordered bases $\mathcal B=(v_1,\ldots,v_n)$ of $V$ and $\mathcal C=(w_1,\ldots,w_m)$ of $W$, the [matrix representation of a linear map](../../../../../matrix-representation-of-a-linear-map.md) $\gamma:V\to W$ is the matrix whose $j$th column consists of the $\mathcal C$-coordinates of $\gamma(v_j)$. Thus

$$
[\gamma(v)]_{\mathcal C}
=[\gamma]_{\mathcal C\leftarrow\mathcal B}[v]_{\mathcal B}.
$$

The operators $\alpha,\beta:V\to V$ are [conjugate linear operators](../../../../../conjugate-linear-operators.md) when there is an isomorphism $s:V\to V$ such that

$$
\beta=s^{-1}\alpha s.
$$

In one basis their matrices therefore satisfy $[\beta]=[s]^{-1}[\alpha][s]$, so they are similar matrices.

For invertible $\beta$, the map

$$
\phi_\beta(A)=\beta^{-1}A\beta
$$

is linear, and its inverse is $A\mapsto\beta A\beta^{-1}$; hence it is a linear isomorphism of $\operatorname{End}(V)$. If $\beta'=s^{-1}\beta s$, define $\Phi_s(A)=s^{-1}As$. A direct substitution gives

$$
\phi_{\beta'}=\Phi_s\phi_\beta\Phi_s^{-1},
$$

so $\phi_{\beta'}$ and $\phi_\beta$ are conjugate. This is the [conjugation operator on an endomorphism space](../../../../../conjugation-operator-on-an-endomorphism-space.md).

It remains to compute the [Jordan normal form](../../../../../jordan-normal-form.md) over $\mathbb C$. By the preceding conjugacy, we may put $\beta$ in Jordan form.

If

$$
\beta=\begin{pmatrix}\lambda&0\\0&\mu\end{pmatrix},
\qquad \lambda\mu\ne0,
$$

then the matrix units $E_{ij}$ are eigenvectors because

$$
\phi_\beta(E_{ij})=\frac{\beta_j}{\beta_i}E_{ij}.
$$

Thus

$$
\boxed{\operatorname{JNF}(\phi_\beta)
=\operatorname{diag}\left(1,1,\frac\mu\lambda,\frac\lambda\mu\right)}.
$$

This includes the scalar case $\lambda=\mu$, when $\phi_\beta$ is the identity.

Otherwise $\beta$ has one size-two [Jordan block](../../../../../jordan-block.md). Multiplying $\beta$ by a nonzero scalar does not change $\phi_\beta$, and conjugating within its Jordan class allows us to use $J=I+N$ with $N=E_{12}$. Put $D=\phi_J-I$. Direct multiplication gives

$$
D(E_{11})=E_{12},\quad D(E_{12})=0,\quad
D(E_{22})=-E_{12},
$$



$$
D(E_{21})=E_{22}-E_{11}-E_{12}.
$$

Hence $D^3=0$, $\operatorname{rank}D=2$, and $\operatorname{rank}D^2=1$. The nilpotent Jordan blocks of $D$ therefore have sizes three and one. Adding the identity gives

$$
\boxed{\operatorname{JNF}(\phi_\beta)=J_3(1)\oplus J_1(1)}.
$$

These two cases are the [Jordan normal form of conjugation on two-by-two matrices](../../../../../jordan-normal-form-of-conjugation-on-two-by-two-matrices.md).

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
