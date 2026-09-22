<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

[Anti-self-adjoint](../../../../skew-adjoint-generator.md) means $T^*=-T$. Unitary means $T^*T=TT^*=I$, so $T^{-1}=T^*$. For a [unitary operator](../../../../unitary-operator.md) $\|Tu\|^2=\langle u,T^*Tu\rangle=\|u\|^2$, and the space is nonzero. Thus **$\|T\|=1$**.

The [series](../../../../series-mathematics.md) for the exponential converges absolutely in the [Banach algebra](../../../../banach-algebra-split.md) $B(V)$, since $\sum_n\|T^n/n!\|\leq e^{\|T\|}$. The adjoint is [norm](../../../../norm.md) continuous and conjugate linear, and its action on these real scalar coefficients gives $(e^T)^*=e^{T^*}$. The absolutely convergent Cauchy product gives

$$
e^Te^{-T}=e^{-T}e^T=I,
$$

because its degree-$n$ coefficient for $n>0$ is $T^n\sum_{j=0}^n(-1)^j/[j!(n-j)!]=0$. If $T^*=-T$, these identities prove **$e^T$ is unitary**.

If $T$ is invertible, zero is outside the spectrum of $T^{-1}$. For $\mu\ne0$ the factorization

$$
T^{-1}-\mu I=-\mu T^{-1}(T-\mu^{-1}I)
$$

shows that the left side is invertible exactly when the final factor is. Hence

$$
\boxed{\sigma(T^{-1})=\{\lambda^{-1}:\lambda\in\sigma(T)\}.}
$$

For unitary $T$, both $T$ and $T^{-1}=T^*$ have [norm](../../../../norm.md) one. The [norm](../../../../norm.md) bound on each spectrum gives $|\lambda|\leq1$ and $|\lambda^{-1}|\leq1$, forcing **$\sigma(T)$ to lie on the unit circle**.

The converse fails: on $\mathbb C^2$ with its usual [inner product](../../../../inner-product-split.md) take

$$
\boxed{T=\begin{pmatrix}1&1\\0&1\end{pmatrix}.}
$$

Its spectrum is $\{1\}$, but $T^*T=\begin{pmatrix}1&1\\1&2\end{pmatrix}\ne I$, so it is not unitary.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
