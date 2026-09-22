<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write a qubit density operator as $\rho=(I+\mathbf r\cdot\boldsymbol\sigma)/2$, with [Bloch vector](../../../../../../bloch-vector.md) $|\mathbf r|\leq1$. The [depolarizing channel](../../../../../../quantum-depolarizing-channel.md) sends $\mathbf r$ to $p\mathbf r$. Its output eigenvalues are $(1\pm |p||\mathbf r|)/2$, so its [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is minimized at $|\mathbf r|=1$. Define

$$
\boxed{q=(1-p)/2}.
$$

The minimum output entropy is $h(q)$, since binary entropy is symmetric under $q\mapsto1-q$. The usual probabilistic-mixture convention has $0\leq p\leq1$. The argument also holds throughout the physical qubit CPTP range $-1/3\leq p\leq1$, where this $q$ still lies in $[0,1]$.

To handle multiple channel uses, let a classical message $x$ select a product input $\rho_x=\bigotimes_{j=1}^n\rho_{xj}$ with probability $\pi_x$. Memorylessness gives product outputs $\sigma_x=\bigotimes_j\Phi(\rho_{xj})$. Additivity of [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) on tensor products gives $S(\sigma_x)\geq n h(q)$. The average output $\bar\sigma=\sum_x\pi_x\sigma_x$ acts on $n$ qubits, so $S(\bar\sigma)\leq\log_2(2^n)=n$. Thus the [Holevo quantity](../../../../../../holevo-quantity.md) obeys the [product-input block bound for a qubit depolarizing channel](../../../../../../product-input-block-bound-for-a-qubit-depolarizing-channel.md)

$$
\chi=S(\bar\sigma)-\sum_x\pi_xS(\sigma_x)\leq n[1-h(q)].
$$

The [Holevo bound](../../../../../../holevo-s-theorem.md) says the classical [mutual information](../../../../../../mutual-information.md) obtained by any measurement, including a joint measurement on all outputs, is at most $\chi$.

For a reliable code with $M$ equiprobable messages and decoding error $P_e$, [Fano's inequality](../../../../../../fano-s-inequality.md) gives $H(X\mid\hat X)\leq h(P_e)+P_e\log_2(M-1)$. Consequently $(1-P_e)\log_2M\leq n[1-h(q)]+h(P_e)$. Letting the error tend to zero proves **$\boxed{\mathcal I(\Phi)\leq1-h((1-p)/2)}$.**

The bound is tight: equal use of $|0\rangle,|1\rangle$ and computational-basis output measurements produce a [binary symmetric channel](../../../../../../binary-symmetric-channel.md) with crossover probability $q$. Ordinary classical coding achieves $1-h(q)$ bits per use.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
