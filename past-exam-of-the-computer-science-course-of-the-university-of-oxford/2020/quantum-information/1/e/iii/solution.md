<h1 id="1/e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $R=\operatorname{diag}(1,e^{i\pi/12})$. Since the [Hadamard gate](../../../../../../hadamard-gate.md) maps the standard [basis](../../../../../../basis.md) to $|+\rangle,|-\rangle$, the given gate is $Q=HRH$. Because $H^2=I$,

$$
Q^3=HR^3H=HTH,\qquad\boxed{T=HQ^3H.}
$$

Next, use $HZH=X$ on the target wire of the [Controlled-Z gate](../../../../../../controlled-z-gate.md):

$$
\boxed{\mathrm{CNOT}=(I\otimes H)\,CZ\,(I\otimes H).}
$$

The control-zero block remains the identity, and the control-one block becomes $HZH=X$, proving the identity with the stated control convention. We have therefore constructed each gate in the assumed [universal quantum gate set](../../../../../../universal-quantum-gate-set.md) $\{\mathrm{CNOT},H,T\}$ using only $CZ,Q,H$.

Replacing every gate of a circuit by its displayed finite construction reproduces that circuit exactly. Thus **$\{CZ,Q,H\}$ is universal** under the usual arbitrary-accuracy convention: it can perform every approximation obtainable from the given universal set. The claim concerns approximation of arbitrary [unitary operators](../../../../../../unitary-operator.md); it does not assert that finitely many circuits exactly represent an uncountable continuum of gates. This is [universality transfer by exact gate synthesis](../../../../../../universality-transfer-by-exact-gate-synthesis.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [E](../../e.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
