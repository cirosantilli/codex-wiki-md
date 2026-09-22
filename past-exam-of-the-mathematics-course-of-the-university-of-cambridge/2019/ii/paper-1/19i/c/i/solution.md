<h1 id="19i/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $e_0,\ldots,e_{n-1}$ be the standard basis and let the generator $g$ send $e_j$ to $e_{j+1}$ modulo $n$. The constant vector

$$
c_0=\sum_{j=0}^{n-1}e_j
$$

spans a trivial module. Since $n$ is even, the alternating vector

$$
c_{n/2}=\sum_{j=0}^{n-1}(-1)^je_j
$$

spans a sign module on which $g$ acts by $-1$.

For each $1\leq k<n/2$, define the real [discrete Fourier modes](../../../../../../../discrete-fourier-mode.md)

$$
c_k=\sum_{j=0}^{n-1}\cos\left(\frac{2\pi kj}{n}\right)e_j,
\qquad
s_k=\sum_{j=0}^{n-1}\sin\left(\frac{2\pi kj}{n}\right)e_j.
$$

The plane $W_k=\operatorname{span}\{c_k,s_k\}$ is invariant, and $g$ acts on it by rotation through $2\pi k/n$. Since this angle is neither zero nor $\pi$, $W_k$ is irreducible over $\mathbb R$. The traces $2\cos(2\pi k/n)$ are distinct for $1\leq k<n/2$, so these modules are pairwise nonisomorphic. Orthogonality of the [discrete Fourier transform](../../../../../../../discrete-fourier-transform.md) gives

$$
\boxed{\mathbb RC_n
=\langle c_0\rangle\oplus\langle c_{n/2}\rangle
\oplus\bigoplus_{k=1}^{(n-2)/2}W_k}.
$$

The dimensions sum to $1+1+2(n-2)/2=n$, so this is the whole regular module: two nonisomorphic one-dimensional summands and $(n-2)/2$ nonisomorphic two-dimensional summands.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [19I](../../../19i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
