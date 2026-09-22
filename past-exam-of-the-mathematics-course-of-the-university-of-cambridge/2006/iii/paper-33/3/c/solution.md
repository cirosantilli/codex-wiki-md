<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Successive uses of the same [quantum channel](../../../../../../quantum-channel.md) mean coupling to a fresh vacuum environment each time, or resetting the environment between uses. They do not mean repeatedly applying the dilation unitary to one unreinitialized two-state environment. Direct composition gives

$$
\mathcal A_p^2(\rho)=\begin{pmatrix}\rho_{00}+(2p-p^2)\rho_{11}&(1-p)\rho_{01}\\(1-p)\rho_{10}&(1-p)^2\rho_{11}\end{pmatrix}.
$$

Inductively, with $q_n=1-(1-p)^n$,

$$
\boxed{\mathcal A_p^n(\rho)=\begin{pmatrix}\rho_{00}+q_n\rho_{11}&(1-p)^{n/2}\rho_{01}\\(1-p)^{n/2}\rho_{10}&(1-p)^n\rho_{11}\end{pmatrix}.}
$$

For $0<p\le1$, this tends to the pure ground state $|0\rangle\langle0|$, whose [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is zero. For $p=0$, the channel is the identity: the state remains $\rho$ and its [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) remains $S(\rho)$. Thus the [repeated amplitude damping limit](../../../../../../repeated-amplitude-damping-limit.md) must include this no-decay exception.

A zero-[Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) output means there is no uncertainty about the final atomic state. It does not mean that the receiver has gained information about the initial preparation: all initial states have the same limiting output, so their distinguishability has been erased from the atom. Under the global unitary evolution, information is carried into the environment. Without observing an emission record, this is a nonselective dissipative process, not an inference about which input was sent. Indeed, starting from the excited [pure state](../../../../../../pure-state.md), one intermediate output has [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) equal to the [binary entropy](../../../../../../binary-entropy.md) of $p$, which is positive for $0<p<1$; the atom's [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) need not decrease monotonically during the approach to the final ground state.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
