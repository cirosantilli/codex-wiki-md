<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $P_\phi=|\phi\rangle\langle\phi|$. An arbitrary deterministic strategy, including auxiliary systems, intermediate measurements, adaptive actions and discarded records, is a [quantum channel](../../../../../quantum-channel.md) $\mathcal E$ from the two input qubits to the three returned qubits. Its output is $R_\phi=\mathcal E(P_\phi^{\otimes2})$. The three local tests commute, and their joint all-pass projector is $P_\phi^{\otimes3}$. Thus

$$
\epsilon_\phi=1-\operatorname{Tr}(P_\phi^{\otimes3}R_\phi)
$$

is exactly the [probability](../../../../../probability.md) of at least one failed test. No independence of the three returned qubits is assumed.

We prove a uniform positive obstruction using [trace distance](../../../../../trace-distance.md), $D(\rho,\sigma)=\|\rho-\sigma\|_1/2$. Two normalized pure kets obey

$$
D(|u\rangle\langle u|,|v\rangle\langle v|)=\sqrt{1-|\langle u|v\rangle|^2}.
$$

Indeed their projector difference is supported on their two-dimensional span, has trace zero, and has [eigenvalues](../../../../../eigenvalue.md) $\pm\sqrt{1-|\langle u|v\rangle|^2}$.

Two further estimates will cover even mixed outputs. First, [trace distance](../../../../../trace-distance.md) contracts under a [quantum channel](../../../../../quantum-channel.md). To see this directly, the positive spectral projector of the trace-zero difference gives $D(\rho,\sigma)=\max_{0\leq A\leq I}\operatorname{Tr}[A(\rho-\sigma)]$. The adjoint of a channel is positive and unital, so it takes any output effect into an input effect. Maximizing over this subset cannot exceed the input maximum, proving contraction.

Second, for a mixed state $R=\sum_jq_j|u_j\rangle\langle u_j|$ and a pure target $P=|v\rangle\langle v|$, the trace-norm triangle inequality and weighted [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) give the [pure-target upper bound on trace distance](../../../../../pure-target-upper-bound-on-trace-distance.md):

$$
D(R,P)\leq\sum_jq_j\sqrt{1-|\langle u_j|v\rangle|^2}
\leq\sqrt{1-\langle v|R|v\rangle}.
$$

In particular $D(R_\phi,P_\phi^{\otimes3})\leq\sqrt{\epsilon_\phi}$.

Now take $|\phi_0\rangle=|0\rangle$ and $|\phi_1\rangle=|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$. The two-copy input distance is $D_2=\sqrt{1-1/4}=\sqrt3/2$, whereas the ideal three-copy distance is $D_3=\sqrt{1-1/8}=\sqrt{7/8}$. Writing $R_j=R_{\phi_j}$, contraction and the triangle inequality yield

$$
D_3\leq D(P_{\phi_0}^{\otimes3},R_0)+D(R_0,R_1)+D(R_1,P_{\phi_1}^{\otimes3})
\leq\sqrt{\epsilon_0}+D_2+\sqrt{\epsilon_1}.
$$

Let $\delta=D_3-D_2>0$. Then $\sqrt{\epsilon_0}+\sqrt{\epsilon_1}\geq\delta$, and squaring gives

$$
\boxed{\frac{\epsilon_0+\epsilon_1}{2}\geq\frac{\delta^2}{4}>0.}
$$

This is the [copy-number trace-distance obstruction](../../../../../copy-number-trace-distance-obstruction.md). It applies to every Bob strategy, irrespective of its internal complexity. If Alice chooses these two possible inputs with equal [probabilities](../../../../../probability.md), the left side is her unconditional failure [probability](../../../../../probability.md). For every device, at least one of the two inputs also has failure [probability](../../../../../probability.md) at least $\delta^2/4$, establishing the worst-case guarantee.

The same positive bound holds if Alice chooses a uniformly random pure-qubit state. Apply the preceding inequality to $U|0\rangle$ and $U|+\rangle$ for every single-qubit unitary $U$, since their overlap is unchanged. Average over normalized [Haar measure](../../../../../haar-measure.md). Both rotated kets have the same uniform distribution on the [Bloch sphere](../../../../../bloch-sphere.md), so each of the two average failures is the uniform-input average. Consequently that average is also at least $\delta^2/4$. A constant satisfying the strict requested inequality in either this average or the worst-case interpretation is

$$
\boxed{p=\frac18\left(\sqrt{\frac78}-\frac{\sqrt3}{2}\right)^2>0.}
$$

The proven bound is $2p$, hence strictly greater than $p$. This proof establishes a quantitative gap, rather than relying only on the impossibility of exact [quantum cloning](../../../../../quantum-cloning.md).

There is a necessary quantifier qualification because the PDF does not specify Alice's input distribution. A positive lower bound for every fixed state against every strategy would be false: a device hardwired to return $|000\rangle$ never fails when the input is $|0\rangle^{\otimes2}$. The unknown-state assertion is therefore meaningful as a worst-case guarantee over possible inputs, or as an average for a specified hidden input ensemble. Both the equal-prior example and the uniform-input version have been proved here, with a constant independent of Bob's strategy.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
