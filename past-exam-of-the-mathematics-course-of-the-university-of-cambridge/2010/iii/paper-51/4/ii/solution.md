<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the first copy to determine computational-basis parity and the second to determine phase parity. On the first pair, Alice and Bob each measure the [Pauli operator](../../../../../../pauli-operator.md) $Z$ and communicate their signs $z_A,z_B$. On the second, each measures $X$ in the $|+\rangle,|-\rangle$ basis and communicates the signs $x_A,x_B$.

Every [Bell state](../../../../../../bell-state-split.md) is an eigenstate of both $Z\otimes Z$ and $X\otimes X$. Direct application to its two basis terms gives the table

$$
\begin{array}{c|cc}
\text{state}&z_Az_B&x_Ax_B\\\hline
\Phi^+&+1&+1\\
\Phi^-&+1&-1\\
\Psi^+&-1&+1\\
\Psi^-&-1&-1
\end{array}
$$

For example, $Z\otimes Z$ acts positively on $|00\rangle,|11\rangle$ and negatively on $|01\rangle,|10\rangle$; $X\otimes X$ exchanges the two terms in each pair, detecting their relative sign. Thus individual outcomes are random, but the products in the table are certain. The [Bell parity and phase observables](../../../../../../bell-parity-and-phase-observables.md) label the state uniquely.

**The two communicated parities identify all four states with probability one.** Each measurement is local and all remaining operations are classical, so the protocol is [LOCC discrimination of four Bell states using two copies](../../../../../../locc-discrimination-of-four-bell-states-using-two-copies.md). Alice can simply send her two signs to Bob, who combines them with his own. Measuring $Z$ on the first copy destroys its phase information, but the second identical copy still supplies it; this is why the two-copy assumption enables this protocol.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
