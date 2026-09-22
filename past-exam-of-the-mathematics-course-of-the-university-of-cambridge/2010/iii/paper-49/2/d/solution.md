<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [two-bit remote state preparation on a graph-state path](../../../../../../two-bit-remote-state-preparation-on-a-graph-state-path.md). Alice performs the first two measurements from the preceding [measurement-based quantum computation](../../../../../../measurement-based-quantum-computation.md): angle $\alpha$ on her first qubit, giving $r$, then angle $(-1)^r\beta$ on her second, giving $s$. She sends the pair $(r,s)$ to Bob, using exactly two [classical communication](../../../../../../classical-communication.md) bits.

The branch calculation already gives Bob's state as $e^{ir\beta}X^sZ^r|\chi\rangle$, where $|\chi\rangle=U(\beta)U(\alpha)|+\rangle$. Bob applies $X^s$ first and $Z^r$ second, so his correction operator is $Z^rX^s$. Since $X^2=Z^2=I$,

$$
(Z^rX^s)(X^sZ^r)|\chi\rangle=|\chi\rangle.
$$

Thus

$$
\boxed{\text{Alice sends }(r,s);\qquad\text{Bob applies }Z^rX^s.}
$$

The final state is exactly the desired state up to the irrelevant global phase. No postselection is used: all four measurement branches have probability $1/4$ and are corrected. Bob does not need the angles themselves; Alice uses them in her measurement choices, while the two bits specify his Pauli correction.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
