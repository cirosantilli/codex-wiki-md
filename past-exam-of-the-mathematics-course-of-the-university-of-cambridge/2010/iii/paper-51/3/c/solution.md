<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Alice makes a two-outcome local [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) with [Kraus operators](../../../../../../kraus-operator.md)

$$
K_{\rm s}=\begin{pmatrix}\tan\alpha/\tan\beta&0\\0&1\end{pmatrix},\qquad
K_{\rm f}=\begin{pmatrix}\sqrt{1-\tan^2\alpha/\tan^2\beta}&0\\0&0\end{pmatrix}.
$$

Since $0<\tan\alpha/\tan\beta<1$, these are valid and satisfy $K_{\rm s}^\dagger K_{\rm s}+K_{\rm f}^\dagger K_{\rm f}=I$. Alice sends Bob the success or failure outcome. The successful unnormalized branch is

$$
\begin{aligned}
(K_{\rm s}\otimes I)|\psi\rangle
&=\frac{\sin\alpha\cos\beta}{\sin\beta}|00\rangle+\sin\alpha|11\rangle\\
&=\frac{\sin\alpha}{\sin\beta}|\phi\rangle.
\end{aligned}
$$

Therefore the normalized success state is exactly the target and

$$
\boxed{p_{\rm succ}=\frac{\sin^2\alpha}{\sin^2\beta}=\frac{s}{t}=p_{\max}.}
$$

Bob needs no quantum correction in this known Schmidt basis. The failure branch is proportional to $|00\rangle$, a [product state](../../../../../../product-state.md), and has probability $1-s/t$. The successful branch saturates the previous bound: $p_{\rm succ}E_2(\phi)=E_2(\psi)$ and failure contributes zero. This establishes [optimal stochastic conversion of a two-qubit pure state](../../../../../../optimal-stochastic-conversion-of-a-two-qubit-pure-state.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
