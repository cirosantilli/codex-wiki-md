<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [history-subspace propagation Hamiltonian](../../../../../../../history-subspace-propagation-hamiltonian.md) has diagonal entries $1/2$ at the endpoints and $1$ in the interior, and nearest-neighbour entries $-1/2$. The [spectrum of a path propagation Hamiltonian](../../../../../../../spectrum-of-a-path-propagation-hamiltonian.md) is

$$
\boxed{\lambda_k=1-\cos\left(\frac{\pi k}{T+1}\right),
\qquad k=0,\ldots,T.}
$$

To see the indexing directly, set $q_k=\pi k/(T+1)$ and $f_t=\cos[q_k(t+1/2)]$. The interior difference equation gives $Ef=(1-\cos q_k)f$. The endpoint equations correspond to $f_{-1}=f_0$ and $f_{T+1}=f_T$, both satisfied by these $q_k$. The $T+1$ distinct [eigenvalues](../../../../../../../eigenvalue.md) and their nonzero [eigenvectors](../../../../../../../eigenvector.md) exhaust the matrix.

The zero [eigenvalue](../../../../../../../eigenvalue.md) is simple, so

$$
\boxed{\Delta(E)=1-\cos\left(\frac{\pi}{T+1}\right)
\geq\frac{2}{(T+1)^2}=\Omega(T^{-2}).}
$$

The inequality uses $\sin x\geq2x/\pi$ on $[0,\pi/2]$ and $1-\cos q=2\sin^2(q/2)$.

The supplied path-matrix hint sums through $i=N$ while listing a basis ending at $N$. That last summand would introduce an extra vertex. The matrix derived in (a) has exactly $T$ edges and $T+1$ vertices, as used here; this also proves the needed spectrum without relying on the misindexed summation.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 67](../../../../paper-67-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
