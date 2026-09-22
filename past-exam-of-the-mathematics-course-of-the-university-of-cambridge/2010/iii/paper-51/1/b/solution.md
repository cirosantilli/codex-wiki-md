<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Label an [orthonormal basis](../../../../../../orthonormal-basis.md) of the $n$-dimensional [Hilbert space](../../../../../../hilbert-space-split.md) by $j=0,\ldots,n-1$, with indices modulo $n$. Let

$$
\omega=e^{2\pi i/n},\qquad X|j\rangle=|j+1\rangle,\qquad Z|j\rangle=\omega^j|j\rangle.
$$

These are the shift and phase [Heisenberg-Weyl operators](../../../../../../heisenberg-weyl-operator.md). Alice holds the input $S$ and one half $A$ of the shared [maximally entangled state](../../../../../../maximally-entangled-state.md)

$$
|\Phi_n\rangle_{AB}=\frac1{\sqrt n}\sum_{j=0}^{n-1}|j\rangle_A|j\rangle_B.
$$

She measures $SA$ in the [generalized Bell basis](../../../../../../generalized-bell-basis.md)

$$
|B_{pq}\rangle_{SA}=\frac1{\sqrt n}\sum_{j=0}^{n-1}\omega^{pj}|j\rangle_S|j+q\rangle_A,
\qquad p,q=0,\ldots,n-1.
$$

Its inner products are

$$
\langle B_{pq}|B_{p'q'}\rangle
=\delta_{qq'}\frac1n\sum_{j=0}^{n-1}\omega^{(p'-p)j}
=\delta_{pp'}\delta_{qq'}.
$$

There are $n^2$ orthonormal vectors in an $n^2$-dimensional space, so this is a complete [projective measurement](../../../../../../projective-measurement.md).

For an unknown normalized state $|u\rangle=\sum_j u_j|j\rangle$, its contraction with measurement outcome $(p,q)$ gives Bob's unnormalized state

$$
\begin{aligned}
{}_{SA}\langle B_{pq}|\bigl(|u\rangle_S|\Phi_n\rangle_{AB}\bigr)
&=\frac1n\sum_j u_j\omega^{-pj}|j+q\rangle_B\\
&=\frac1nX^qZ^{-p}|u\rangle_B.
\end{aligned}
$$

Each outcome has [probability](../../../../../../probability.md) $1/n^2$, independently of the input. Alice communicates the two $n$-valued labels, and Bob applies the ordered inverse

$$
\boxed{U_{pq}=Z^pX^{-q},\qquad
U_{pq}\left(\frac1nX^qZ^{-p}|u\rangle\right)=\frac1n|u\rangle.}
$$

The order matters because shift and phase operators do not generally commute. Normalizing the branch recovers the unknown state exactly, and all outcomes are corrected, so success is deterministic. The quantum resource is one maximally entangled pair of local dimension $n$. The classical resource is an $n^2$-valued message, with information content $2\log_2 n$ bits; $\lceil\log_2(n^2)\rceil$ ordinary bits suffice in fixed-length binary encoding.

This is faithful [qudit teleportation](../../../../../../qudit-teleportation.md) even for an input entangled with a reference $R$. Expand a joint pure state as $\sum_j|j\rangle_S|r_j\rangle_R$, without requiring the reference vectors to be orthogonal. The same contraction and correction act on each system basis vector, producing $n^{-1}\sum_j|j\rangle_B|r_j\rangle_R$. Thus the whole joint state, not just a reduced state, is preserved. Linearity extends the conclusion to mixed inputs. This is [teleportation as an identity channel on a reference](../../../../../../teleportation-as-an-identity-channel-on-a-reference.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
