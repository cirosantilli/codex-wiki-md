<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Interpret the requested measurement as distinguishing all four stated orthogonal [eigenstates](../../../../../../eigenstate.md), hence as their rank-one [projective measurement](../../../../../../projective-measurement.md). If they have indistinguishable degenerate [eigenvalues](../../../../../../eigenvalue.md), this assumption need not hold; the identity observable, for example, cannot reveal the basis and gives no contradiction.

Let Bob initially prepare $|0\rangle_B$. Alice encodes a bit by preparing $|0\rangle_A$ or $|1\rangle_A$, without changing Bob's initial [reduced density matrix](../../../../../../reduced-density-matrix.md). If Alice prepares zero, the global input is the first [eigenstate](../../../../../../eigenstate.md), so nondemolition leaves Bob in $|0\rangle$ with certainty. If Alice prepares one, the rank-one [Lüders rule](../../../../../../luders-rule.md), after discarding the outcome, dephases Bob in the rotated basis

$$
|u\rangle=\cos\theta|0\rangle+\sin\theta|1\rangle,
\qquad |v\rangle=\sin\theta|0\rangle-\cos\theta|1\rangle.
$$

His output is $\rho_B=\cos^2\theta|u\rangle\langle u|+\sin^2\theta|v\rangle\langle v|$. A computational-basis measurement then gives

$$
\boxed{\Pr_B(1\mid A=0)=0,\qquad
\Pr_B(1\mid A=1)=2\sin^2\theta\cos^2\theta=\tfrac12\sin^2(2\theta).}
$$

It is positive for every $0<\theta\leq\pi/4$. Repeating the experiment would transmit Alice's choice across a spacelike interval, violating [quantum no-signalling](../../../../../../quantum-no-signalling.md). The [controlled-basis measurement causality obstruction](../../../../../../controlled-basis-measurement-causality-obstruction.md) therefore excludes the entire nonzero interval, including $\pi/4$.

At **$\theta=0$**, the basis is the computational product basis, up to an irrelevant sign on the fourth vector. Alice and Bob each measure $Z$ locally, then compare their results later. Each product [eigenstate](../../../../../../eigenstate.md) is preserved. Thus being a product basis is insufficient for an instantaneous [quantum nondemolition measurement](../../../../../../quantum-nondemolition-measurement.md): a remote party's choice of which local basis is measured can still cause signalling.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
