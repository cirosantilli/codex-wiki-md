<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $N$ to be an [even number](../../../../../../even-number.md) for a perfectly bipartite periodic chain and make the [bipartite spin rotation](../../../../../../bipartite-spin-rotation.md) by $\pi$ about the $x$ axis on alternating sites. In the local frame the [Néel state](../../../../../../neel-state.md) has all spins up, while a bond becomes

$$
\mathbf S_i\cdot\mathbf S_j=-\widetilde S_i^z\widetilde S_j^z+\tfrac12(\widetilde S_i^+\widetilde S_j^++\widetilde S_i^-\widetilde S_j^-).
$$

The [linear spin-wave approximation](../../../../../../linear-spin-wave-approximation.md) keeps $\widetilde S^z=S-a^\dagger a$ and $\widetilde S^\pm\simeq\sqrt{2S}(a,a^\dagger)$. Therefore

$$
H=-NJS^2+JS\sum_{\langle ij\rangle}(n_i+n_j+a_ia_j+a_i^\dagger a_j^\dagger)+O(S^0).
$$

Every site has two neighbours. [Fourier transform](../../../../../../fourier-transform.md) gives $\sum_{\langle ij\rangle}(n_i+n_j)=2\sum_kn_k$ and pairing coefficient $\gamma_k=\cos k$, so

$$
H=-NJS^2+2JS\sum_ka_k^\dagger a_k+JS\sum_k\gamma_k(a_ka_{-k}+a_k^\dagger a_{-k}^\dagger)+O(S^0).
$$

The [bosonic Nambu normal-ordering shift](../../../../../../bosonic-nambu-normal-ordering-shift.md) follows from $a_{-k}a_{-k}^\dagger=1+a_{-k}^\dagger a_{-k}$. It adds $NJS$ inside the matrix expression, which must be subtracted in its constant. Hence

$$
\boxed{H=-NJS(S+1)+JS\sum_k(a_k^\dagger,a_{-k})
\begin{pmatrix}1&\gamma_k\\\gamma_k&1\end{pmatrix}
\begin{pmatrix}a_k\\a_{-k}^\dagger\end{pmatrix}+O(S^0).}
$$

A periodic chain with an [odd number](../../../../../../odd-number.md) of sites is frustrated at the boundary and lacks this exact two-sublattice reference; the bulk thermodynamic calculation uses the even-chain sequence.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
