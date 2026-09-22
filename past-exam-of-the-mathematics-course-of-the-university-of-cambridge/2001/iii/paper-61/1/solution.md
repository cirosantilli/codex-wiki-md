<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose a real [unitary matrix](../../../../../unitary-matrix.md) and undo it at the second stage:

$$
U=\begin{pmatrix}\sqrt q&-\sqrt p\\ \sqrt p&\sqrt q\end{pmatrix},
\qquad U'=U^\dagger,\qquad 0<p<1,\quad q=1-p.
$$

After the first rotation the [photon](../../../../../photon.md) [qubit](../../../../../qubit.md) is $\sqrt q\,|0\rangle+\sqrt p\,|1\rangle$. A dud leaves this [quantum superposition](../../../../../quantum-superposition.md) unchanged, so the inverse rotation restores $|0\rangle$. Its final [projective measurement](../../../../../projective-measurement.md) can never return $1$.

For a live bomb the absorbing component explodes with [probability](../../../../../probability.md) $p$. If the [photon](../../../../../photon.md) survives, the normalized state is $|0\rangle$, and the second rotation makes it $\sqrt q\,|0\rangle-\sqrt p\,|1\rangle$. The unconditional probabilities of the three possible live-bomb outcomes are consequently

$$
P(\text{explosion})=p,\qquad
P(\text{safe certification})=qp,\qquad
P(\text{inconclusive})=q^2.
$$

They sum to one. The nonexplosive result $1$ certifies a live bomb because its dud probability is exactly zero. The inconclusive result $0$ resets the [qubit](../../../../../qubit.md) to its original state, allowing another identical trial.

The [repeated weak-rotation bomb-test efficiency](../../../../../repeated-weak-rotation-bomb-test-efficiency.md) follows by summing the [geometric series](../../../../../geometric-series.md) over the first successful trial:

$$
P_N=pq\sum_{j=0}^{N-1}q^{2j}
=\frac{q}{1+q}(1-q^{2N}),\qquad
\boxed{P_\infty=\frac{q}{1+q}=\frac{1-p}{2-p}\longrightarrow\frac12
\quad\text{as }p\downarrow0.}
$$

This is conditional on testing a live bomb, not an average over an unspecified prior fraction of duds. To make the finite-run success probability exceed $1/2-\varepsilon$, choose positive $p$ so that $p/[2(2-p)]<\varepsilon/2$, then choose $N$ so that $q^{2N}<\varepsilon/2$. The first condition controls the limiting deficit and the second controls the remaining tail. Exactly $p=0$ yields no explosion but also no information, so the limit must be approached with nonzero weak rotations.

The half-efficiency limit is consistent with the structure of this [Elitzur-Vaidman bomb tester](../../../../../elitzur-vaidman-bomb-tester.md). Suppose generally $U|0\rangle=a|0\rangle+b|1\rangle$. A final outcome that certifies a live bomb must be orthogonal to the dud output $U'U|0\rangle$. Pulling this outcome backwards through $U'$ gives the normalized vector orthogonal to $(a,b)$. Its squared overlap with $|0\rangle$ is $|b|^2$. Thus the safe-certification probability is $|a|^2|b|^2$, whereas the explosion probability is $|b|^2$. The former never exceeds the latter. Summing these mutually exclusive terminal events over repeated, possibly adaptive trials gives $P_{\rm safe}\leq P_{\rm explosion}$ and hence $P_{\rm safe}\leq1/2$. This concerns the specified rotate–interact–rotate–measure protocol.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
