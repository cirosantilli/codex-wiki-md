<h1 id="35a/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [one-dimensional freely jointed chain](../../../../../../../one-dimensional-freely-jointed-chain.md), counting right- and left-pointing links gives

$$
N_{\rightarrow}+N_{\leftarrow}=N,
\qquad
a(N_{\rightarrow}-N_{\leftarrow})=L.
$$

Therefore

$$
\boxed{N_{\rightarrow}=\frac12\left(N+\frac La\right),
\qquad
N_{\leftarrow}=\frac12\left(N-\frac La\right).}
$$

Choosing which links point right gives the [state degeneracy](../../../../../../../state-degeneracy.md)

$$
\boxed{\Omega(L,N)=\binom N{N_{\rightarrow}}
=\frac{N!}{N_{\rightarrow}!N_{\leftarrow}!}.}
$$

Put $x=L/(Na)$. Applying the [Stirling formula](../../../../../../../stirling-formula.md) to $S=k_B\log\Omega$ and discarding terms subleading in $N$ yields

$$
\boxed{S(L,N)=k_BN\left[
\log2-\frac{1+x}{2}\log(1+x)
-\frac{1-x}{2}\log(1-x)
\right],
\qquad x=\frac{L}{Na}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [35A](../../../35a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
